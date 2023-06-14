# Comparing `tmp/returnn-1.20230609.82609.tar.gz` & `tmp/returnn-1.20230614.134509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230609.82609.tar", last modified: Fri Jun  9 06:52:10 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230614.134509.tar", last modified: Wed Jun 14 12:10:12 2023, max compression
```

## Comparing `returnn-1.20230609.82609.tar` & `returnn-1.20230614.134509.tar`

### file list

```diff
@@ -1,447 +1,448 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25269 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-09 06:51:47.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-09 06:51:51.000000 returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99527 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   157757 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151839 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   150722 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586670 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   297063 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31004 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   552442 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:52:10.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-09 06:51:45.000000 returnn-1.20230609.82609/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63112 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 12:09:51.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-14 12:09:54.000000 returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99665 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151839 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40159 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150722 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586670 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   539876 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   297063 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35124 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72173 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   552605 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:10:12.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-14 12:09:49.000000 returnn-1.20230614.134509/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230609.82609/.gitignore` & `returnn-1.20230614.134509/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/.gitmodules` & `returnn-1.20230614.134509/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/CHANGELOG.md` & `returnn-1.20230614.134509/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/CODEOWNERS` & `returnn-1.20230614.134509/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/CONTRIBUTING.md` & `returnn-1.20230614.134509/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/LICENSE` & `returnn-1.20230614.134509/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/MANIFEST.in` & `returnn-1.20230614.134509/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/PKG-INFO` & `returnn-1.20230614.134509/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230609.82609
+Version: 1.20230614.134509
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230609.82609/README.rst` & `returnn-1.20230614.134509/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/__init__.py` & `returnn-1.20230614.134509/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/12AX.cluster_map` & `returnn-1.20230614.134509/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-fwd.config` & `returnn-1.20230614.134509/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-horovod-mpi.py` & `returnn-1.20230614.134509/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230614.134509/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-hyper-param-tuning.config` & `returnn-1.20230614.134509/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-iter-dataset.py` & `returnn-1.20230614.134509/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-list-devices.py` & `returnn-1.20230614.134509/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-lua-torch-layer.config` & `returnn-1.20230614.134509/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230614.134509/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-returnn-as-framework.py` & `returnn-1.20230614.134509/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-rf.config` & `returnn-1.20230614.134509/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-rhn-enwik8.config` & `returnn-1.20230614.134509/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-sprint-interface.py` & `returnn-1.20230614.134509/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-att-copy.config` & `returnn-1.20230614.134509/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-attention.config` & `returnn-1.20230614.134509/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230614.134509/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230614.134509/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-enc-dec.config` & `returnn-1.20230614.134509/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230614.134509/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230614.134509/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230614.134509/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230614.134509/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230614.134509/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230614.134509/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230614.134509/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230614.134509/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230614.134509/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230614.134509/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-rec-self-att.config` & `returnn-1.20230614.134509/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230614.134509/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230614.134509/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230614.134509/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-torch.config` & `returnn-1.20230614.134509/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230614.134509/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/demo.sh` & `returnn-1.20230614.134509/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230614.134509/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/README.txt` & `returnn-1.20230614.134509/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/config_demo` & `returnn-1.20230614.134509/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230614.134509/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/config_real` & `returnn-1.20230614.134509/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230614.134509/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/decode.py` & `returnn-1.20230614.134509/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230614.134509/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230614.134509/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230614.134509/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230614.134509/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230614.134509/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230614.134509/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230614.134509/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230614.134509/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/__init__.py` & `returnn-1.20230614.134509/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/__main__.py` & `returnn-1.20230614.134509/returnn/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,25 @@
         OpMaker.log_stream = log.v3
         tf_util.debug_register_better_repr()
         if config.is_true("distributed_tf"):
             import returnn.tf.distributed
 
             returnn.tf.distributed.init_distributed_tf(config)
     elif BackendEngine.is_torch_selected():
+        if config.typed_value("torch_distributed") is not None:
+            import socket
+            import returnn.torch.distributed
+
+            torch_distributed = returnn.torch.distributed.get_ctx(config=config)
+            print(
+                "Torch: Hostname %s, pid %i, using GPU %s."
+                % (socket.gethostname(), os.getpid(), str(torch_distributed.local_rank())),
+                file=log.v3,
+            )
+
         print("PyTorch:", util.describe_torch_version(), file=log.v3)
     else:
         raise NotImplementedError
 
 
 def init(config_filename=None, command_line_options=(), config_updates=None, extra_greeting=None):
     """
@@ -382,14 +393,19 @@
     if engine:
         if BackendEngine.is_tensorflow_selected():
             engine.finalize(error_occurred=error_occurred)
             if config.is_true("use_horovod"):
                 import horovod.tensorflow as hvd  # noqa
 
                 hvd.shutdown()
+        elif BackendEngine.is_torch_selected():
+            if config.typed_value("torch_distributed") is not None:
+                from torch.distributed import destroy_process_group
+
+                destroy_process_group()
 
 
 def need_data():
     """
     :return: whether we need to init the data (call :func:`init_data`) for the current task (:func:`execute_main_task`)
     :rtype: bool
     """
```

### Comparing `returnn-1.20230609.82609/returnn/__old_mod_loader__.py` & `returnn-1.20230614.134509/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/__setup__.py` & `returnn-1.20230614.134509/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/config.py` & `returnn-1.20230614.134509/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/audio.py` & `returnn-1.20230614.134509/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/basic.py` & `returnn-1.20230614.134509/returnn/datasets/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,14 +241,19 @@
         if not config:
             return 0
         if config.is_true("use_horovod"):
             import returnn.tf.horovod
 
             if returnn.tf.horovod.get_ctx().is_dataset_distribution_random_seed_offset():
                 return returnn.tf.horovod.get_ctx().rank() * 16127
+
+        if config.typed_value("torch_distributed") is not None:
+            import returnn.torch.distributed
+
+            return returnn.torch.distributed.get_ctx().rank() * 16127
         return 0
 
     @staticmethod
     def _parse_chunking(chunking):
         """
         :param None|str|int|(int,int)|dict|(dict,dict)|(NumbersDict,NumbersDict)|function chunking:
           as it comes from the config / from the user
```

### Comparing `returnn-1.20230609.82609/returnn/datasets/bundle_file.py` & `returnn-1.20230614.134509/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/cached.py` & `returnn-1.20230614.134509/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/cached2.py` & `returnn-1.20230614.134509/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/generating.py` & `returnn-1.20230614.134509/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/hdf.py` & `returnn-1.20230614.134509/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/lm.py` & `returnn-1.20230614.134509/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/map.py` & `returnn-1.20230614.134509/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/meta.py` & `returnn-1.20230614.134509/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/multi_proc.py` & `returnn-1.20230614.134509/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/normalization_data.py` & `returnn-1.20230614.134509/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/numpy_dump.py` & `returnn-1.20230614.134509/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/raw_wav.py` & `returnn-1.20230614.134509/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/sprint.py` & `returnn-1.20230614.134509/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/stereo.py` & `returnn-1.20230614.134509/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230614.134509/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/datasets/util/vocabulary.py` & `returnn-1.20230614.134509/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/engine/base.py` & `returnn-1.20230614.134509/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/engine/batch.py` & `returnn-1.20230614.134509/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230614.134509/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230614.134509/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230614.134509/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230614.134509/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/graph_editor/edit.py` & `returnn-1.20230614.134509/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230614.134509/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/graph_editor/select.py` & `returnn-1.20230614.134509/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230614.134509/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/graph_editor/transform.py` & `returnn-1.20230614.134509/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/extern/graph_editor/util.py` & `returnn-1.20230614.134509/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/forward_iface.py` & `returnn-1.20230614.134509/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/__init__.py` & `returnn-1.20230614.134509/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/_backend.py` & `returnn-1.20230614.134509/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/_numpy_backend.py` & `returnn-1.20230614.134509/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/_utils.py` & `returnn-1.20230614.134509/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/array_.py` & `returnn-1.20230614.134509/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/attention.py` & `returnn-1.20230614.134509/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/cond.py` & `returnn-1.20230614.134509/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/const.py` & `returnn-1.20230614.134509/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/container.py` & `returnn-1.20230614.134509/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/conv.py` & `returnn-1.20230614.134509/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/device.py` & `returnn-1.20230614.134509/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/dims.py` & `returnn-1.20230614.134509/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/dropout.py` & `returnn-1.20230614.134509/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/dtype.py` & `returnn-1.20230614.134509/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/encoder/base.py` & `returnn-1.20230614.134509/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/encoder/conformer.py` & `returnn-1.20230614.134509/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/init.py` & `returnn-1.20230614.134509/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/linear.py` & `returnn-1.20230614.134509/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/loop.py` & `returnn-1.20230614.134509/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/loss.py` & `returnn-1.20230614.134509/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/math_.py` & `returnn-1.20230614.134509/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/matmul.py` & `returnn-1.20230614.134509/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/module.py` & `returnn-1.20230614.134509/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/normalization.py` & `returnn-1.20230614.134509/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/parameter.py` & `returnn-1.20230614.134509/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/rand.py` & `returnn-1.20230614.134509/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/rec.py` & `returnn-1.20230614.134509/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/reduce.py` & `returnn-1.20230614.134509/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/run_ctx.py` & `returnn-1.20230614.134509/returnn/frontend/run_ctx.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,16 @@
             # The expected output usually comes from `model_outputs` from the user config.
             # The dimensions of `expected_output` and `tensor` should match,
             # but we can't directly check for expected_output.dims == tensor.dims
             # because not all dims can be known in advance in `expected_output`,
             # e.g. dynamic dims.
             # Thus, we allow undefined dims in the expected output,
             # and ignore them when checking for equality.
+            # The most important thing for the user is to define what dims are dynamic and what dims are static.
+            # This is also necessary for ONNX export.
             assert len(expected_output.dims) == len(tensor.dims), (
                 f"mark_as_output: lengths of expected output {expected_output.dims}"
                 f" and actual output {tensor.dims} don't match."
             )
             for expected_dim, actual_dim in zip(expected_output.dims, tensor.dims):
                 expected_dim: Dim
                 actual_dim: Dim
@@ -231,18 +233,20 @@
                     )
                 elif expected_dim.is_dynamic():
                     assert actual_dim.is_dynamic(), (
                         f"mark_as_output: expected dim {expected_dim} is dynamic."
                         f" Matching actual dim assumed to be dynamic, but got non-dynamic dim {actual_dim}."
                     )
                 elif expected_dim.is_static():
-                    assert actual_dim is expected_dim, (
+                    assert expected_dim.is_static() and actual_dim.dimension == expected_dim.dimension, (
                         f"mark_as_output: expected dim {expected_dim} is static."
-                        f" Matching actual dim assumed to be the same static dim, but got {actual_dim}."
+                        f" Matching actual dim assumed to be the same static dim value, but got {actual_dim}."
                     )
+                else:
+                    assert False, f"mark_as_output: unexpected expected dim {expected_dim}."
             assert expected_output.dtype == tensor.dtype, (
                 f"mark_as_output: {name!r} dtype mismatch from expected output,"
                 f" given {tensor.dtype}, expected {expected_output.dtype}"
             )
             assert expected_output.sparse_dim == tensor.sparse_dim, (
                 f"mark_as_output: {name!r} sparse_dim mismatch from expected output,"
                 f" given {tensor.sparse_dim}, expected {expected_output.sparse_dim}"
```

### Comparing `returnn-1.20230609.82609/returnn/frontend/signal.py` & `returnn-1.20230614.134509/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/state.py` & `returnn-1.20230614.134509/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/tensor_array.py` & `returnn-1.20230614.134509/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/frontend/types.py` & `returnn-1.20230614.134509/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/import_/common.py` & `returnn-1.20230614.134509/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/import_/git.py` & `returnn-1.20230614.134509/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/import_/import_.py` & `returnn-1.20230614.134509/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/learning_rate_control.py` & `returnn-1.20230614.134509/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/log.py` & `returnn-1.20230614.134509/returnn/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,26 @@
             hvd = returnn.tf.horovod.get_ctx(config=config)
             new_logs = []
             for fn in logs:
                 fn_prefix, fn_ext = os.path.splitext(fn)
                 fn_ext = ".horovod-%i-%i%s" % (hvd.rank(), hvd.size(), fn_ext)
                 new_logs.append(fn_prefix + fn_ext)
             logs = new_logs
+
+        if config.typed_value("torch_distributed") is not None:
+            import returnn.torch.distributed
+
+            torch_distributed = returnn.torch.distributed.get_ctx(config=config)
+            new_logs = []
+            for fn in logs:
+                fn_prefix, fn_ext = os.path.splitext(fn)
+                fn_ext = ".torch-distrib-%i-%i%s" % (torch_distributed.rank(), torch_distributed.size(), fn_ext)
+                new_logs.append(fn_prefix + fn_ext)
+            logs = new_logs
+
         self.initialize(logs=logs, verbosity=log_verbosity, formatter=log_format)
 
     def print_warning(self, text, prefix_text="WARNING:", extra_text=None):
         """
         Write a warning to log.v2. Does not write repeated warnings.
 
         :param str text:
```

### Comparing `returnn-1.20230609.82609/returnn/native_op.cpp` & `returnn-1.20230614.134509/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/native_op.py` & `returnn-1.20230614.134509/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/pretrain.py` & `returnn-1.20230614.134509/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/sprint/cache.py` & `returnn-1.20230614.134509/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/sprint/control.py` & `returnn-1.20230614.134509/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/sprint/error_signals.py` & `returnn-1.20230614.134509/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/sprint/extern_interface.py` & `returnn-1.20230614.134509/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/sprint/interface.py` & `returnn-1.20230614.134509/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tensor/_dim_extra.py` & `returnn-1.20230614.134509/returnn/tensor/_dim_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -976,5246 +976,5255 @@
 00003cf0: 676e 6f72 6520 7468 6520 6374 7820 666f  gnore the ctx fo
 00003d00: 7220 7468 6520 6261 7463 6820 6469 6d20  r the batch dim 
 00003d10: 6375 7272 656e 746c 792e 0a20 2020 2020  currently..     
 00003d20: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
 00003d30: 6174 6368 203d 3d20 6261 7463 683a 0a20  atch == batch:. 
 00003d40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
 00003d50: 6574 7572 6e20 7365 6c66 0a20 2020 2020  eturn self.     
-00003d60: 2020 2020 2020 2072 6574 7572 6e20 5f64         return _d
-00003d70: 2e44 696d 286b 696e 643d 4469 6d54 7970  .Dim(kind=DimTyp
-00003d80: 6573 2e42 6174 6368 2c20 6465 7363 7269  es.Batch, descri
-00003d90: 7074 696f 6e3d 2262 6174 6368 3a25 7322  ption="batch:%s"
-00003da0: 2025 2062 6174 6368 2e73 686f 7274 5f72   % batch.short_r
-00003db0: 6570 7228 292c 2062 6174 6368 3d62 6174  epr(), batch=bat
-00003dc0: 6368 2c20 6469 6d65 6e73 696f 6e3d 4e6f  ch, dimension=No
-00003dd0: 6e65 290a 2020 2020 2020 2020 6966 206e  ne).        if n
-00003de0: 6f74 2073 656c 662e 6973 5f64 796e 616d  ot self.is_dynam
-00003df0: 6963 2829 3a0a 2020 2020 2020 2020 2020  ic():.          
-00003e00: 2020 2320 4966 2073 7461 7469 6320 6469    # If static di
-00003e10: 6d2c 206e 6f20 6566 6665 6374 2e0a 2020  m, no effect..  
-00003e20: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00003e30: 206e 6f74 2073 656c 662e 6261 7463 680a   not self.batch.
-00003e40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00003e50: 726e 2073 656c 660a 2020 2020 2020 2020  rn self.        
-00003e60: 6966 2062 6174 6368 2e69 735f 6272 6f61  if batch.is_broa
-00003e70: 6463 6173 7428 293a 0a20 2020 2020 2020  dcast():.       
-00003e80: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00003e90: 2020 2320 6a75 7374 206c 6561 7665 2061    # just leave a
-00003ea0: 732d 6973 2e20 7368 6f75 6c64 206e 6f74  s-is. should not
-00003eb0: 206d 6174 7465 722e 0a20 2020 2020 2020   matter..       
-00003ec0: 2069 6620 7365 6c66 2e5f 6578 7472 613a   if self._extra:
-00003ed0: 0a20 2020 2020 2020 2020 2020 2073 616d  .            sam
-00003ee0: 655f 6261 7365 203d 2073 656c 662e 6765  e_base = self.ge
-00003ef0: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
-00003f00: 2020 2020 2020 2020 2020 7361 6d65 5f62            same_b
-00003f10: 6173 652e 5f76 616c 6964 6174 655f 696e  ase._validate_in
-00003f20: 5f63 7572 7265 6e74 5f67 7261 7068 2829  _current_graph()
-00003f30: 0a20 2020 2020 2020 2020 2020 2023 206e  .            # n
-00003f40: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
-00003f50: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
-00003f60: 2020 2020 2020 2020 2020 6966 2073 616d            if sam
-00003f70: 655f 6261 7365 2e5f 6578 7472 613a 0a20  e_base._extra:. 
-00003f80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00003f90: 726f 6d20 7265 7475 726e 6e2e 7466 2e75  rom returnn.tf.u
-00003fa0: 7469 6c2e 6461 7461 2069 6d70 6f72 7420  til.data import 
-00003fb0: 436f 6e74 726f 6c46 6c6f 7743 6f6e 7465  ControlFlowConte
-00003fc0: 7874 0a0a 2020 2020 2020 2020 2020 2020  xt..            
-00003fd0: 2020 2020 666f 7220 6374 785f 2069 6e20      for ctx_ in 
-00003fe0: 436f 6e74 726f 6c46 6c6f 7743 6f6e 7465  ControlFlowConte
-00003ff0: 7874 2e61 6273 5f63 7478 5f73 7461 636b  xt.abs_ctx_stack
-00004000: 5f77 6974 685f 726f 6f74 2863 7478 293a  _with_root(ctx):
-00004010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004020: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
-00004030: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
-00004040: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
-00004050: 2020 2020 2020 2020 2020 7461 6720 3d20            tag = 
-00004060: 7361 6d65 5f62 6173 652e 5f65 7874 7261  same_base._extra
-00004070: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-00004080: 6374 782e 6765 7428 2862 6174 6368 2c20  ctx.get((batch, 
-00004090: 6374 785f 292c 204e 6f6e 6529 0a20 2020  ctx_), None).   
-000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040b0: 2069 6620 7461 6720 616e 6420 7461 672e   if tag and tag.
-000040c0: 5f63 616e 5f75 7365 5f69 6e5f 6374 7828  _can_use_in_ctx(
-000040d0: 6374 7829 2061 6e64 2074 6167 2e5f 7661  ctx) and tag._va
-000040e0: 6c69 6461 7465 5f69 6e5f 6375 7272 656e  lidate_in_curren
-000040f0: 745f 6772 6170 6828 293a 0a20 2020 2020  t_graph():.     
-00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004110: 2020 2061 7373 6572 7420 280a 2020 2020     assert (.    
-00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004130: 2020 2020 2020 2020 7461 672e 6261 7463          tag.batc
-00004140: 6820 3d3d 2062 6174 6368 0a20 2020 2020  h == batch.     
-00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004160: 2020 2029 2020 2320 736f 6d65 2063 6f64     )  # some cod
-00004170: 6520 7570 6461 7465 6420 6261 7463 6820  e updated batch 
-00004180: 6469 7265 6374 6c79 2028 696e 636f 7272  directly (incorr
-00004190: 6563 746c 7929 2061 6e64 2063 6f75 6c64  ectly) and could
-000041a0: 2074 7269 6767 6572 2074 6869 730a 2020   trigger this.  
-000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041c0: 2020 2020 2020 7265 7475 726e 2074 6167        return tag
-000041d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000041e0: 7361 6d65 5f62 6173 652e 6261 7463 6820  same_base.batch 
-000041f0: 3d3d 2062 6174 6368 2061 6e64 2073 616d  == batch and sam
-00004200: 655f 6261 7365 2e5f 6361 6e5f 7573 655f  e_base._can_use_
-00004210: 696e 5f63 7478 2863 7478 2920 616e 6420  in_ctx(ctx) and 
-00004220: 7361 6d65 5f62 6173 652e 6479 6e5f 7369  same_base.dyn_si
-00004230: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
-00004240: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00004250: 616d 655f 6261 7365 0a20 2020 2020 2020  ame_base.       
-00004260: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00004270: 2020 2073 616d 655f 6261 7365 203d 2073     same_base = s
-00004280: 656c 660a 2020 2020 2020 2020 7361 6d65  elf.        same
-00004290: 5f62 6173 655f 6578 7472 6120 3d20 7361  _base_extra = sa
-000042a0: 6d65 5f62 6173 652e 5f6d 616b 655f 6578  me_base._make_ex
-000042b0: 7472 6128 290a 2020 2020 2020 2020 2320  tra().        # 
-000042c0: 4f6b 2c20 6e6f 7468 696e 6720 6d61 7463  Ok, nothing matc
-000042d0: 6869 6e67 2066 6f75 6e64 2e0a 2020 2020  hing found..    
-000042e0: 2020 2020 6966 2063 7478 3a0a 2020 2020      if ctx:.    
-000042f0: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
-00004300: 6966 2074 6865 2063 7478 2069 7320 7265  if the ctx is re
-00004310: 616c 6c79 2072 656c 6576 616e 742c 2077  ally relevant, w
-00004320: 6865 6e20 7468 6973 2069 7320 6465 7269  hen this is deri
-00004330: 7665 6420 6672 6f6d 206f 7468 6572 2074  ved from other t
-00004340: 6167 732e 0a20 2020 2020 2020 2020 2020  ags..           
-00004350: 2064 6572 6976 6564 5f62 6173 6573 203d   derived_bases =
-00004360: 2073 616d 655f 6261 7365 2e67 6574 5f64   same_base.get_d
-00004370: 6572 6976 6564 5f62 6173 6573 5f73 6574  erived_bases_set
-00004380: 2829 0a20 2020 2020 2020 2020 2020 2064  ().            d
-00004390: 6572 6976 6564 5f62 6173 6573 2e72 656d  erived_bases.rem
-000043a0: 6f76 6528 7361 6d65 5f62 6173 6529 0a20  ove(same_base). 
-000043b0: 2020 2020 2020 2020 2020 2069 6620 6465             if de
-000043c0: 7269 7665 645f 6261 7365 733a 0a20 2020  rived_bases:.   
-000043d0: 2020 2020 2020 2020 2020 2020 2064 6572               der
-000043e0: 6976 6564 5f63 7478 7320 3d20 7365 7428  ived_ctxs = set(
-000043f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004400: 2020 666f 7220 6420 696e 2064 6572 6976    for d in deriv
-00004410: 6564 5f62 6173 6573 3a0a 2020 2020 2020  ed_bases:.      
-00004420: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00004430: 7468 2075 7469 6c2e 6775 6172 645f 696e  th util.guard_in
-00004440: 6669 6e69 7465 5f72 6563 7572 7369 6f6e  finite_recursion
-00004450: 285f 642e 4469 6d2e 6765 745f 666f 725f  (_d.Dim.get_for_
-00004460: 6261 7463 685f 6374 782c 2064 293a 0a20  batch_ctx, d):. 
-00004470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004480: 2020 2020 2020 2064 203d 2064 2e67 6574         d = d.get
-00004490: 5f66 6f72 5f62 6174 6368 5f63 7478 2862  _for_batch_ctx(b
-000044a0: 6174 6368 3d62 6174 6368 2c20 6374 783d  atch=batch, ctx=
-000044b0: 6374 7829 0a20 2020 2020 2020 2020 2020  ctx).           
-000044c0: 2020 2020 2020 2020 2069 6620 642e 636f           if d.co
-000044d0: 6e74 726f 6c5f 666c 6f77 5f63 7478 3a0a  ntrol_flow_ctx:.
-000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044f0: 2020 2020 2020 2020 6465 7269 7665 645f          derived_
-00004500: 6374 7873 2e61 6464 2864 2e63 6f6e 7472  ctxs.add(d.contr
-00004510: 6f6c 5f66 6c6f 775f 6374 7829 0a20 2020  ol_flow_ctx).   
-00004520: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004530: 6e6f 7420 6465 7269 7665 645f 6374 7873  not derived_ctxs
-00004540: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004550: 2020 2020 2020 6374 7820 3d20 4e6f 6e65        ctx = None
-00004560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004570: 2065 6c69 6620 6c65 6e28 6465 7269 7665   elif len(derive
-00004580: 645f 6374 7873 2920 3d3d 2031 3a0a 2020  d_ctxs) == 1:.  
-00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045a0: 2020 6374 7820 3d20 6465 7269 7665 645f    ctx = derived_
-000045b0: 6374 7873 2e70 6f70 2829 0a20 2020 2020  ctxs.pop().     
-000045c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000045d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000045e0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
-000045f0: 706c 656d 656e 7465 6445 7272 6f72 2822  plementedError("
-00004600: 6e6f 7420 7965 7420 696d 706c 656d 656e  not yet implemen
-00004610: 7465 643a 206d 756c 7469 706c 6520 6465  ted: multiple de
-00004620: 7269 7665 6420 6374 7873 3a20 2572 2220  rived ctxs: %r" 
-00004630: 2520 2864 6572 6976 6564 5f63 7478 732c  % (derived_ctxs,
-00004640: 2929 0a20 2020 2020 2020 2064 796e 5f73  )).        dyn_s
-00004650: 697a 655f 6578 7420 3d20 4e6f 6e65 0a20  ize_ext = None. 
-00004660: 2020 2020 2020 2023 204d 6179 6265 2077         # Maybe w
-00004670: 6520 6861 7665 2073 7468 2077 6974 6820  e have sth with 
-00004680: 7468 6520 6261 7365 2062 6174 6368 2077  the base batch w
-00004690: 6974 686f 7574 2062 6561 6d20 6f72 2070  ithout beam or p
-000046a0: 6164 6465 6420 6261 7463 6820 7768 6963  added batch whic
-000046b0: 6820 7765 2063 616e 2065 7874 656e 642e  h we can extend.
-000046c0: 0a20 2020 2020 2020 2069 6620 6261 7463  .        if batc
-000046d0: 6820 213d 2062 6174 6368 2e67 6574 5f67  h != batch.get_g
-000046e0: 6c6f 6261 6c5f 6261 7365 2829 3a0a 2020  lobal_base():.  
-000046f0: 2020 2020 2020 2020 2020 6261 7463 685f            batch_
-00004700: 6261 7365 203d 2062 6174 6368 2e67 6574  base = batch.get
-00004710: 5f67 6c6f 6261 6c5f 6261 7365 2829 0a20  _global_base(). 
-00004720: 2020 2020 2020 2020 2020 2062 6173 655f             base_
-00004730: 6361 6e5f 7573 655f 696e 5f63 7478 203d  can_use_in_ctx =
-00004740: 204e 6f6e 6520 2023 2074 7970 653a 204f   None  # type: O
-00004750: 7074 696f 6e61 6c5b 5f64 2e44 696d 5d0a  ptional[_d.Dim].
-00004760: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
-00004770: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
-00004780: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
-00004790: 2020 2020 2020 2020 2069 6620 7361 6d65           if same
-000047a0: 5f62 6173 652e 6261 7463 6820 3d3d 2062  _base.batch == b
-000047b0: 6174 6368 5f62 6173 6520 616e 6420 7361  atch_base and sa
-000047c0: 6d65 5f62 6173 652e 5f63 616e 5f75 7365  me_base._can_use
-000047d0: 5f69 6e5f 6374 7828 6374 7829 2061 6e64  _in_ctx(ctx) and
-000047e0: 2073 616d 655f 6261 7365 2e64 796e 5f73   same_base.dyn_s
-000047f0: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
-00004800: 2020 2020 2020 2020 2062 6173 655f 6361           base_ca
-00004810: 6e5f 7573 655f 696e 5f63 7478 203d 2073  n_use_in_ctx = s
-00004820: 616d 655f 6261 7365 0a20 2020 2020 2020  ame_base.       
-00004830: 2020 2020 2065 6c69 6620 7361 6d65 5f62       elif same_b
-00004840: 6173 652e 5f65 7874 7261 3a0a 2020 2020  ase._extra:.    
-00004850: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
-00004860: 2072 6574 7572 6e6e 2e74 662e 7574 696c   returnn.tf.util
-00004870: 2e64 6174 6120 696d 706f 7274 2043 6f6e  .data import Con
-00004880: 7472 6f6c 466c 6f77 436f 6e74 6578 740a  trolFlowContext.
-00004890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000048a0: 2066 6f72 2063 7478 5f20 696e 2043 6f6e   for ctx_ in Con
-000048b0: 7472 6f6c 466c 6f77 436f 6e74 6578 742e  trolFlowContext.
-000048c0: 6162 735f 6374 785f 7374 6163 6b5f 7769  abs_ctx_stack_wi
-000048d0: 7468 5f72 6f6f 7428 6374 7829 3a0a 2020  th_root(ctx):.  
-000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048f0: 2020 2320 6e6f 696e 7370 6563 7469 6f6e    # noinspection
-00004900: 2050 7950 726f 7465 6374 6564 4d65 6d62   PyProtectedMemb
-00004910: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-00004920: 2020 2020 2020 2074 6167 203d 2073 616d         tag = sam
-00004930: 655f 6261 7365 2e5f 6578 7472 612e 7361  e_base._extra.sa
-00004940: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
-00004950: 2e67 6574 2828 6261 7463 685f 6261 7365  .get((batch_base
-00004960: 2c20 6374 785f 292c 204e 6f6e 6529 0a20  , ctx_), None). 
-00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 2020 2069 6620 7461 6720 616e 6420 7461     if tag and ta
-00004990: 672e 5f63 616e 5f75 7365 5f69 6e5f 6374  g._can_use_in_ct
-000049a0: 7828 6374 7829 2061 6e64 2074 6167 2e5f  x(ctx) and tag._
-000049b0: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-000049c0: 656e 745f 6772 6170 6828 2920 616e 6420  ent_graph() and 
-000049d0: 7461 672e 6479 6e5f 7369 7a65 5f65 7874  tag.dyn_size_ext
-000049e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000049f0: 2020 2020 2020 2020 2020 6261 7365 5f63            base_c
-00004a00: 616e 5f75 7365 5f69 6e5f 6374 7820 3d20  an_use_in_ctx = 
-00004a10: 7461 670a 2020 2020 2020 2020 2020 2020  tag.            
-00004a20: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00004a30: 6b0a 2020 2020 2020 2020 2020 2020 6966  k.            if
-00004a40: 2062 6173 655f 6361 6e5f 7573 655f 696e   base_can_use_in
-00004a50: 5f63 7478 2061 6e64 2062 6173 655f 6361  _ctx and base_ca
-00004a60: 6e5f 7573 655f 696e 5f63 7478 2e64 796e  n_use_in_ctx.dyn
-00004a70: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-00004a80: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
-00004a90: 7365 5f63 616e 5f75 7365 5f69 6e5f 6374  se_can_use_in_ct
-00004aa0: 782e 6479 6e5f 7369 7a65 5f65 7874 2e68  x.dyn_size_ext.h
-00004ab0: 6176 655f 6261 7463 685f 6178 6973 2829  ave_batch_axis()
-00004ac0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004ad0: 2020 2020 2020 2320 5468 6520 7361 6d65        # The same
-00004ae0: 5f62 6173 6520 6861 7320 736f 6d65 2064  _base has some d
-00004af0: 796e 2073 697a 6520 7769 7468 6f75 7420  yn size without 
-00004b00: 616e 7920 6265 616d 206e 6f72 2063 6f6e  any beam nor con
-00004b10: 7472 6f6c 2066 6c6f 7720 636f 6e74 6578  trol flow contex
-00004b20: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
-00004b30: 2020 2020 2020 2023 2057 6520 6361 6e20         # We can 
-00004b40: 6578 7061 6e64 2069 7420 746f 2074 6865  expand it to the
-00004b50: 2063 7572 7265 6e74 2062 6561 6d2c 206f   current beam, o
-00004b60: 7220 6578 7465 6e64 2062 7920 7061 6464  r extend by padd
-00004b70: 6564 2062 6174 6368 2e0a 2020 2020 2020  ed batch..      
-00004b80: 2020 2020 2020 2020 2020 2020 2020 6479                dy
-00004b90: 6e5f 7369 7a65 5f65 7874 203d 2062 6173  n_size_ext = bas
-00004ba0: 655f 6361 6e5f 7573 655f 696e 5f63 7478  e_can_use_in_ctx
-00004bb0: 2e64 796e 5f73 697a 655f 6578 742e 636f  .dyn_size_ext.co
-00004bc0: 7079 5f65 7874 656e 645f 6261 7463 6828  py_extend_batch(
-00004bd0: 6261 7463 6829 0a20 2020 2020 2020 2020  batch).         
-00004be0: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
-00004bf0: 7463 682e 6265 616d 3a0a 2020 2020 2020  tch.beam:.      
-00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c10: 2020 6479 6e5f 7369 7a65 5f65 7874 203d    dyn_size_ext =
-00004c20: 2062 6173 655f 6361 6e5f 7573 655f 696e   base_can_use_in
-00004c30: 5f63 7478 2e64 796e 5f73 697a 655f 6578  _ctx.dyn_size_ex
-00004c40: 742e 636f 7079 5f65 7874 656e 645f 7769  t.copy_extend_wi
-00004c50: 7468 5f62 6561 6d28 6261 7463 682e 6265  th_beam(batch.be
-00004c60: 616d 290a 2020 2020 2020 2020 2020 2020  am).            
-00004c70: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-00004c80: 796e 5f73 697a 655f 6578 742e 6261 7463  yn_size_ext.batc
-00004c90: 6820 3d3d 2062 6174 6368 0a20 2020 2020  h == batch.     
-00004ca0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004cb0: 6620 6479 6e5f 7369 7a65 5f65 7874 2e70  f dyn_size_ext.p
-00004cc0: 6c61 6365 686f 6c64 6572 2069 7320 6e6f  laceholder is no
-00004cd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cf0: 6265 616d 5f65 7870 616e 6465 645f 6261  beam_expanded_ba
-00004d00: 7365 5f64 6174 6120 3d20 6765 7461 7474  se_data = getatt
-00004d10: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004d30: 796e 5f73 697a 655f 6578 742e 706c 6163  yn_size_ext.plac
-00004d40: 6568 6f6c 6465 722c 2022 5f52 4554 5552  eholder, "_RETUR
-00004d50: 4e4e 5f62 6561 6d5f 6578 7061 6e64 6564  NN_beam_expanded
-00004d60: 5f62 6173 655f 6461 7461 222c 204e 6f6e  _base_data", Non
-00004d70: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00004d80: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00003d60: 2020 2020 2020 2069 6620 6261 7463 682e         if batch.
+00003d70: 6973 5f67 6c6f 6261 6c5f 6261 7463 6828  is_global_batch(
+00003d80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00003d90: 2020 2072 6574 7572 6e20 5f64 2e62 6174     return _d.bat
+00003da0: 6368 5f64 696d 2020 2320 7265 7573 6520  ch_dim  # reuse 
+00003db0: 676c 6f62 616c 2062 6174 6368 2064 696d  global batch dim
+00003dc0: 2069 6620 706f 7373 6962 6c65 0a20 2020   if possible.   
+00003dd0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003de0: 5f64 2e44 696d 286b 696e 643d 4469 6d54  _d.Dim(kind=DimT
+00003df0: 7970 6573 2e42 6174 6368 2c20 6465 7363  ypes.Batch, desc
+00003e00: 7269 7074 696f 6e3d 2262 6174 6368 3a25  ription="batch:%
+00003e10: 7322 2025 2062 6174 6368 2e73 686f 7274  s" % batch.short
+00003e20: 5f72 6570 7228 292c 2062 6174 6368 3d62  _repr(), batch=b
+00003e30: 6174 6368 2c20 6469 6d65 6e73 696f 6e3d  atch, dimension=
+00003e40: 4e6f 6e65 290a 2020 2020 2020 2020 6966  None).        if
+00003e50: 206e 6f74 2073 656c 662e 6973 5f64 796e   not self.is_dyn
+00003e60: 616d 6963 2829 3a0a 2020 2020 2020 2020  amic():.        
+00003e70: 2020 2020 2320 4966 2073 7461 7469 6320      # If static 
+00003e80: 6469 6d2c 206e 6f20 6566 6665 6374 2e0a  dim, no effect..
+00003e90: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00003ea0: 7274 206e 6f74 2073 656c 662e 6261 7463  rt not self.batc
+00003eb0: 680a 2020 2020 2020 2020 2020 2020 7265  h.            re
+00003ec0: 7475 726e 2073 656c 660a 2020 2020 2020  turn self.      
+00003ed0: 2020 6966 2062 6174 6368 2e69 735f 6272    if batch.is_br
+00003ee0: 6f61 6463 6173 7428 293a 0a20 2020 2020  oadcast():.     
+00003ef0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00003f00: 6c66 2020 2320 6a75 7374 206c 6561 7665  lf  # just leave
+00003f10: 2061 732d 6973 2e20 7368 6f75 6c64 206e   as-is. should n
+00003f20: 6f74 206d 6174 7465 722e 0a20 2020 2020  ot matter..     
+00003f30: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
+00003f40: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
+00003f50: 616d 655f 6261 7365 203d 2073 656c 662e  ame_base = self.
+00003f60: 6765 745f 7361 6d65 5f62 6173 6528 290a  get_same_base().
+00003f70: 2020 2020 2020 2020 2020 2020 7361 6d65              same
+00003f80: 5f62 6173 652e 5f76 616c 6964 6174 655f  _base._validate_
+00003f90: 696e 5f63 7572 7265 6e74 5f67 7261 7068  in_current_graph
+00003fa0: 2829 0a20 2020 2020 2020 2020 2020 2023  ().            #
+00003fb0: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
+00003fc0: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
+00003fd0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00003fe0: 616d 655f 6261 7365 2e5f 6578 7472 613a  ame_base._extra:
+00003ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004000: 2066 726f 6d20 7265 7475 726e 6e2e 7466   from returnn.tf
+00004010: 2e75 7469 6c2e 6461 7461 2069 6d70 6f72  .util.data impor
+00004020: 7420 436f 6e74 726f 6c46 6c6f 7743 6f6e  t ControlFlowCon
+00004030: 7465 7874 0a0a 2020 2020 2020 2020 2020  text..          
+00004040: 2020 2020 2020 666f 7220 6374 785f 2069        for ctx_ i
+00004050: 6e20 436f 6e74 726f 6c46 6c6f 7743 6f6e  n ControlFlowCon
+00004060: 7465 7874 2e61 6273 5f63 7478 5f73 7461  text.abs_ctx_sta
+00004070: 636b 5f77 6974 685f 726f 6f74 2863 7478  ck_with_root(ctx
+00004080: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00004090: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
+000040a0: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
+000040b0: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
+000040c0: 2020 2020 2020 2020 2020 2020 7461 6720              tag 
+000040d0: 3d20 7361 6d65 5f62 6173 652e 5f65 7874  = same_base._ext
+000040e0: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
+000040f0: 685f 6374 782e 6765 7428 2862 6174 6368  h_ctx.get((batch
+00004100: 2c20 6374 785f 292c 204e 6f6e 6529 0a20  , ctx_), None). 
+00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004120: 2020 2069 6620 7461 6720 616e 6420 7461     if tag and ta
+00004130: 672e 5f63 616e 5f75 7365 5f69 6e5f 6374  g._can_use_in_ct
+00004140: 7828 6374 7829 2061 6e64 2074 6167 2e5f  x(ctx) and tag._
+00004150: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
+00004160: 656e 745f 6772 6170 6828 293a 0a20 2020  ent_graph():.   
+00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004180: 2020 2020 2061 7373 6572 7420 280a 2020       assert (.  
+00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041a0: 2020 2020 2020 2020 2020 7461 672e 6261            tag.ba
+000041b0: 7463 6820 3d3d 2062 6174 6368 0a20 2020  tch == batch.   
+000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041d0: 2020 2020 2029 2020 2320 736f 6d65 2063       )  # some c
+000041e0: 6f64 6520 7570 6461 7465 6420 6261 7463  ode updated batc
+000041f0: 6820 6469 7265 6374 6c79 2028 696e 636f  h directly (inco
+00004200: 7272 6563 746c 7929 2061 6e64 2063 6f75  rrectly) and cou
+00004210: 6c64 2074 7269 6767 6572 2074 6869 730a  ld trigger this.
+00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004230: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00004240: 6167 0a20 2020 2020 2020 2020 2020 2069  ag.            i
+00004250: 6620 7361 6d65 5f62 6173 652e 6261 7463  f same_base.batc
+00004260: 6820 3d3d 2062 6174 6368 2061 6e64 2073  h == batch and s
+00004270: 616d 655f 6261 7365 2e5f 6361 6e5f 7573  ame_base._can_us
+00004280: 655f 696e 5f63 7478 2863 7478 2920 616e  e_in_ctx(ctx) an
+00004290: 6420 7361 6d65 5f62 6173 652e 6479 6e5f  d same_base.dyn_
+000042a0: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
+000042b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000042c0: 2073 616d 655f 6261 7365 0a20 2020 2020   same_base.     
+000042d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000042e0: 2020 2020 2073 616d 655f 6261 7365 203d       same_base =
+000042f0: 2073 656c 660a 2020 2020 2020 2020 7361   self.        sa
+00004300: 6d65 5f62 6173 655f 6578 7472 6120 3d20  me_base_extra = 
+00004310: 7361 6d65 5f62 6173 652e 5f6d 616b 655f  same_base._make_
+00004320: 6578 7472 6128 290a 2020 2020 2020 2020  extra().        
+00004330: 2320 4f6b 2c20 6e6f 7468 696e 6720 6d61  # Ok, nothing ma
+00004340: 7463 6869 6e67 2066 6f75 6e64 2e0a 2020  tching found..  
+00004350: 2020 2020 2020 6966 2063 7478 3a0a 2020        if ctx:.  
+00004360: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
+00004370: 6b20 6966 2074 6865 2063 7478 2069 7320  k if the ctx is 
+00004380: 7265 616c 6c79 2072 656c 6576 616e 742c  really relevant,
+00004390: 2077 6865 6e20 7468 6973 2069 7320 6465   when this is de
+000043a0: 7269 7665 6420 6672 6f6d 206f 7468 6572  rived from other
+000043b0: 2074 6167 732e 0a20 2020 2020 2020 2020   tags..         
+000043c0: 2020 2064 6572 6976 6564 5f62 6173 6573     derived_bases
+000043d0: 203d 2073 616d 655f 6261 7365 2e67 6574   = same_base.get
+000043e0: 5f64 6572 6976 6564 5f62 6173 6573 5f73  _derived_bases_s
+000043f0: 6574 2829 0a20 2020 2020 2020 2020 2020  et().           
+00004400: 2064 6572 6976 6564 5f62 6173 6573 2e72   derived_bases.r
+00004410: 656d 6f76 6528 7361 6d65 5f62 6173 6529  emove(same_base)
+00004420: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004430: 6465 7269 7665 645f 6261 7365 733a 0a20  derived_bases:. 
+00004440: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00004450: 6572 6976 6564 5f63 7478 7320 3d20 7365  erived_ctxs = se
+00004460: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00004470: 2020 2020 666f 7220 6420 696e 2064 6572      for d in der
+00004480: 6976 6564 5f62 6173 6573 3a0a 2020 2020  ived_bases:.    
+00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044a0: 7769 7468 2075 7469 6c2e 6775 6172 645f  with util.guard_
+000044b0: 696e 6669 6e69 7465 5f72 6563 7572 7369  infinite_recursi
+000044c0: 6f6e 285f 642e 4469 6d2e 6765 745f 666f  on(_d.Dim.get_fo
+000044d0: 725f 6261 7463 685f 6374 782c 2064 293a  r_batch_ctx, d):
+000044e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000044f0: 2020 2020 2020 2020 2064 203d 2064 2e67           d = d.g
+00004500: 6574 5f66 6f72 5f62 6174 6368 5f63 7478  et_for_batch_ctx
+00004510: 2862 6174 6368 3d62 6174 6368 2c20 6374  (batch=batch, ct
+00004520: 783d 6374 7829 0a20 2020 2020 2020 2020  x=ctx).         
+00004530: 2020 2020 2020 2020 2020 2069 6620 642e             if d.
+00004540: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+00004550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004560: 2020 2020 2020 2020 2020 6465 7269 7665            derive
+00004570: 645f 6374 7873 2e61 6464 2864 2e63 6f6e  d_ctxs.add(d.con
+00004580: 7472 6f6c 5f66 6c6f 775f 6374 7829 0a20  trol_flow_ctx). 
+00004590: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000045a0: 6620 6e6f 7420 6465 7269 7665 645f 6374  f not derived_ct
+000045b0: 7873 3a0a 2020 2020 2020 2020 2020 2020  xs:.            
+000045c0: 2020 2020 2020 2020 6374 7820 3d20 4e6f          ctx = No
+000045d0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+000045e0: 2020 2065 6c69 6620 6c65 6e28 6465 7269     elif len(deri
+000045f0: 7665 645f 6374 7873 2920 3d3d 2031 3a0a  ved_ctxs) == 1:.
+00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004610: 2020 2020 6374 7820 3d20 6465 7269 7665      ctx = derive
+00004620: 645f 6374 7873 2e70 6f70 2829 0a20 2020  d_ctxs.pop().   
+00004630: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00004640: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00004650: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00004660: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00004670: 2822 6e6f 7420 7965 7420 696d 706c 656d  ("not yet implem
+00004680: 656e 7465 643a 206d 756c 7469 706c 6520  ented: multiple 
+00004690: 6465 7269 7665 6420 6374 7873 3a20 2572  derived ctxs: %r
+000046a0: 2220 2520 2864 6572 6976 6564 5f63 7478  " % (derived_ctx
+000046b0: 732c 2929 0a20 2020 2020 2020 2064 796e  s,)).        dyn
+000046c0: 5f73 697a 655f 6578 7420 3d20 4e6f 6e65  _size_ext = None
+000046d0: 0a20 2020 2020 2020 2023 204d 6179 6265  .        # Maybe
+000046e0: 2077 6520 6861 7665 2073 7468 2077 6974   we have sth wit
+000046f0: 6820 7468 6520 6261 7365 2062 6174 6368  h the base batch
+00004700: 2077 6974 686f 7574 2062 6561 6d20 6f72   without beam or
+00004710: 2070 6164 6465 6420 6261 7463 6820 7768   padded batch wh
+00004720: 6963 6820 7765 2063 616e 2065 7874 656e  ich we can exten
+00004730: 642e 0a20 2020 2020 2020 2069 6620 6261  d..        if ba
+00004740: 7463 6820 213d 2062 6174 6368 2e67 6574  tch != batch.get
+00004750: 5f67 6c6f 6261 6c5f 6261 7365 2829 3a0a  _global_base():.
+00004760: 2020 2020 2020 2020 2020 2020 6261 7463              batc
+00004770: 685f 6261 7365 203d 2062 6174 6368 2e67  h_base = batch.g
+00004780: 6574 5f67 6c6f 6261 6c5f 6261 7365 2829  et_global_base()
+00004790: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+000047a0: 655f 6361 6e5f 7573 655f 696e 5f63 7478  e_can_use_in_ctx
+000047b0: 203d 204e 6f6e 6520 2023 2074 7970 653a   = None  # type:
+000047c0: 204f 7074 696f 6e61 6c5b 5f64 2e44 696d   Optional[_d.Dim
+000047d0: 5d0a 2020 2020 2020 2020 2020 2020 2320  ].            # 
+000047e0: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
+000047f0: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
+00004800: 2020 2020 2020 2020 2020 2069 6620 7361             if sa
+00004810: 6d65 5f62 6173 652e 6261 7463 6820 3d3d  me_base.batch ==
+00004820: 2062 6174 6368 5f62 6173 6520 616e 6420   batch_base and 
+00004830: 7361 6d65 5f62 6173 652e 5f63 616e 5f75  same_base._can_u
+00004840: 7365 5f69 6e5f 6374 7828 6374 7829 2061  se_in_ctx(ctx) a
+00004850: 6e64 2073 616d 655f 6261 7365 2e64 796e  nd same_base.dyn
+00004860: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
+00004870: 2020 2020 2020 2020 2020 2062 6173 655f             base_
+00004880: 6361 6e5f 7573 655f 696e 5f63 7478 203d  can_use_in_ctx =
+00004890: 2073 616d 655f 6261 7365 0a20 2020 2020   same_base.     
+000048a0: 2020 2020 2020 2065 6c69 6620 7361 6d65         elif same
+000048b0: 5f62 6173 652e 5f65 7874 7261 3a0a 2020  _base._extra:.  
+000048c0: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+000048d0: 6f6d 2072 6574 7572 6e6e 2e74 662e 7574  om returnn.tf.ut
+000048e0: 696c 2e64 6174 6120 696d 706f 7274 2043  il.data import C
+000048f0: 6f6e 7472 6f6c 466c 6f77 436f 6e74 6578  ontrolFlowContex
+00004900: 740a 0a20 2020 2020 2020 2020 2020 2020  t..             
+00004910: 2020 2066 6f72 2063 7478 5f20 696e 2043     for ctx_ in C
+00004920: 6f6e 7472 6f6c 466c 6f77 436f 6e74 6578  ontrolFlowContex
+00004930: 742e 6162 735f 6374 785f 7374 6163 6b5f  t.abs_ctx_stack_
+00004940: 7769 7468 5f72 6f6f 7428 6374 7829 3a0a  with_root(ctx):.
+00004950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004960: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+00004970: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+00004980: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+00004990: 2020 2020 2020 2020 2074 6167 203d 2073           tag = s
+000049a0: 616d 655f 6261 7365 2e5f 6578 7472 612e  ame_base._extra.
+000049b0: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
+000049c0: 7478 2e67 6574 2828 6261 7463 685f 6261  tx.get((batch_ba
+000049d0: 7365 2c20 6374 785f 292c 204e 6f6e 6529  se, ctx_), None)
+000049e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000049f0: 2020 2020 2069 6620 7461 6720 616e 6420       if tag and 
+00004a00: 7461 672e 5f63 616e 5f75 7365 5f69 6e5f  tag._can_use_in_
+00004a10: 6374 7828 6374 7829 2061 6e64 2074 6167  ctx(ctx) and tag
+00004a20: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+00004a30: 7272 656e 745f 6772 6170 6828 2920 616e  rrent_graph() an
+00004a40: 6420 7461 672e 6479 6e5f 7369 7a65 5f65  d tag.dyn_size_e
+00004a50: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+00004a60: 2020 2020 2020 2020 2020 2020 6261 7365              base
+00004a70: 5f63 616e 5f75 7365 5f69 6e5f 6374 7820  _can_use_in_ctx 
+00004a80: 3d20 7461 670a 2020 2020 2020 2020 2020  = tag.          
+00004a90: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00004aa0: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00004ab0: 6966 2062 6173 655f 6361 6e5f 7573 655f  if base_can_use_
+00004ac0: 696e 5f63 7478 2061 6e64 2062 6173 655f  in_ctx and base_
+00004ad0: 6361 6e5f 7573 655f 696e 5f63 7478 2e64  can_use_in_ctx.d
+00004ae0: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
+00004af0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004b00: 6261 7365 5f63 616e 5f75 7365 5f69 6e5f  base_can_use_in_
+00004b10: 6374 782e 6479 6e5f 7369 7a65 5f65 7874  ctx.dyn_size_ext
+00004b20: 2e68 6176 655f 6261 7463 685f 6178 6973  .have_batch_axis
+00004b30: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00004b40: 2020 2020 2020 2020 2320 5468 6520 7361          # The sa
+00004b50: 6d65 5f62 6173 6520 6861 7320 736f 6d65  me_base has some
+00004b60: 2064 796e 2073 697a 6520 7769 7468 6f75   dyn size withou
+00004b70: 7420 616e 7920 6265 616d 206e 6f72 2063  t any beam nor c
+00004b80: 6f6e 7472 6f6c 2066 6c6f 7720 636f 6e74  ontrol flow cont
+00004b90: 6578 742e 0a20 2020 2020 2020 2020 2020  ext..           
+00004ba0: 2020 2020 2020 2020 2023 2057 6520 6361           # We ca
+00004bb0: 6e20 6578 7061 6e64 2069 7420 746f 2074  n expand it to t
+00004bc0: 6865 2063 7572 7265 6e74 2062 6561 6d2c  he current beam,
+00004bd0: 206f 7220 6578 7465 6e64 2062 7920 7061   or extend by pa
+00004be0: 6464 6564 2062 6174 6368 2e0a 2020 2020  dded batch..    
+00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c00: 6479 6e5f 7369 7a65 5f65 7874 203d 2062  dyn_size_ext = b
+00004c10: 6173 655f 6361 6e5f 7573 655f 696e 5f63  ase_can_use_in_c
+00004c20: 7478 2e64 796e 5f73 697a 655f 6578 742e  tx.dyn_size_ext.
+00004c30: 636f 7079 5f65 7874 656e 645f 6261 7463  copy_extend_batc
+00004c40: 6828 6261 7463 6829 0a20 2020 2020 2020  h(batch).       
+00004c50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004c60: 6261 7463 682e 6265 616d 3a0a 2020 2020  batch.beam:.    
+00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c80: 2020 2020 6479 6e5f 7369 7a65 5f65 7874      dyn_size_ext
+00004c90: 203d 2062 6173 655f 6361 6e5f 7573 655f   = base_can_use_
+00004ca0: 696e 5f63 7478 2e64 796e 5f73 697a 655f  in_ctx.dyn_size_
+00004cb0: 6578 742e 636f 7079 5f65 7874 656e 645f  ext.copy_extend_
+00004cc0: 7769 7468 5f62 6561 6d28 6261 7463 682e  with_beam(batch.
+00004cd0: 6265 616d 290a 2020 2020 2020 2020 2020  beam).          
+00004ce0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00004cf0: 2064 796e 5f73 697a 655f 6578 742e 6261   dyn_size_ext.ba
+00004d00: 7463 6820 3d3d 2062 6174 6368 0a20 2020  tch == batch.   
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2069 6620 6479 6e5f 7369 7a65 5f65 7874   if dyn_size_ext
+00004d30: 2e70 6c61 6365 686f 6c64 6572 2069 7320  .placeholder is 
+00004d40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d60: 2020 6265 616d 5f65 7870 616e 6465 645f    beam_expanded_
+00004d70: 6261 7365 5f64 6174 6120 3d20 6765 7461  base_data = geta
+00004d80: 7474 7228 0a20 2020 2020 2020 2020 2020  ttr(.           
 00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004da0: 2020 2020 6966 2062 6174 6368 2e62 6561      if batch.bea
-00004db0: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
-00004dc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00004dd0: 7373 6572 7420 6265 616d 5f65 7870 616e  ssert beam_expan
-00004de0: 6465 645f 6261 7365 5f64 6174 610a 2020  ded_base_data.  
-00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e00: 2020 2020 2020 2320 4e6f 7465 3a20 5468        # Note: Th
-00004e10: 6520 6265 616d 2065 7870 616e 7369 6f6e  e beam expansion
-00004e20: 2075 7365 6420 7469 6c69 6e67 2c20 7768   used tiling, wh
-00004e30: 6963 6820 6361 6e20 6265 2063 6163 6865  ich can be cache
-00004e40: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
-00004e50: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
-00004e60: 7320 6d65 616e 7320 7468 6174 2077 6520  s means that we 
-00004e70: 636f 756c 6420 656e 6420 7570 2077 6974  could end up wit
-00004e80: 6820 7468 6520 7361 6d65 2073 697a 6520  h the same size 
-00004e90: 7465 6e73 6f72 2028 706c 6163 6568 6f6c  tensor (placehol
-00004ea0: 6465 7229 0a20 2020 2020 2020 2020 2020  der).           
-00004eb0: 2020 2020 2020 2020 2020 2020 2023 2066               # f
-00004ec0: 6f72 206d 756c 7469 706c 6520 6469 6666  or multiple diff
-00004ed0: 6572 656e 7420 6265 616d 732c 0a20 2020  erent beams,.   
-00004ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ef0: 2020 2020 2023 2077 6865 6e20 7468 6572       # when ther
-00004f00: 6520 6172 6520 6469 6666 6572 656e 7420  e are different 
-00004f10: 6265 616d 7320 7769 7468 2073 616d 6520  beams with same 
-00004f20: 6265 616d 2073 697a 6521 0a20 2020 2020  beam size!.     
-00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f40: 2020 2023 2054 6869 7320 6272 6561 6b73     # This breaks
-00004f50: 2074 6865 2063 7572 7265 6e74 206c 6f67   the current log
-00004f60: 6963 2069 6e20 6765 745f 7461 675f 6672  ic in get_tag_fr
-00004f70: 6f6d 5f73 697a 655f 7465 6e73 6f72 2e0a  om_size_tensor..
-00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f90: 2020 2020 2020 2020 2320 4173 2061 2077          # As a w
-00004fa0: 6f72 6b61 726f 756e 642c 2077 6520 6d61  orkaround, we ma
-00004fb0: 6b65 2061 6e20 6578 706c 6963 6974 206e  ke an explicit n
-00004fc0: 6577 2074 656e 736f 7220 6865 7265 2e0a  ew tensor here..
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 2020 2020 2020 2020 696d 706f 7274 2074          import t
-00004ff0: 656e 736f 7266 6c6f 7720 6173 2074 660a  ensorflow as tf.
-00005000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005010: 2020 2020 2020 2020 6672 6f6d 2072 6574          from ret
-00005020: 7572 6e6e 2e74 662e 7574 696c 2e62 6173  urnn.tf.util.bas
-00005030: 6963 2069 6d70 6f72 7420 6765 745f 7661  ic import get_va
-00005040: 6c69 645f 7363 6f70 655f 6e61 6d65 5f66  lid_scope_name_f
-00005050: 726f 6d5f 7374 722c 2073 616d 655f 636f  rom_str, same_co
-00005060: 6e74 726f 6c5f 666c 6f77 5f63 7478 0a0a  ntrol_flow_ctx..
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 2020 2020 2020 2020 7769 7468 2073 616d          with sam
-00005090: 655f 636f 6e74 726f 6c5f 666c 6f77 5f63  e_control_flow_c
-000050a0: 7478 2864 796e 5f73 697a 655f 6578 742e  tx(dyn_size_ext.
-000050b0: 706c 6163 6568 6f6c 6465 7229 3a0a 2020  placeholder):.  
-000050c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050d0: 2020 2020 2020 2020 2020 6479 6e5f 7369            dyn_si
-000050e0: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
-000050f0: 6572 203d 2074 662e 6964 656e 7469 7479  er = tf.identity
-00005100: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005120: 2020 6479 6e5f 7369 7a65 5f65 7874 2e70    dyn_size_ext.p
-00005130: 6c61 6365 686f 6c64 6572 2c0a 2020 2020  laceholder,.    
-00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005150: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00005160: 3d67 6574 5f76 616c 6964 5f73 636f 7065  =get_valid_scope
-00005170: 5f6e 616d 655f 6672 6f6d 5f73 7472 280a  _name_from_str(.
+00004da0: 2064 796e 5f73 697a 655f 6578 742e 706c   dyn_size_ext.pl
+00004db0: 6163 6568 6f6c 6465 722c 2022 5f52 4554  aceholder, "_RET
+00004dc0: 5552 4e4e 5f62 6561 6d5f 6578 7061 6e64  URNN_beam_expand
+00004dd0: 6564 5f62 6173 655f 6461 7461 222c 204e  ed_base_data", N
+00004de0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00004df0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e10: 2020 2020 2020 6966 2062 6174 6368 2e62        if batch.b
+00004e20: 6561 6d3a 0a20 2020 2020 2020 2020 2020  eam:.           
+00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e40: 2061 7373 6572 7420 6265 616d 5f65 7870   assert beam_exp
+00004e50: 616e 6465 645f 6261 7365 5f64 6174 610a  anded_base_data.
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 2020 2020 2020 2020 2320 4e6f 7465 3a20          # Note: 
+00004e80: 5468 6520 6265 616d 2065 7870 616e 7369  The beam expansi
+00004e90: 6f6e 2075 7365 6420 7469 6c69 6e67 2c20  on used tiling, 
+00004ea0: 7768 6963 6820 6361 6e20 6265 2063 6163  which can be cac
+00004eb0: 6865 642e 0a20 2020 2020 2020 2020 2020  hed..           
+00004ec0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
+00004ed0: 6869 7320 6d65 616e 7320 7468 6174 2077  his means that w
+00004ee0: 6520 636f 756c 6420 656e 6420 7570 2077  e could end up w
+00004ef0: 6974 6820 7468 6520 7361 6d65 2073 697a  ith the same siz
+00004f00: 6520 7465 6e73 6f72 2028 706c 6163 6568  e tensor (placeh
+00004f10: 6f6c 6465 7229 0a20 2020 2020 2020 2020  older).         
+00004f20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00004f30: 2066 6f72 206d 756c 7469 706c 6520 6469   for multiple di
+00004f40: 6666 6572 656e 7420 6265 616d 732c 0a20  fferent beams,. 
+00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f60: 2020 2020 2020 2023 2077 6865 6e20 7468         # when th
+00004f70: 6572 6520 6172 6520 6469 6666 6572 656e  ere are differen
+00004f80: 7420 6265 616d 7320 7769 7468 2073 616d  t beams with sam
+00004f90: 6520 6265 616d 2073 697a 6521 0a20 2020  e beam size!.   
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fb0: 2020 2020 2023 2054 6869 7320 6272 6561       # This brea
+00004fc0: 6b73 2074 6865 2063 7572 7265 6e74 206c  ks the current l
+00004fd0: 6f67 6963 2069 6e20 6765 745f 7461 675f  ogic in get_tag_
+00004fe0: 6672 6f6d 5f73 697a 655f 7465 6e73 6f72  from_size_tensor
+00004ff0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005000: 2020 2020 2020 2020 2020 2320 4173 2061            # As a
+00005010: 2077 6f72 6b61 726f 756e 642c 2077 6520   workaround, we 
+00005020: 6d61 6b65 2061 6e20 6578 706c 6963 6974  make an explicit
+00005030: 206e 6577 2074 656e 736f 7220 6865 7265   new tensor here
+00005040: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005050: 2020 2020 2020 2020 2020 696d 706f 7274            import
+00005060: 2074 656e 736f 7266 6c6f 7720 6173 2074   tensorflow as t
+00005070: 660a 2020 2020 2020 2020 2020 2020 2020  f.              
+00005080: 2020 2020 2020 2020 2020 6672 6f6d 2072            from r
+00005090: 6574 7572 6e6e 2e74 662e 7574 696c 2e62  eturnn.tf.util.b
+000050a0: 6173 6963 2069 6d70 6f72 7420 6765 745f  asic import get_
+000050b0: 7661 6c69 645f 7363 6f70 655f 6e61 6d65  valid_scope_name
+000050c0: 5f66 726f 6d5f 7374 722c 2073 616d 655f  _from_str, same_
+000050d0: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+000050e0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000050f0: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+00005100: 616d 655f 636f 6e74 726f 6c5f 666c 6f77  ame_control_flow
+00005110: 5f63 7478 2864 796e 5f73 697a 655f 6578  _ctx(dyn_size_ex
+00005120: 742e 706c 6163 6568 6f6c 6465 7229 3a0a  t.placeholder):.
+00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005140: 2020 2020 2020 2020 2020 2020 6479 6e5f              dyn_
+00005150: 7369 7a65 5f65 7874 2e70 6c61 6365 686f  size_ext.placeho
+00005160: 6c64 6572 203d 2074 662e 6964 656e 7469  lder = tf.identi
+00005170: 7479 280a 2020 2020 2020 2020 2020 2020  ty(.            
 00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2020 2020 2225 735f 6765 745f 666f 725f      "%s_get_for_
-000051b0: 6261 7463 685f 6374 785f 2573 2220 2520  batch_ctx_%s" % 
-000051c0: 2864 796e 5f73 697a 655f 6578 742e 6e61  (dyn_size_ext.na
-000051d0: 6d65 2c20 6261 7463 682e 7368 6f72 745f  me, batch.short_
-000051e0: 7265 7072 2829 290a 2020 2020 2020 2020  repr()).        
-000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005200: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005220: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005240: 2069 6620 6261 7463 682e 6265 616d 3a0a   if batch.beam:.
-00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005260: 2020 2020 2020 2020 2020 2020 6479 6e5f              dyn_
-00005270: 7369 7a65 5f65 7874 2e70 6c61 6365 686f  size_ext.placeho
-00005280: 6c64 6572 2e5f 5245 5455 524e 4e5f 6479  lder._RETURNN_dy
-00005290: 6e5f 7369 7a65 5f62 6561 6d20 3d20 6261  n_size_beam = ba
-000052a0: 7463 682e 6265 616d 0a20 2020 2020 2020  tch.beam.       
-000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052c0: 2020 2020 2064 796e 5f73 697a 655f 6578       dyn_size_ex
-000052d0: 742e 706c 6163 6568 6f6c 6465 722e 5f52  t.placeholder._R
-000052e0: 4554 5552 4e4e 5f62 6561 6d5f 6578 7061  ETURNN_beam_expa
-000052f0: 6e64 6564 5f62 6173 655f 6461 7461 203d  nded_base_data =
-00005300: 2062 6561 6d5f 6578 7061 6e64 6564 5f62   beam_expanded_b
-00005310: 6173 655f 6461 7461 0a20 2020 2020 2020  ase_data.       
-00005320: 2069 6620 6e6f 7420 6479 6e5f 7369 7a65   if not dyn_size
-00005330: 5f65 7874 2061 6e64 2061 6c6c 6f77 5f6e  _ext and allow_n
-00005340: 6f6e 6520 616e 6420 6e6f 7420 7361 6d65  one and not same
-00005350: 5f62 6173 652e 6465 7269 7665 645f 6672  _base.derived_fr
-00005360: 6f6d 5f6f 703a 0a20 2020 2020 2020 2020  om_op:.         
-00005370: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00005380: 2020 2020 2020 2069 6620 6e6f 7420 6479         if not dy
-00005390: 6e5f 7369 7a65 5f65 7874 2061 6e64 2073  n_size_ext and s
-000053a0: 616d 655f 6261 7365 5f65 7874 7261 2e73  ame_base_extra.s
-000053b0: 616d 655f 666f 725f 6261 7463 685f 6374  ame_for_batch_ct
-000053c0: 783a 0a20 2020 2020 2020 2020 2020 2023  x:.            #
-000053d0: 2054 6865 7265 2061 7265 2065 6172 6c69   There are earli
-000053e0: 6572 2065 6e74 7269 6573 2069 6e20 5f73  er entries in _s
-000053f0: 616d 655f 666f 725f 6261 7463 685f 6374  ame_for_batch_ct
-00005400: 780a 2020 2020 2020 2020 2020 2020 2320  x.            # 
-00005410: 2d2d 206d 6179 6265 2077 6520 6361 6e20  -- maybe we can 
-00005420: 696e 6665 7220 6479 6e5f 7369 7a65 5f65  infer dyn_size_e
-00005430: 7874 2c20 6576 656e 2077 6974 6820 6469  xt, even with di
-00005440: 6666 6572 656e 7420 6261 7463 682e 0a20  fferent batch.. 
-00005450: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-00005460: 6261 7463 685f 2c20 6374 785f 292c 206f  batch_, ctx_), o
-00005470: 7468 6572 2069 6e20 7361 6d65 5f62 6173  ther in same_bas
-00005480: 655f 6578 7472 612e 7361 6d65 5f66 6f72  e_extra.same_for
-00005490: 5f62 6174 6368 5f63 7478 2e69 7465 6d73  _batch_ctx.items
-000054a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000054b0: 2020 2020 6966 2063 7478 5f20 3d3d 2063      if ctx_ == c
-000054c0: 7478 2061 6e64 206f 7468 6572 2e64 796e  tx and other.dyn
-000054d0: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-000054e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000054f0: 796e 5f73 697a 655f 6578 7420 3d20 6f74  yn_size_ext = ot
-00005500: 6865 722e 6479 6e5f 7369 7a65 5f65 7874  her.dyn_size_ext
-00005510: 2e63 6f70 795f 7465 6d70 6c61 7465 2829  .copy_template()
-00005520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005530: 2020 2020 2064 796e 5f73 697a 655f 6578       dyn_size_ex
-00005540: 742e 6265 616d 203d 2062 6174 6368 2e62  t.beam = batch.b
-00005550: 6561 6d0a 2020 2020 2020 2020 2020 2020  eam.            
-00005560: 2020 2020 2020 2020 6479 6e5f 7369 7a65          dyn_size
-00005570: 5f65 7874 2e62 6174 6368 203d 2062 6174  _ext.batch = bat
-00005580: 6368 0a20 2020 2020 2020 2020 2020 2020  ch.             
-00005590: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-000055a0: 2020 2020 2063 7478 203d 2064 796e 5f73       ctx = dyn_s
-000055b0: 697a 655f 6578 742e 636f 6e74 726f 6c5f  ize_ext.control_
-000055c0: 666c 6f77 5f63 7478 2069 6620 6479 6e5f  flow_ctx if dyn_
-000055d0: 7369 7a65 5f65 7874 2065 6c73 6520 6374  size_ext else ct
-000055e0: 780a 2020 2020 2020 2020 6469 6d5f 7461  x.        dim_ta
-000055f0: 6720 3d20 4e6f 6e65 0a20 2020 2020 2020  g = None.       
-00005600: 2066 6f72 2063 616e 6469 6461 7465 2069   for candidate i
-00005610: 6e20 5b73 656c 662c 2073 616d 655f 6261  n [self, same_ba
-00005620: 7365 5d3a 0a20 2020 2020 2020 2020 2020  se]:.           
-00005630: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-00005640: 2020 2020 2020 2863 616e 6469 6461 7465        (candidate
-00005650: 2e62 6174 6368 203d 3d20 6261 7463 6820  .batch == batch 
-00005660: 6f72 2028 6e6f 7420 6361 6e64 6964 6174  or (not candidat
-00005670: 652e 6261 7463 6820 616e 6420 6261 7463  e.batch and batc
-00005680: 682e 6973 5f67 6c6f 6261 6c5f 6261 7463  h.is_global_batc
-00005690: 6828 2929 290a 2020 2020 2020 2020 2020  h())).          
-000056a0: 2020 2020 2020 616e 6420 6e6f 7420 6361        and not ca
-000056b0: 6e64 6964 6174 652e 636f 6e74 726f 6c5f  ndidate.control_
-000056c0: 666c 6f77 5f63 7478 0a20 2020 2020 2020  flow_ctx.       
-000056d0: 2020 2020 2020 2020 2061 6e64 206e 6f74           and not
-000056e0: 2063 7478 0a20 2020 2020 2020 2020 2020   ctx.           
-000056f0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00005700: 2020 2020 2320 5468 6520 7361 6d65 5f62      # The same_b
-00005710: 6173 6520 696e 7374 616e 6365 2069 7320  ase instance is 
-00005720: 6569 7468 6572 2075 6e64 6566 696e 6564  either undefined
-00005730: 2028 6e6f 2062 6174 6368 2c20 6e6f 2063   (no batch, no c
-00005740: 7478 290a 2020 2020 2020 2020 2020 2020  tx).            
-00005750: 2020 2020 2320 6f72 2069 7420 6973 2064      # or it is d
-00005760: 6566 696e 6564 2066 6f72 2074 6865 2073  efined for the s
-00005770: 616d 6520 6261 7463 6820 616e 6420 6374  ame batch and ct
-00005780: 782e 0a20 2020 2020 2020 2020 2020 2020  x..             
-00005790: 2020 2023 2049 6e20 616e 7920 6361 7365     # In any case
-000057a0: 2c20 7265 7573 6520 6974 2074 6865 6e2e  , reuse it then.
-000057b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057c0: 2063 616e 6469 6461 7465 2e62 6174 6368   candidate.batch
-000057d0: 203d 2062 6174 6368 0a20 2020 2020 2020   = batch.       
-000057e0: 2020 2020 2020 2020 2069 6620 6479 6e5f           if dyn_
-000057f0: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-00005800: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005810: 2063 616e 6469 6461 7465 2e64 796e 5f73   candidate.dyn_s
-00005820: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
-00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005840: 2063 616e 6469 6461 7465 2e64 796e 5f73   candidate.dyn_s
-00005850: 697a 655f 6578 742e 6261 7463 6820 3d20  ize_ext.batch = 
-00005860: 6261 7463 680a 2020 2020 2020 2020 2020  batch.          
-00005870: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00005880: 7365 7274 2063 616e 6469 6461 7465 2e64  sert candidate.d
-00005890: 796e 5f73 697a 655f 6578 742e 6469 6d5f  yn_size_ext.dim_
-000058a0: 7461 6773 203d 3d20 6479 6e5f 7369 7a65  tags == dyn_size
-000058b0: 5f65 7874 2e64 696d 5f74 6167 730a 2020  _ext.dim_tags.  
-000058c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00005190: 2020 2020 6479 6e5f 7369 7a65 5f65 7874      dyn_size_ext
+000051a0: 2e70 6c61 6365 686f 6c64 6572 2c0a 2020  .placeholder,.  
+000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051c0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+000051d0: 6d65 3d67 6574 5f76 616c 6964 5f73 636f  me=get_valid_sco
+000051e0: 7065 5f6e 616d 655f 6672 6f6d 5f73 7472  pe_name_from_str
+000051f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005210: 2020 2020 2020 2225 735f 6765 745f 666f        "%s_get_fo
+00005220: 725f 6261 7463 685f 6374 785f 2573 2220  r_batch_ctx_%s" 
+00005230: 2520 2864 796e 5f73 697a 655f 6578 742e  % (dyn_size_ext.
+00005240: 6e61 6d65 2c20 6261 7463 682e 7368 6f72  name, batch.shor
+00005250: 745f 7265 7072 2829 290a 2020 2020 2020  t_repr()).      
+00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005270: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052b0: 2020 2069 6620 6261 7463 682e 6265 616d     if batch.beam
+000052c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000052d0: 2020 2020 2020 2020 2020 2020 2020 6479                dy
+000052e0: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
+000052f0: 686f 6c64 6572 2e5f 5245 5455 524e 4e5f  holder._RETURNN_
+00005300: 6479 6e5f 7369 7a65 5f62 6561 6d20 3d20  dyn_size_beam = 
+00005310: 6261 7463 682e 6265 616d 0a20 2020 2020  batch.beam.     
+00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005330: 2020 2020 2020 2064 796e 5f73 697a 655f         dyn_size_
+00005340: 6578 742e 706c 6163 6568 6f6c 6465 722e  ext.placeholder.
+00005350: 5f52 4554 5552 4e4e 5f62 6561 6d5f 6578  _RETURNN_beam_ex
+00005360: 7061 6e64 6564 5f62 6173 655f 6461 7461  panded_base_data
+00005370: 203d 2062 6561 6d5f 6578 7061 6e64 6564   = beam_expanded
+00005380: 5f62 6173 655f 6461 7461 0a20 2020 2020  _base_data.     
+00005390: 2020 2069 6620 6e6f 7420 6479 6e5f 7369     if not dyn_si
+000053a0: 7a65 5f65 7874 2061 6e64 2061 6c6c 6f77  ze_ext and allow
+000053b0: 5f6e 6f6e 6520 616e 6420 6e6f 7420 7361  _none and not sa
+000053c0: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
+000053d0: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
+000053e0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000053f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00005400: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
+00005410: 2073 616d 655f 6261 7365 5f65 7874 7261   same_base_extra
+00005420: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
+00005430: 6374 783a 0a20 2020 2020 2020 2020 2020  ctx:.           
+00005440: 2023 2054 6865 7265 2061 7265 2065 6172   # There are ear
+00005450: 6c69 6572 2065 6e74 7269 6573 2069 6e20  lier entries in 
+00005460: 5f73 616d 655f 666f 725f 6261 7463 685f  _same_for_batch_
+00005470: 6374 780a 2020 2020 2020 2020 2020 2020  ctx.            
+00005480: 2320 2d2d 206d 6179 6265 2077 6520 6361  # -- maybe we ca
+00005490: 6e20 696e 6665 7220 6479 6e5f 7369 7a65  n infer dyn_size
+000054a0: 5f65 7874 2c20 6576 656e 2077 6974 6820  _ext, even with 
+000054b0: 6469 6666 6572 656e 7420 6261 7463 682e  different batch.
+000054c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000054d0: 2028 6261 7463 685f 2c20 6374 785f 292c   (batch_, ctx_),
+000054e0: 206f 7468 6572 2069 6e20 7361 6d65 5f62   other in same_b
+000054f0: 6173 655f 6578 7472 612e 7361 6d65 5f66  ase_extra.same_f
+00005500: 6f72 5f62 6174 6368 5f63 7478 2e69 7465  or_batch_ctx.ite
+00005510: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+00005520: 2020 2020 2020 6966 2063 7478 5f20 3d3d        if ctx_ ==
+00005530: 2063 7478 2061 6e64 206f 7468 6572 2e64   ctx and other.d
+00005540: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
+00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005560: 2064 796e 5f73 697a 655f 6578 7420 3d20   dyn_size_ext = 
+00005570: 6f74 6865 722e 6479 6e5f 7369 7a65 5f65  other.dyn_size_e
+00005580: 7874 2e63 6f70 795f 7465 6d70 6c61 7465  xt.copy_template
+00005590: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000055a0: 2020 2020 2020 2064 796e 5f73 697a 655f         dyn_size_
+000055b0: 6578 742e 6265 616d 203d 2062 6174 6368  ext.beam = batch
+000055c0: 2e62 6561 6d0a 2020 2020 2020 2020 2020  .beam.          
+000055d0: 2020 2020 2020 2020 2020 6479 6e5f 7369            dyn_si
+000055e0: 7a65 5f65 7874 2e62 6174 6368 203d 2062  ze_ext.batch = b
+000055f0: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
+00005600: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00005610: 2020 2020 2020 2063 7478 203d 2064 796e         ctx = dyn
+00005620: 5f73 697a 655f 6578 742e 636f 6e74 726f  _size_ext.contro
+00005630: 6c5f 666c 6f77 5f63 7478 2069 6620 6479  l_flow_ctx if dy
+00005640: 6e5f 7369 7a65 5f65 7874 2065 6c73 6520  n_size_ext else 
+00005650: 6374 780a 2020 2020 2020 2020 6469 6d5f  ctx.        dim_
+00005660: 7461 6720 3d20 4e6f 6e65 0a20 2020 2020  tag = None.     
+00005670: 2020 2066 6f72 2063 616e 6469 6461 7465     for candidate
+00005680: 2069 6e20 5b73 656c 662c 2073 616d 655f   in [self, same_
+00005690: 6261 7365 5d3a 0a20 2020 2020 2020 2020  base]:.         
+000056a0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+000056b0: 2020 2020 2020 2020 2863 616e 6469 6461          (candida
+000056c0: 7465 2e62 6174 6368 203d 3d20 6261 7463  te.batch == batc
+000056d0: 6820 6f72 2028 6e6f 7420 6361 6e64 6964  h or (not candid
+000056e0: 6174 652e 6261 7463 6820 616e 6420 6261  ate.batch and ba
+000056f0: 7463 682e 6973 5f67 6c6f 6261 6c5f 6261  tch.is_global_ba
+00005700: 7463 6828 2929 290a 2020 2020 2020 2020  tch())).        
+00005710: 2020 2020 2020 2020 616e 6420 6e6f 7420          and not 
+00005720: 6361 6e64 6964 6174 652e 636f 6e74 726f  candidate.contro
+00005730: 6c5f 666c 6f77 5f63 7478 0a20 2020 2020  l_flow_ctx.     
+00005740: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
+00005750: 6f74 2063 7478 0a20 2020 2020 2020 2020  ot ctx.         
+00005760: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00005770: 2020 2020 2020 2320 5468 6520 7361 6d65        # The same
+00005780: 5f62 6173 6520 696e 7374 616e 6365 2069  _base instance i
+00005790: 7320 6569 7468 6572 2075 6e64 6566 696e  s either undefin
+000057a0: 6564 2028 6e6f 2062 6174 6368 2c20 6e6f  ed (no batch, no
+000057b0: 2063 7478 290a 2020 2020 2020 2020 2020   ctx).          
+000057c0: 2020 2020 2020 2320 6f72 2069 7420 6973        # or it is
+000057d0: 2064 6566 696e 6564 2066 6f72 2074 6865   defined for the
+000057e0: 2073 616d 6520 6261 7463 6820 616e 6420   same batch and 
+000057f0: 6374 782e 0a20 2020 2020 2020 2020 2020  ctx..           
+00005800: 2020 2020 2023 2049 6e20 616e 7920 6361       # In any ca
+00005810: 7365 2c20 7265 7573 6520 6974 2074 6865  se, reuse it the
+00005820: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
+00005830: 2020 2063 616e 6469 6461 7465 2e62 6174     candidate.bat
+00005840: 6368 203d 2062 6174 6368 0a20 2020 2020  ch = batch.     
+00005850: 2020 2020 2020 2020 2020 2069 6620 6479             if dy
+00005860: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 6966 2063 616e 6469 6461 7465 2e64 796e  if candidate.dyn
+00005890: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
+000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058b0: 2020 2063 616e 6469 6461 7465 2e64 796e     candidate.dyn
+000058c0: 5f73 697a 655f 6578 742e 6261 7463 6820  _size_ext.batch 
+000058d0: 3d20 6261 7463 680a 2020 2020 2020 2020  = batch.        
 000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 6361 6e64 6964 6174 652e 6479 6e5f 7369  candidate.dyn_si
-00005900: 7a65 5f65 7874 203d 2064 796e 5f73 697a  ze_ext = dyn_siz
-00005910: 655f 6578 740a 2020 2020 2020 2020 2020  e_ext.          
-00005920: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00005930: 206e 6f74 2063 616e 6469 6461 7465 2e64   not candidate.d
-00005940: 796e 5f73 697a 655f 6578 742e 636f 6e74  yn_size_ext.cont
-00005950: 726f 6c5f 666c 6f77 5f63 7478 0a20 2020  rol_flow_ctx.   
-00005960: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00005970: 6620 6361 6e64 6964 6174 652e 6479 6e5f  f candidate.dyn_
-00005980: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-00005990: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-000059a0: 6e64 6964 6174 652e 6479 6e5f 7369 7a65  ndidate.dyn_size
-000059b0: 5f65 7874 2e62 6174 6368 203d 2062 6174  _ext.batch = bat
-000059c0: 6368 0a20 2020 2020 2020 2020 2020 2020  ch.             
-000059d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000059e0: 2020 2020 2020 2020 2020 2020 2063 616e               can
-000059f0: 6469 6461 7465 2e63 6f6d 706c 6574 655f  didate.complete_
-00005a00: 6479 6e5f 7369 7a65 2874 656d 706c 6174  dyn_size(templat
-00005a10: 655f 6f6e 6c79 3d54 7275 6529 0a20 2020  e_only=True).   
-00005a20: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-00005a30: 5f74 6167 203d 2063 616e 6469 6461 7465  _tag = candidate
-00005a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005a50: 2062 7265 616b 0a20 2020 2020 2020 2069   break.        i
-00005a60: 6620 6e6f 7420 6469 6d5f 7461 673a 0a20  f not dim_tag:. 
-00005a70: 2020 2020 2020 2020 2020 2064 696d 5f74             dim_t
-00005a80: 6167 203d 205f 642e 4469 6d28 0a20 2020  ag = _d.Dim(.   
-00005a90: 2020 2020 2020 2020 2020 2020 206b 696e               kin
-00005aa0: 643d 7365 6c66 2e6b 696e 642c 0a20 2020  d=self.kind,.   
-00005ab0: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00005ac0: 6372 6970 7469 6f6e 3d73 656c 662e 6465  cription=self.de
-00005ad0: 7363 7269 7074 696f 6e2c 0a20 2020 2020  scription,.     
-00005ae0: 2020 2020 2020 2020 2020 2064 696d 656e             dimen
-00005af0: 7369 6f6e 3d73 656c 662e 6469 6d65 6e73  sion=self.dimens
-00005b00: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00005b10: 2020 2020 2061 7574 6f5f 6765 6e65 7261       auto_genera
-00005b20: 7465 643d 7365 6c66 2e61 7574 6f5f 6765  ted=self.auto_ge
-00005b30: 6e65 7261 7465 642c 0a20 2020 2020 2020  nerated,.       
-00005b40: 2020 2020 2020 2020 2062 6174 6368 3d62           batch=b
-00005b50: 6174 6368 2c0a 2020 2020 2020 2020 2020  atch,.          
-00005b60: 2020 2020 2020 636f 6e74 726f 6c5f 666c        control_fl
-00005b70: 6f77 5f63 7478 3d63 7478 2c0a 2020 2020  ow_ctx=ctx,.    
-00005b80: 2020 2020 2020 2020 2020 2020 6479 6e5f              dyn_
-00005b90: 7369 7a65 5f65 7874 3d64 796e 5f73 697a  size_ext=dyn_siz
-00005ba0: 655f 6578 742c 0a20 2020 2020 2020 2020  e_ext,.         
-00005bb0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00005bc0: 2064 696d 5f74 6167 2e73 616d 655f 6173   dim_tag.same_as
-00005bd0: 203d 2073 616d 655f 6261 7365 0a20 2020   = same_base.   
-00005be0: 2020 2020 2069 6620 6479 6e5f 7369 7a65       if dyn_size
-00005bf0: 5f65 7874 2061 6e64 2064 796e 5f73 697a  _ext and dyn_siz
-00005c00: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
-00005c10: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-00005c20: 2020 2020 2020 2020 2020 2069 6620 5f64             if _d
-00005c30: 2e44 696d 2e67 6574 5f74 6167 5f66 726f  .Dim.get_tag_fro
-00005c40: 6d5f 7369 7a65 5f74 656e 736f 7228 6479  m_size_tensor(dy
-00005c50: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
-00005c60: 686f 6c64 6572 2920 6973 204e 6f6e 653a  holder) is None:
-00005c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005c80: 2064 696d 5f74 6167 2e73 6574 5f74 6167   dim_tag.set_tag
-00005c90: 5f6f 6e5f 7369 7a65 5f74 656e 736f 7228  _on_size_tensor(
-00005ca0: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
-00005cb0: 6365 686f 6c64 6572 2c20 6261 7463 683d  ceholder, batch=
-00005cc0: 6261 7463 6829 0a20 2020 2020 2020 2073  batch).        s
-00005cd0: 616d 655f 6261 7365 5f65 7874 7261 2e73  ame_base_extra.s
-00005ce0: 616d 655f 666f 725f 6261 7463 685f 6374  ame_for_batch_ct
-00005cf0: 785b 2862 6174 6368 2c20 6374 7829 5d20  x[(batch, ctx)] 
-00005d00: 3d20 6469 6d5f 7461 670a 2020 2020 2020  = dim_tag.      
-00005d10: 2020 6469 6d5f 7461 672e 636f 6d70 6c65    dim_tag.comple
-00005d20: 7465 5f64 796e 5f73 697a 6528 7465 6d70  te_dyn_size(temp
-00005d30: 6c61 7465 5f6f 6e6c 793d 5472 7565 290a  late_only=True).
-00005d40: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00005d50: 696d 5f74 6167 0a0a 2020 2020 6465 6620  im_tag..    def 
-00005d60: 7265 7365 745f 6261 7463 685f 6374 7828  reset_batch_ctx(
-00005d70: 7365 6c66 3a20 4469 6d29 3a0a 2020 2020  self: Dim):.    
-00005d80: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00005d90: 466f 7220 7468 6520 7365 6c66 2069 6e73  For the self ins
-00005da0: 7461 6e63 652c 2072 6573 6574 2062 6174  tance, reset bat
-00005db0: 6368 2061 6e64 2063 6f6e 7465 7874 2e0a  ch and context..
-00005dc0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00005dd0: 2020 2020 6966 2073 656c 662e 5f65 7874      if self._ext
-00005de0: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
-00005df0: 7365 6c66 2e5f 6578 7472 612e 7361 6d65  self._extra.same
-00005e00: 5f66 6f72 5f62 6174 6368 5f63 7478 2e70  _for_batch_ctx.p
-00005e10: 6f70 2828 7365 6c66 2e62 6174 6368 2c20  op((self.batch, 
-00005e20: 7365 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f  self.control_flo
-00005e30: 775f 6374 7829 2c20 4e6f 6e65 290a 2020  w_ctx), None).  
-00005e40: 2020 2020 2020 7365 6c66 2e62 6174 6368        self.batch
-00005e50: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00005e60: 7365 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f  self.control_flo
-00005e70: 775f 6374 7820 3d20 4e6f 6e65 0a20 2020  w_ctx = None.   
-00005e80: 2020 2020 2069 6620 7365 6c66 2e64 796e       if self.dyn
-00005e90: 5f73 697a 655f 6578 7420 616e 6420 7365  _size_ext and se
-00005ea0: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00005eb0: 6261 7463 683a 0a20 2020 2020 2020 2020  batch:.         
-00005ec0: 2020 2073 656c 662e 6479 6e5f 7369 7a65     self.dyn_size
-00005ed0: 5f65 7874 203d 2073 656c 662e 6479 6e5f  _ext = self.dyn_
-00005ee0: 7369 7a65 5f65 7874 2e63 6f70 795f 7465  size_ext.copy_te
-00005ef0: 6d70 6c61 7465 2829 0a20 2020 2020 2020  mplate().       
-00005f00: 2020 2020 2073 656c 662e 6479 6e5f 7369       self.dyn_si
-00005f10: 7a65 5f65 7874 2e62 6174 6368 203d 204e  ze_ext.batch = N
-00005f20: 6f6e 650a 0a20 2020 2064 6566 2073 6574  one..    def set
-00005f30: 5f64 796e 5f73 697a 655f 6578 745f 666f  _dyn_size_ext_fo
-00005f40: 725f 6261 7463 685f 6374 7828 7365 6c66  r_batch_ctx(self
-00005f50: 2c20 6261 7463 682c 2063 7478 2c20 6479  , batch, ctx, dy
-00005f60: 6e5f 7369 7a65 5f65 7874 293a 0a20 2020  n_size_ext):.   
-00005f70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005f80: 203a 7061 7261 6d20 4261 7463 6849 6e66   :param BatchInf
-00005f90: 6f20 6261 7463 683a 0a20 2020 2020 2020  o batch:.       
-00005fa0: 203a 7061 7261 6d20 436f 6e74 726f 6c46   :param ControlF
-00005fb0: 6c6f 7743 6f6e 7465 7874 7c4e 6f6e 6520  lowContext|None 
-00005fc0: 6374 783a 0a20 2020 2020 2020 203a 7061  ctx:.        :pa
-00005fd0: 7261 6d20 4461 7461 2064 796e 5f73 697a  ram Data dyn_siz
-00005fe0: 655f 6578 743a 0a20 2020 2020 2020 2022  e_ext:.        "
-00005ff0: 2222 0a20 2020 2020 2020 2061 7373 6572  "".        asser
-00006000: 7420 7365 6c66 2e63 616e 5f62 655f 7573  t self.can_be_us
-00006010: 6564 5f61 735f 6469 6d28 290a 2020 2020  ed_as_dim().    
-00006020: 2020 2020 7361 6d65 203d 2073 656c 662e      same = self.
-00006030: 6765 745f 666f 725f 6261 7463 685f 6374  get_for_batch_ct
-00006040: 7828 6261 7463 682c 2063 7478 290a 2020  x(batch, ctx).  
-00006050: 2020 2020 2020 6173 7365 7274 2064 796e        assert dyn
-00006060: 5f73 697a 655f 6578 742e 6261 7463 6820  _size_ext.batch 
-00006070: 3d3d 2062 6174 6368 2061 6e64 2064 796e  == batch and dyn
-00006080: 5f73 697a 655f 6578 742e 636f 6e74 726f  _size_ext.contro
-00006090: 6c5f 666c 6f77 5f63 7478 203d 3d20 6374  l_flow_ctx == ct
-000060a0: 780a 2020 2020 2020 2020 6966 2073 616d  x.        if sam
-000060b0: 652e 6479 6e5f 7369 7a65 5f65 7874 3a0a  e.dyn_size_ext:.
-000060c0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-000060d0: 7274 2073 616d 652e 6479 6e5f 7369 7a65  rt same.dyn_size
-000060e0: 5f65 7874 2e64 696d 5f74 6167 7320 3d3d  _ext.dim_tags ==
-000060f0: 2064 796e 5f73 697a 655f 6578 742e 6469   dyn_size_ext.di
-00006100: 6d5f 7461 6773 0a20 2020 2020 2020 2020  m_tags.         
-00006110: 2020 2069 6620 6479 6e5f 7369 7a65 5f65     if dyn_size_e
-00006120: 7874 2e70 6c61 6365 686f 6c64 6572 2069  xt.placeholder i
-00006130: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00006140: 2020 2020 2020 2020 2020 2020 7361 6d65              same
-00006150: 2e64 796e 5f73 697a 655f 6578 742e 706c  .dyn_size_ext.pl
-00006160: 6163 6568 6f6c 6465 7220 3d20 6479 6e5f  aceholder = dyn_
-00006170: 7369 7a65 5f65 7874 2e70 6c61 6365 686f  size_ext.placeho
-00006180: 6c64 6572 0a20 2020 2020 2020 2065 6c73  lder.        els
-00006190: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000061a0: 616d 652e 6479 6e5f 7369 7a65 5f65 7874  ame.dyn_size_ext
-000061b0: 203d 2064 796e 5f73 697a 655f 6578 740a   = dyn_size_ext.
-000061c0: 2020 2020 2020 2020 7365 6c66 2e5f 6d61          self._ma
-000061d0: 7962 655f 7570 6461 7465 2829 0a0a 2020  ybe_update()..  
-000061e0: 2020 6465 6620 6765 745f 6479 6e5f 7369    def get_dyn_si
-000061f0: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
-00006200: 5f63 7478 2873 656c 662c 2062 6174 6368  _ctx(self, batch
-00006210: 2c20 6374 782c 2074 656d 706c 6174 655f  , ctx, template_
-00006220: 6f6e 6c79 3d46 616c 7365 293a 0a20 2020  only=False):.   
-00006230: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00006240: 203a 7061 7261 6d20 4261 7463 6849 6e66   :param BatchInf
-00006250: 6f7c 4e6f 6e65 2062 6174 6368 3a0a 2020  o|None batch:.  
-00006260: 2020 2020 2020 3a70 6172 616d 2043 6f6e        :param Con
-00006270: 7472 6f6c 466c 6f77 436f 6e74 6578 747c  trolFlowContext|
-00006280: 4e6f 6e65 2063 7478 3a0a 2020 2020 2020  None ctx:.      
-00006290: 2020 3a70 6172 616d 2062 6f6f 6c20 7465    :param bool te
-000062a0: 6d70 6c61 7465 5f6f 6e6c 793a 0a20 2020  mplate_only:.   
-000062b0: 2020 2020 203a 7274 7970 653a 2044 6174       :rtype: Dat
-000062c0: 617c 4e6f 6e65 0a20 2020 2020 2020 2022  a|None.        "
-000062d0: 2222 0a20 2020 2020 2020 2061 7373 6572  "".        asser
-000062e0: 7420 7365 6c66 2e63 616e 5f62 655f 7573  t self.can_be_us
-000062f0: 6564 5f61 735f 6469 6d28 290a 2020 2020  ed_as_dim().    
-00006300: 2020 2020 6966 206e 6f74 2062 6174 6368      if not batch
-00006310: 2061 6e64 2073 656c 662e 6261 7463 683a   and self.batch:
-00006320: 0a20 2020 2020 2020 2020 2020 2023 2041  .            # A
-00006330: 7373 756d 6520 676c 6f62 616c 2062 6174  ssume global bat
-00006340: 6368 2e0a 2020 2020 2020 2020 2020 2020  ch..            
-00006350: 6261 7463 6820 3d20 7365 6c66 2e62 6174  batch = self.bat
-00006360: 6368 2e67 6574 5f67 6c6f 6261 6c5f 6261  ch.get_global_ba
-00006370: 7365 2829 0a20 2020 2020 2020 2069 6620  se().        if 
-00006380: 6e6f 7420 6261 7463 683a 0a20 2020 2020  not batch:.     
-00006390: 2020 2020 2020 2023 2054 6869 7320 6973         # This is
-000063a0: 2075 7375 616c 6c79 206e 6f74 2076 616c   usually not val
-000063b0: 6964 2e20 486f 7765 7665 722c 2074 6869  id. However, thi
-000063c0: 7320 6361 7365 2063 616e 2068 6170 7065  s case can happe
-000063d0: 6e20 6561 726c 7920 6174 2069 6e69 7469  n early at initi
-000063e0: 616c 697a 6174 696f 6e2e 0a20 2020 2020  alization..     
-000063f0: 2020 2020 2020 2061 7373 6572 7420 6261         assert ba
-00006400: 7463 6820 3d3d 2073 656c 662e 6261 7463  tch == self.batc
-00006410: 6820 616e 6420 6374 7820 3d3d 2073 656c  h and ctx == sel
-00006420: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
-00006430: 7478 0a20 2020 2020 2020 2020 2020 2072  tx.            r
-00006440: 6574 7572 6e20 7365 6c66 2e64 796e 5f73  eturn self.dyn_s
-00006450: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
-00006460: 7361 6d65 203d 2073 656c 662e 6765 745f  same = self.get_
-00006470: 666f 725f 6261 7463 685f 6374 7828 6261  for_batch_ctx(ba
-00006480: 7463 682c 2063 7478 2c20 616c 6c6f 775f  tch, ctx, allow_
-00006490: 6e6f 6e65 3d54 7275 6529 0a20 2020 2020  none=True).     
-000064a0: 2020 2069 6620 6e6f 7420 7361 6d65 3a0a     if not same:.
-000064b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000064c0: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
-000064d0: 7361 6d65 2e63 6f6d 706c 6574 655f 6479  same.complete_dy
-000064e0: 6e5f 7369 7a65 2874 656d 706c 6174 655f  n_size(template_
-000064f0: 6f6e 6c79 3d74 656d 706c 6174 655f 6f6e  only=template_on
-00006500: 6c79 290a 2020 2020 2020 2020 7265 7475  ly).        retu
-00006510: 726e 2073 616d 652e 6479 6e5f 7369 7a65  rn same.dyn_size
-00006520: 5f65 7874 0a0a 2020 2020 4070 726f 7065  _ext..    @prope
-00006530: 7274 790a 2020 2020 6465 6620 6479 6e5f  rty.    def dyn_
-00006540: 7369 7a65 2873 656c 6629 3a0a 2020 2020  size(self):.    
-00006550: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006560: 3a72 6574 7572 6e3a 2064 796e 2073 697a  :return: dyn siz
-00006570: 6520 2f20 7365 7120 6c65 6e20 2875 7375  e / seq len (usu
-00006580: 616c 6c79 206f 6620 7368 6170 6520 5b42  ally of shape [B
-00006590: 5d29 2c20 6f72 204e 6f6e 650a 2020 2020  ]), or None.    
-000065a0: 2020 2020 2020 4966 2074 6865 2064 796e        If the dyn
-000065b0: 2073 697a 6520 6361 6e20 706f 7465 6e74   size can potent
-000065c0: 6961 6c6c 7920 6265 206f 6620 6120 6469  ially be of a di
-000065d0: 6666 6572 656e 7420 7368 6170 652c 2064  fferent shape, d
-000065e0: 6972 6563 746c 7920 6163 6365 7373 2064  irectly access d
-000065f0: 796e 5f73 697a 655f 6578 742e 0a20 2020  yn_size_ext..   
-00006600: 2020 2020 203a 7274 7970 653a 2074 662e       :rtype: tf.
-00006610: 5465 6e73 6f72 7c4e 6f6e 650a 2020 2020  Tensor|None.    
-00006620: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006630: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
-00006640: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
-00006650: 2020 7265 7475 726e 2073 656c 662e 6479    return self.dy
-00006660: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
-00006670: 686f 6c64 6572 0a20 2020 2020 2020 2072  holder.        r
-00006680: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00006690: 4064 796e 5f73 697a 652e 7365 7474 6572  @dyn_size.setter
-000066a0: 0a20 2020 2064 6566 2064 796e 5f73 697a  .    def dyn_siz
-000066b0: 6528 7365 6c66 2c20 6479 6e5f 7369 7a65  e(self, dyn_size
-000066c0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-000066d0: 2020 2020 2020 2041 6c73 6f20 7365 6520         Also see 
-000066e0: 3a66 756e 633a 6073 6574 5f64 796e 5f73  :func:`set_dyn_s
-000066f0: 697a 655f 6578 745f 666f 725f 6261 7463  ize_ext_for_batc
-00006700: 685f 6374 7860 2e0a 0a20 2020 2020 2020  h_ctx`...       
-00006710: 203a 7061 7261 6d20 7466 2e54 656e 736f   :param tf.Tenso
-00006720: 7220 6479 6e5f 7369 7a65 3a0a 2020 2020  r dyn_size:.    
-00006730: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006740: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
-00006750: 5f65 7874 2061 6e64 2073 656c 662e 6479  _ext and self.dy
-00006760: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
-00006770: 686f 6c64 6572 2069 7320 6479 6e5f 7369  holder is dyn_si
-00006780: 7a65 3a20 2023 2066 6173 7420 7061 7468  ze:  # fast path
-00006790: 2063 6865 636b 0a20 2020 2020 2020 2020   check.         
-000067a0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000067b0: 2020 6173 7365 7274 2073 656c 662e 6361    assert self.ca
-000067c0: 6e5f 6265 5f75 7365 645f 6173 5f64 696d  n_be_used_as_dim
-000067d0: 2829 0a20 2020 2020 2020 206f 7468 6572  ().        other
-000067e0: 203d 205f 642e 4469 6d2e 6765 745f 7461   = _d.Dim.get_ta
-000067f0: 675f 6672 6f6d 5f73 697a 655f 7465 6e73  g_from_size_tens
-00006800: 6f72 2864 796e 5f73 697a 6529 0a20 2020  or(dyn_size).   
-00006810: 2020 2020 2069 6620 6f74 6865 723a 0a20       if other:. 
-00006820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006830: 6465 636c 6172 655f 7361 6d65 5f61 7328  declare_same_as(
-00006840: 6f74 6865 7229 0a20 2020 2020 2020 2020  other).         
-00006850: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
-00006860: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006870: 2020 6173 7365 7274 2073 656c 662e 6261    assert self.ba
-00006880: 7463 6820 3d3d 206f 7468 6572 2e62 6174  tch == other.bat
-00006890: 6368 2061 6e64 2073 656c 662e 636f 6e74  ch and self.cont
-000068a0: 726f 6c5f 666c 6f77 5f63 7478 203d 3d20  rol_flow_ctx == 
-000068b0: 6f74 6865 722e 636f 6e74 726f 6c5f 666c  other.control_fl
-000068c0: 6f77 5f63 7478 0a20 2020 2020 2020 2020  ow_ctx.         
-000068d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000068e0: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
-000068f0: 7463 6820 3d20 6f74 6865 722e 6261 7463  tch = other.batc
-00006900: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
-00006910: 2020 7365 6c66 2e63 6f6e 7472 6f6c 5f66    self.control_f
-00006920: 6c6f 775f 6374 7820 3d20 6f74 6865 722e  low_ctx = other.
-00006930: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
-00006940: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006950: 662e 6479 6e5f 7369 7a65 5f65 7874 203d  f.dyn_size_ext =
-00006960: 206f 7468 6572 2e64 796e 5f73 697a 655f   other.dyn_size_
-00006970: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
-00006980: 7265 7475 726e 0a20 2020 2020 2020 2073  return.        s
-00006990: 656c 662e 5f69 6e69 745f 6465 6661 756c  elf._init_defaul
-000069a0: 745f 6479 6e5f 7369 7a65 5f65 7874 2864  t_dyn_size_ext(d
-000069b0: 796e 5f73 697a 6529 0a20 2020 2020 2020  yn_size).       
-000069c0: 2073 656c 662e 7365 745f 7461 675f 6f6e   self.set_tag_on
-000069d0: 5f73 697a 655f 7465 6e73 6f72 2864 796e  _size_tensor(dyn
-000069e0: 5f73 697a 6529 0a0a 2020 2020 6465 6620  _size)..    def 
-000069f0: 5f69 6e69 745f 6465 6661 756c 745f 6479  _init_default_dy
-00006a00: 6e5f 7369 7a65 5f65 7874 2873 656c 662c  n_size_ext(self,
-00006a10: 2064 796e 5f73 697a 6529 3a0a 2020 2020   dyn_size):.    
-00006a20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006a30: 3a70 6172 616d 2074 662e 5465 6e73 6f72  :param tf.Tensor
-00006a40: 2064 796e 5f73 697a 653a 0a20 2020 2020   dyn_size:.     
-00006a50: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00006a60: 6620 7365 6c66 2e64 796e 5f73 697a 655f  f self.dyn_size_
-00006a70: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-00006a80: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
-00006a90: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
-00006aa0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-00006ab0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00006ac0: 2044 6f20 6e6f 7420 616c 6c6f 7720 7265   Do not allow re
-00006ad0: 7365 7474 696e 6720 6974 2074 6f20 7374  setting it to st
-00006ae0: 6820 6469 6666 6572 656e 742e 0a20 2020  h different..   
-00006af0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-00006b00: 6572 7420 7365 6c66 2e64 796e 5f73 697a  ert self.dyn_siz
-00006b10: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
-00006b20: 7220 6973 2064 796e 5f73 697a 650a 2020  r is dyn_size.  
-00006b30: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00006b40: 2020 2020 2020 2020 6265 616d 203d 2067          beam = g
-00006b50: 6574 6174 7472 2864 796e 5f73 697a 652c  etattr(dyn_size,
-00006b60: 2022 5f52 4554 5552 4e4e 5f64 796e 5f73   "_RETURNN_dyn_s
-00006b70: 697a 655f 6265 616d 222c 204e 6f6e 6529  ize_beam", None)
-00006b80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006b90: 662e 6479 6e5f 7369 7a65 5f65 7874 203d  f.dyn_size_ext =
-00006ba0: 205f 742e 5465 6e73 6f72 280a 2020 2020   _t.Tensor(.    
-00006bb0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00006bc0: 3d28 2225 733a 6479 6e5f 7369 7a65 2220  =("%s:dyn_size" 
-00006bd0: 2520 7365 6c66 2e64 6573 6372 6970 7469  % self.descripti
-00006be0: 6f6e 2920 6966 2073 656c 662e 6465 7363  on) if self.desc
-00006bf0: 7269 7074 696f 6e20 656c 7365 2064 796e  ription else dyn
-00006c00: 5f73 697a 652e 6f70 2e6e 616d 652c 0a20  _size.op.name,. 
-00006c10: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006c20: 7479 7065 3d5f 742e 5465 6e73 6f72 2e73  type=_t.Tensor.s
-00006c30: 697a 655f 6474 7970 652c 0a20 2020 2020  ize_dtype,.     
-00006c40: 2020 2020 2020 2020 2020 2073 6861 7065             shape
-00006c50: 3d28 292c 0a20 2020 2020 2020 2020 2020  =(),.           
-00006c60: 2020 2020 2062 6174 6368 5f64 696d 5f61       batch_dim_a
-00006c70: 7869 733d 302c 0a20 2020 2020 2020 2020  xis=0,.         
-00006c80: 2020 2020 2020 2062 6174 6368 3d73 656c         batch=sel
-00006c90: 662e 6261 7463 682c 0a20 2020 2020 2020  f.batch,.       
-00006ca0: 2020 2020 2020 2020 2062 6561 6d3d 6265           beam=be
-00006cb0: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
-00006cc0: 2020 2020 636f 6e74 726f 6c5f 666c 6f77      control_flow
-00006cd0: 5f63 7478 3d73 656c 662e 636f 6e74 726f  _ctx=self.contro
-00006ce0: 6c5f 666c 6f77 5f63 7478 2c0a 2020 2020  l_flow_ctx,.    
-00006cf0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00006d00: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
-00006d10: 6578 742e 706c 6163 6568 6f6c 6465 7220  ext.placeholder 
-00006d20: 3d20 6479 6e5f 7369 7a65 0a0a 2020 2020  = dyn_size..    
-00006d30: 6465 6620 6765 745f 6d61 736b 2873 656c  def get_mask(sel
-00006d40: 663a 2044 696d 2c20 2a2c 2064 696d 5f6f  f: Dim, *, dim_o
-00006d50: 7264 6572 3a20 4f70 7469 6f6e 616c 5b53  rder: Optional[S
-00006d60: 6571 7565 6e63 655b 4469 6d5d 5d20 3d20  equence[Dim]] = 
-00006d70: 4e6f 6e65 2920 2d3e 205f 742e 5465 6e73  None) -> _t.Tens
-00006d80: 6f72 3a0a 2020 2020 2020 2020 2222 220a  or:.        """.
-00006d90: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00006da0: 696d 5f6f 7264 6572 3a20 6966 2067 6976  im_order: if giv
-00006db0: 656e 2c20 7468 6520 6469 6d73 206f 6620  en, the dims of 
-00006dc0: 7468 6520 6d61 736b 2077 696c 6c20 6265  the mask will be
-00006dd0: 2069 6e20 7468 6973 206f 7264 6572 2e0a   in this order..
-00006de0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-00006df0: 2063 616e 2062 6520 7573 6566 756c 2069   can be useful i
-00006e00: 6620 7468 6520 6d61 736b 2069 7320 6272  f the mask is br
-00006e10: 6f61 6463 6173 7465 6420 6167 6169 6e73  oadcasted agains
-00006e20: 7420 736f 6d65 206f 7468 6572 2074 656e  t some other ten
-00006e30: 736f 722e 0a20 2020 2020 2020 203a 7265  sor..        :re
-00006e40: 7475 726e 3a20 6966 206e 6565 645f 6d61  turn: if need_ma
-00006e50: 736b 696e 6728 292c 2074 6865 2063 6f72  sking(), the cor
-00006e60: 7265 7370 6f6e 6469 6e67 206d 6173 6b2e  responding mask.
-00006e70: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00006e80: 7468 6973 2069 7320 652e 672e 2074 6865  this is e.g. the
-00006e90: 2074 696d 652d 6469 6d20 5420 6f66 2073   time-dim T of s
-00006ea0: 6861 7065 205b 425d 2c20 7468 656e 2074  hape [B], then t
-00006eb0: 6865 206d 6173 6b20 7769 6c6c 2062 6520  he mask will be 
-00006ec0: 6f66 2073 6861 7065 205b 422c 545d 2e0a  of shape [B,T]..
-00006ed0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00006ee0: 6d61 736b 2063 6f75 6c64 2062 6520 7573  mask could be us
-00006ef0: 6564 2077 6974 6820 3a66 756e 633a 606d  ed with :func:`m
-00006f00: 6173 6b65 645f 7365 6c65 6374 6020 2860  asked_select` (`
-00006f10: 6062 6f6f 6c65 616e 5f6d 6173 6b60 6029  `boolean_mask``)
-00006f20: 206f 7220 6060 7768 6572 6560 602e 0a20   or ``where``.. 
-00006f30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00006f40: 2020 2069 6d70 6f72 7420 7265 7475 726e     import return
-00006f50: 6e2e 6672 6f6e 7465 6e64 2061 7320 7266  n.frontend as rf
-00006f60: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00006f70: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00006f80: 7874 2061 6e64 2073 656c 662e 6479 6e5f  xt and self.dyn_
-00006f90: 7369 7a65 5f65 7874 2e72 6177 5f74 656e  size_ext.raw_ten
-00006fa0: 736f 7220 6973 206e 6f74 204e 6f6e 650a  sor is not None.
-00006fb0: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
-00006fc0: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
-00006fd0: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
-00006fe0: 2062 6163 6b65 6e64 203d 2073 656c 662e   backend = self.
-00006ff0: 6479 6e5f 7369 7a65 5f65 7874 2e5f 7261  dyn_size_ext._ra
-00007000: 775f 6261 636b 656e 640a 0a20 2020 2020  w_backend..     
-00007010: 2020 206d 6178 5f69 6478 203d 2072 662e     max_idx = rf.
-00007020: 7265 6475 6365 280a 2020 2020 2020 2020  reduce(.        
-00007030: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
-00007040: 655f 6578 742c 0a20 2020 2020 2020 2020  e_ext,.         
-00007050: 2020 2061 7869 733d 7365 6c66 2e64 796e     axis=self.dyn
-00007060: 5f73 697a 655f 6578 742e 6469 6d73 2c0a  _size_ext.dims,.
-00007070: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00007080: 3d22 6d61 7822 2c0a 2020 2020 2020 2020  ="max",.        
-00007090: 2020 2020 2320 4d61 736b 696e 6720 6865      # Masking he
-000070a0: 7265 2069 7320 6e6f 7420 616c 7761 7973  re is not always
-000070b0: 2070 6f73 7369 626c 652c 2065 2e67 2e20   possible, e.g. 
-000070c0: 6966 2077 6520 6861 7665 0a20 2020 2020  if we have.     
-000070d0: 2020 2020 2020 2023 2074 6167 203d 2044         # tag = D
-000070e0: 696d 7b27 7365 6c66 2d61 7474 2d6b 6579  im{'self-att-key
-000070f0: 7327 5b27 7469 6d65 3a76 6172 3a65 7874  s'['time:var:ext
-00007100: 6572 6e5f 6461 7461 3a63 6c61 7373 6573  ern_data:classes
-00007110: 275b 425d 5d7d 0a20 2020 2020 2020 2020  '[B]]}.         
-00007120: 2020 2075 7365 5f6d 6173 6b3d 4661 6c73     use_mask=Fals
-00007130: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
-00007140: 2020 2020 2023 2057 6520 7573 6520 7468       # We use th
-00007150: 6520 6173 7375 6d70 7469 6f6e 2074 6861  e assumption tha
-00007160: 7420 7365 6c66 2e70 6c61 6365 686f 6c64  t self.placehold
-00007170: 6572 2e73 6861 7065 5b61 7869 735d 203d  er.shape[axis] =
-00007180: 3d20 6d61 785f 6964 782e 0a20 2020 2020  = max_idx..     
-00007190: 2020 2023 2073 697a 655f 6578 7420 6d69     # size_ext mi
-000071a0: 6768 7420 6861 7665 2069 6e76 616c 6964  ght have invalid
-000071b0: 2028 7a65 726f 2920 7369 7a65 730a 2020   (zero) sizes.  
-000071c0: 2020 2020 2020 2320 7768 656e 2069 7420        # when it 
-000071d0: 6974 7365 6c66 2068 6173 2073 6f6d 6520  itself has some 
-000071e0: 7061 6464 696e 672c 2065 2e67 2e20 7768  padding, e.g. wh
-000071f0: 656e 2069 7473 206f 776e 2073 6861 7065  en its own shape
-00007200: 2069 7320 6479 6e61 6d69 632e 0a20 2020   is dynamic..   
-00007210: 2020 2020 2023 2041 207a 6572 6f20 7369       # A zero si
-00007220: 7a65 2063 616e 206c 6561 6420 746f 2070  ze can lead to p
-00007230: 726f 626c 656d 7320 696e 2073 6f6d 6520  roblems in some 
-00007240: 6361 7365 732c 2065 2e67 2e20 696e 2053  cases, e.g. in S
-00007250: 6f66 746d 6178 4f76 6572 5370 6174 6961  oftmaxOverSpatia
-00007260: 6c4c 6179 6572 2c0a 2020 2020 2020 2020  lLayer,.        
-00007270: 2320 7768 656e 2065 7665 7279 7468 696e  # when everythin
-00007280: 6720 6973 206d 6173 6b65 6420 746f 202d  g is masked to -
-00007290: 696e 662c 2069 7420 7265 7375 6c74 7320  inf, it results 
-000072a0: 696e 206e 616e 2c0a 2020 2020 2020 2020  in nan,.        
-000072b0: 2320 616e 6420 7468 6973 206c 696b 656c  # and this likel
-000072c0: 7920 7072 6f64 7563 6573 206e 616e 2069  y produces nan i
-000072d0: 6e20 6261 636b 7072 6f70 206f 7220 656c  n backprop or el
-000072e0: 7365 7768 6572 652e 0a20 2020 2020 2020  sewhere..       
-000072f0: 2023 2054 6875 732c 206d 6173 6b20 7369   # Thus, mask si
-00007300: 7a65 5f65 7874 2069 7473 656c 662c 2061  ze_ext itself, a
-00007310: 6e64 2073 6574 2074 6865 2070 6164 6465  nd set the padde
-00007320: 6420 7661 6c75 6573 2074 6f20 312e 0a20  d values to 1.. 
-00007330: 2020 2020 2020 2023 2054 6869 7320 6173         # This as
-00007340: 7375 6d65 7320 7468 6174 206d 6178 5f69  sumes that max_i
-00007350: 6478 203e 3d20 312e 0a20 2020 2020 2020  dx >= 1..       
-00007360: 2073 697a 655f 6578 7420 3d20 7365 6c66   size_ext = self
-00007370: 2e64 796e 5f73 697a 655f 6578 742e 636f  .dyn_size_ext.co
-00007380: 7079 5f6d 6173 6b65 6428 6d61 785f 6964  py_masked(max_id
-00007390: 7829 0a20 2020 2020 2020 2069 6478 5f72  x).        idx_r
-000073a0: 616e 6765 203d 2062 6163 6b65 6e64 2e72  ange = backend.r
-000073b0: 616e 6765 5f6f 7665 725f 6469 6d28 7365  ange_over_dim(se
-000073c0: 6c66 290a 2020 2020 2020 2020 7365 715f  lf).        seq_
-000073d0: 6d61 736b 203d 2072 662e 636f 6d70 6172  mask = rf.compar
-000073e0: 6528 6964 785f 7261 6e67 652c 2022 3c22  e(idx_range, "<"
-000073f0: 2c20 7369 7a65 5f65 7874 2c20 616c 6c6f  , size_ext, allo
-00007400: 775f 6272 6f61 6463 6173 745f 616c 6c5f  w_broadcast_all_
-00007410: 736f 7572 6365 733d 5472 7565 2c20 6469  sources=True, di
-00007420: 6d5f 6f72 6465 723d 6469 6d5f 6f72 6465  m_order=dim_orde
-00007430: 7229 0a20 2020 2020 2020 2072 6574 7572  r).        retur
-00007440: 6e20 7365 715f 6d61 736b 0a0a 2020 2020  n seq_mask..    
-00007450: 6465 6620 6973 5f62 6174 6368 5f64 696d  def is_batch_dim
-00007460: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007470: 2222 220a 2020 2020 2020 2020 3a72 6574  """.        :ret
-00007480: 7572 6e3a 2077 6865 7468 6572 2074 6869  urn: whether thi
-00007490: 7320 6469 6d20 7461 6720 6973 206f 6620  s dim tag is of 
-000074a0: 6b69 6e64 2062 6174 6368 0a20 2020 2020  kind batch.     
-000074b0: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-000074c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000074d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000074e0: 6b69 6e64 203d 3d20 4469 6d54 7970 6573  kind == DimTypes
-000074f0: 2e42 6174 6368 0a0a 2020 2020 6465 6620  .Batch..    def 
-00007500: 6973 5f66 6561 7475 7265 5f64 696d 2873  is_feature_dim(s
-00007510: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00007520: 220a 2020 2020 2020 2020 3a72 6574 7572  ".        :retur
-00007530: 6e3a 2077 6865 7468 6572 2074 6869 7320  n: whether this 
-00007540: 6469 6d20 7461 6720 6973 206f 6620 6b69  dim tag is of ki
-00007550: 6e64 2066 6561 7475 7265 0a20 2020 2020  nd feature.     
-00007560: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-00007570: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00007580: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00007590: 6b69 6e64 203d 3d20 4469 6d54 7970 6573  kind == DimTypes
-000075a0: 2e46 6561 7475 7265 0a0a 2020 2020 6465  .Feature..    de
-000075b0: 6620 6973 5f73 7061 7469 616c 5f64 696d  f is_spatial_dim
-000075c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000075d0: 2222 220a 2020 2020 2020 2020 3a72 6574  """.        :ret
-000075e0: 7572 6e3a 2077 6865 7468 6572 2074 6869  urn: whether thi
-000075f0: 7320 6469 6d20 7461 6720 6973 206f 6620  s dim tag is of 
-00007600: 6b69 6e64 2073 7061 7469 616c 0a20 2020  kind spatial.   
-00007610: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00007620: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-00007630: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00007640: 662e 6b69 6e64 203d 3d20 4469 6d54 7970  f.kind == DimTyp
-00007650: 6573 2e53 7061 7469 616c 0a0a 2020 2020  es.Spatial..    
-00007660: 6465 6620 6973 5f64 696d 5f6b 6e6f 776e  def is_dim_known
-00007670: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007680: 2222 220a 2020 2020 2020 2020 3a72 6574  """.        :ret
-00007690: 7572 6e3a 2077 6865 7468 6572 2077 6520  urn: whether we 
-000076a0: 6b6e 6f77 2074 6865 2064 696d 656e 7369  know the dimensi
-000076b0: 6f6e 3b20 6261 7369 6361 6c6c 7920 7768  on; basically wh
-000076c0: 6574 6865 7220 7468 6973 2069 7320 6465  ether this is de
-000076d0: 6669 6e65 640a 2020 2020 2020 2020 2020  fined.          
-000076e0: 2861 6c74 686f 7567 6820 606e 6f74 2073  (although `not s
-000076f0: 656c 662e 756e 6465 6669 6e65 6460 2069  elf.undefined` i
-00007700: 7320 6465 6669 6e65 6420 736c 6967 6874  s defined slight
-00007710: 6c79 2064 6966 6665 7265 6e74 6c79 290a  ly differently).
-00007720: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00007730: 626f 6f6c 0a20 2020 2020 2020 2022 2222  bool.        """
-00007740: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00007750: 2e69 735f 6261 7463 685f 6469 6d28 293a  .is_batch_dim():
-00007760: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00007770: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00007780: 2069 6620 6e6f 7420 7365 6c66 2e69 735f   if not self.is_
-00007790: 6479 6e61 6d69 6328 2920 616e 6420 7365  dynamic() and se
-000077a0: 6c66 2e64 696d 656e 7369 6f6e 2069 7320  lf.dimension is 
-000077b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000077c0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000077d0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-000077e0: 662e 6479 6e5f 7369 7a65 5f65 7874 3a0a  f.dyn_size_ext:.
-000077f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00007800: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-00007810: 6578 7472 6120 3d20 7365 6c66 2e5f 6765  extra = self._ge
-00007820: 745f 7361 6d65 5f62 6173 655f 6578 7472  t_same_base_extr
-00007830: 6128 290a 2020 2020 2020 2020 6966 2065  a().        if e
-00007840: 7874 7261 3a0a 2020 2020 2020 2020 2020  xtra:.          
-00007850: 2020 666f 7220 5f2c 206f 7468 6572 2069    for _, other i
-00007860: 6e20 6578 7472 612e 7361 6d65 5f66 6f72  n extra.same_for
-00007870: 5f62 6174 6368 5f63 7478 2e69 7465 6d73  _batch_ctx.items
-00007880: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00007890: 2020 2020 6966 206f 7468 6572 2e64 796e      if other.dyn
-000078a0: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-000078b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000078c0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-000078d0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-000078e0: 0a20 2020 2064 6566 2069 735f 6479 6e61  .    def is_dyna
-000078f0: 6d69 6328 7365 6c66 2920 2d3e 2062 6f6f  mic(self) -> boo
-00007900: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-00007910: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00007920: 7768 6574 6865 7220 7468 6520 6469 6d20  whether the dim 
-00007930: 6973 206e 6f74 2073 7461 7469 632e 2075  is not static. u
-00007940: 7375 616c 6c79 206d 6561 6e73 2074 6861  sually means tha
-00007950: 7420 6974 2068 6173 2073 6571 206c 656e  t it has seq len
-00007960: 6774 6873 0a20 2020 2020 2020 2022 2222  gths.        """
-00007970: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00007980: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
-00007990: 7320 4e6f 6e65 2061 6e64 206e 6f74 2073  s None and not s
-000079a0: 656c 662e 6973 5f62 6174 6368 5f64 696d  elf.is_batch_dim
-000079b0: 2829 0a0a 2020 2020 6465 6620 6973 5f73  ()..    def is_s
-000079c0: 7461 7469 6328 7365 6c66 2920 2d3e 2062  tatic(self) -> b
-000079d0: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-000079e0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000079f0: 3a20 7374 6174 6963 0a20 2020 2020 2020  : static.       
-00007a00: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00007a10: 7572 6e20 6e6f 7420 7365 6c66 2e69 735f  urn not self.is_
-00007a20: 6479 6e61 6d69 6328 290a 0a20 2020 2064  dynamic()..    d
-00007a30: 6566 206e 6565 645f 6d61 736b 696e 6728  ef need_masking(
-00007a40: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000058f0: 6173 7365 7274 2063 616e 6469 6461 7465  assert candidate
+00005900: 2e64 796e 5f73 697a 655f 6578 742e 6469  .dyn_size_ext.di
+00005910: 6d5f 7461 6773 203d 3d20 6479 6e5f 7369  m_tags == dyn_si
+00005920: 7a65 5f65 7874 2e64 696d 5f74 6167 730a  ze_ext.dim_tags.
+00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005940: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 2020 6361 6e64 6964 6174 652e 6479 6e5f    candidate.dyn_
+00005970: 7369 7a65 5f65 7874 203d 2064 796e 5f73  size_ext = dyn_s
+00005980: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
+00005990: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+000059a0: 7274 206e 6f74 2063 616e 6469 6461 7465  rt not candidate
+000059b0: 2e64 796e 5f73 697a 655f 6578 742e 636f  .dyn_size_ext.co
+000059c0: 6e74 726f 6c5f 666c 6f77 5f63 7478 0a20  ntrol_flow_ctx. 
+000059d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000059e0: 6c69 6620 6361 6e64 6964 6174 652e 6479  lif candidate.dy
+000059f0: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
+00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a10: 6361 6e64 6964 6174 652e 6479 6e5f 7369  candidate.dyn_si
+00005a20: 7a65 5f65 7874 2e62 6174 6368 203d 2062  ze_ext.batch = b
+00005a30: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
+00005a40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00005a50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00005a60: 616e 6469 6461 7465 2e63 6f6d 706c 6574  andidate.complet
+00005a70: 655f 6479 6e5f 7369 7a65 2874 656d 706c  e_dyn_size(templ
+00005a80: 6174 655f 6f6e 6c79 3d54 7275 6529 0a20  ate_only=True). 
+00005a90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00005aa0: 696d 5f74 6167 203d 2063 616e 6469 6461  im_tag = candida
+00005ab0: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
+00005ac0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00005ad0: 2069 6620 6e6f 7420 6469 6d5f 7461 673a   if not dim_tag:
+00005ae0: 0a20 2020 2020 2020 2020 2020 2064 696d  .            dim
+00005af0: 5f74 6167 203d 205f 642e 4469 6d28 0a20  _tag = _d.Dim(. 
+00005b00: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00005b10: 696e 643d 7365 6c66 2e6b 696e 642c 0a20  ind=self.kind,. 
+00005b20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00005b30: 6573 6372 6970 7469 6f6e 3d73 656c 662e  escription=self.
+00005b40: 6465 7363 7269 7074 696f 6e2c 0a20 2020  description,.   
+00005b50: 2020 2020 2020 2020 2020 2020 2064 696d               dim
+00005b60: 656e 7369 6f6e 3d73 656c 662e 6469 6d65  ension=self.dime
+00005b70: 6e73 696f 6e2c 0a20 2020 2020 2020 2020  nsion,.         
+00005b80: 2020 2020 2020 2061 7574 6f5f 6765 6e65         auto_gene
+00005b90: 7261 7465 643d 7365 6c66 2e61 7574 6f5f  rated=self.auto_
+00005ba0: 6765 6e65 7261 7465 642c 0a20 2020 2020  generated,.     
+00005bb0: 2020 2020 2020 2020 2020 2062 6174 6368             batch
+00005bc0: 3d62 6174 6368 2c0a 2020 2020 2020 2020  =batch,.        
+00005bd0: 2020 2020 2020 2020 636f 6e74 726f 6c5f          control_
+00005be0: 666c 6f77 5f63 7478 3d63 7478 2c0a 2020  flow_ctx=ctx,.  
+00005bf0: 2020 2020 2020 2020 2020 2020 2020 6479                dy
+00005c00: 6e5f 7369 7a65 5f65 7874 3d64 796e 5f73  n_size_ext=dyn_s
+00005c10: 697a 655f 6578 742c 0a20 2020 2020 2020  ize_ext,.       
+00005c20: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00005c30: 2020 2064 696d 5f74 6167 2e73 616d 655f     dim_tag.same_
+00005c40: 6173 203d 2073 616d 655f 6261 7365 0a20  as = same_base. 
+00005c50: 2020 2020 2020 2069 6620 6479 6e5f 7369         if dyn_si
+00005c60: 7a65 5f65 7874 2061 6e64 2064 796e 5f73  ze_ext and dyn_s
+00005c70: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
+00005c80: 6465 7220 6973 206e 6f74 204e 6f6e 653a  der is not None:
+00005c90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00005ca0: 5f64 2e44 696d 2e67 6574 5f74 6167 5f66  _d.Dim.get_tag_f
+00005cb0: 726f 6d5f 7369 7a65 5f74 656e 736f 7228  rom_size_tensor(
+00005cc0: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
+00005cd0: 6365 686f 6c64 6572 2920 6973 204e 6f6e  ceholder) is Non
+00005ce0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00005cf0: 2020 2064 696d 5f74 6167 2e73 6574 5f74     dim_tag.set_t
+00005d00: 6167 5f6f 6e5f 7369 7a65 5f74 656e 736f  ag_on_size_tenso
+00005d10: 7228 6479 6e5f 7369 7a65 5f65 7874 2e70  r(dyn_size_ext.p
+00005d20: 6c61 6365 686f 6c64 6572 2c20 6261 7463  laceholder, batc
+00005d30: 683d 6261 7463 6829 0a20 2020 2020 2020  h=batch).       
+00005d40: 2073 616d 655f 6261 7365 5f65 7874 7261   same_base_extra
+00005d50: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
+00005d60: 6374 785b 2862 6174 6368 2c20 6374 7829  ctx[(batch, ctx)
+00005d70: 5d20 3d20 6469 6d5f 7461 670a 2020 2020  ] = dim_tag.    
+00005d80: 2020 2020 6469 6d5f 7461 672e 636f 6d70      dim_tag.comp
+00005d90: 6c65 7465 5f64 796e 5f73 697a 6528 7465  lete_dyn_size(te
+00005da0: 6d70 6c61 7465 5f6f 6e6c 793d 5472 7565  mplate_only=True
+00005db0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00005dc0: 2064 696d 5f74 6167 0a0a 2020 2020 6465   dim_tag..    de
+00005dd0: 6620 7265 7365 745f 6261 7463 685f 6374  f reset_batch_ct
+00005de0: 7828 7365 6c66 3a20 4469 6d29 3a0a 2020  x(self: Dim):.  
+00005df0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00005e00: 2020 466f 7220 7468 6520 7365 6c66 2069    For the self i
+00005e10: 6e73 7461 6e63 652c 2072 6573 6574 2062  nstance, reset b
+00005e20: 6174 6368 2061 6e64 2063 6f6e 7465 7874  atch and context
+00005e30: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00005e40: 2020 2020 2020 6966 2073 656c 662e 5f65        if self._e
+00005e50: 7874 7261 3a0a 2020 2020 2020 2020 2020  xtra:.          
+00005e60: 2020 7365 6c66 2e5f 6578 7472 612e 7361    self._extra.sa
+00005e70: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
+00005e80: 2e70 6f70 2828 7365 6c66 2e62 6174 6368  .pop((self.batch
+00005e90: 2c20 7365 6c66 2e63 6f6e 7472 6f6c 5f66  , self.control_f
+00005ea0: 6c6f 775f 6374 7829 2c20 4e6f 6e65 290a  low_ctx), None).
+00005eb0: 2020 2020 2020 2020 7365 6c66 2e62 6174          self.bat
+00005ec0: 6368 203d 204e 6f6e 650a 2020 2020 2020  ch = None.      
+00005ed0: 2020 7365 6c66 2e63 6f6e 7472 6f6c 5f66    self.control_f
+00005ee0: 6c6f 775f 6374 7820 3d20 4e6f 6e65 0a20  low_ctx = None. 
+00005ef0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+00005f00: 796e 5f73 697a 655f 6578 7420 616e 6420  yn_size_ext and 
+00005f10: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00005f20: 742e 6261 7463 683a 0a20 2020 2020 2020  t.batch:.       
+00005f30: 2020 2020 2073 656c 662e 6479 6e5f 7369       self.dyn_si
+00005f40: 7a65 5f65 7874 203d 2073 656c 662e 6479  ze_ext = self.dy
+00005f50: 6e5f 7369 7a65 5f65 7874 2e63 6f70 795f  n_size_ext.copy_
+00005f60: 7465 6d70 6c61 7465 2829 0a20 2020 2020  template().     
+00005f70: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
+00005f80: 7369 7a65 5f65 7874 2e62 6174 6368 203d  size_ext.batch =
+00005f90: 204e 6f6e 650a 0a20 2020 2064 6566 2073   None..    def s
+00005fa0: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
+00005fb0: 666f 725f 6261 7463 685f 6374 7828 7365  for_batch_ctx(se
+00005fc0: 6c66 2c20 6261 7463 682c 2063 7478 2c20  lf, batch, ctx, 
+00005fd0: 6479 6e5f 7369 7a65 5f65 7874 293a 0a20  dyn_size_ext):. 
+00005fe0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005ff0: 2020 203a 7061 7261 6d20 4261 7463 6849     :param BatchI
+00006000: 6e66 6f20 6261 7463 683a 0a20 2020 2020  nfo batch:.     
+00006010: 2020 203a 7061 7261 6d20 436f 6e74 726f     :param Contro
+00006020: 6c46 6c6f 7743 6f6e 7465 7874 7c4e 6f6e  lFlowContext|Non
+00006030: 6520 6374 783a 0a20 2020 2020 2020 203a  e ctx:.        :
+00006040: 7061 7261 6d20 4461 7461 2064 796e 5f73  param Data dyn_s
+00006050: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
+00006060: 2022 2222 0a20 2020 2020 2020 2061 7373   """.        ass
+00006070: 6572 7420 7365 6c66 2e63 616e 5f62 655f  ert self.can_be_
+00006080: 7573 6564 5f61 735f 6469 6d28 290a 2020  used_as_dim().  
+00006090: 2020 2020 2020 7361 6d65 203d 2073 656c        same = sel
+000060a0: 662e 6765 745f 666f 725f 6261 7463 685f  f.get_for_batch_
+000060b0: 6374 7828 6261 7463 682c 2063 7478 290a  ctx(batch, ctx).
+000060c0: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
+000060d0: 796e 5f73 697a 655f 6578 742e 6261 7463  yn_size_ext.batc
+000060e0: 6820 3d3d 2062 6174 6368 2061 6e64 2064  h == batch and d
+000060f0: 796e 5f73 697a 655f 6578 742e 636f 6e74  yn_size_ext.cont
+00006100: 726f 6c5f 666c 6f77 5f63 7478 203d 3d20  rol_flow_ctx == 
+00006110: 6374 780a 2020 2020 2020 2020 6966 2073  ctx.        if s
+00006120: 616d 652e 6479 6e5f 7369 7a65 5f65 7874  ame.dyn_size_ext
+00006130: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
+00006140: 7365 7274 2073 616d 652e 6479 6e5f 7369  sert same.dyn_si
+00006150: 7a65 5f65 7874 2e64 696d 5f74 6167 7320  ze_ext.dim_tags 
+00006160: 3d3d 2064 796e 5f73 697a 655f 6578 742e  == dyn_size_ext.
+00006170: 6469 6d5f 7461 6773 0a20 2020 2020 2020  dim_tags.       
+00006180: 2020 2020 2069 6620 6479 6e5f 7369 7a65       if dyn_size
+00006190: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
+000061a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000061b0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+000061c0: 6d65 2e64 796e 5f73 697a 655f 6578 742e  me.dyn_size_ext.
+000061d0: 706c 6163 6568 6f6c 6465 7220 3d20 6479  placeholder = dy
+000061e0: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
+000061f0: 686f 6c64 6572 0a20 2020 2020 2020 2065  holder.        e
+00006200: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00006210: 2073 616d 652e 6479 6e5f 7369 7a65 5f65   same.dyn_size_e
+00006220: 7874 203d 2064 796e 5f73 697a 655f 6578  xt = dyn_size_ex
+00006230: 740a 2020 2020 2020 2020 7365 6c66 2e5f  t.        self._
+00006240: 6d61 7962 655f 7570 6461 7465 2829 0a0a  maybe_update()..
+00006250: 2020 2020 6465 6620 6765 745f 6479 6e5f      def get_dyn_
+00006260: 7369 7a65 5f65 7874 5f66 6f72 5f62 6174  size_ext_for_bat
+00006270: 6368 5f63 7478 2873 656c 662c 2062 6174  ch_ctx(self, bat
+00006280: 6368 2c20 6374 782c 2074 656d 706c 6174  ch, ctx, templat
+00006290: 655f 6f6e 6c79 3d46 616c 7365 293a 0a20  e_only=False):. 
+000062a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000062b0: 2020 203a 7061 7261 6d20 4261 7463 6849     :param BatchI
+000062c0: 6e66 6f7c 4e6f 6e65 2062 6174 6368 3a0a  nfo|None batch:.
+000062d0: 2020 2020 2020 2020 3a70 6172 616d 2043          :param C
+000062e0: 6f6e 7472 6f6c 466c 6f77 436f 6e74 6578  ontrolFlowContex
+000062f0: 747c 4e6f 6e65 2063 7478 3a0a 2020 2020  t|None ctx:.    
+00006300: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
+00006310: 7465 6d70 6c61 7465 5f6f 6e6c 793a 0a20  template_only:. 
+00006320: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+00006330: 6174 617c 4e6f 6e65 0a20 2020 2020 2020  ata|None.       
+00006340: 2022 2222 0a20 2020 2020 2020 2061 7373   """.        ass
+00006350: 6572 7420 7365 6c66 2e63 616e 5f62 655f  ert self.can_be_
+00006360: 7573 6564 5f61 735f 6469 6d28 290a 2020  used_as_dim().  
+00006370: 2020 2020 2020 6966 206e 6f74 2062 6174        if not bat
+00006380: 6368 2061 6e64 2073 656c 662e 6261 7463  ch and self.batc
+00006390: 683a 0a20 2020 2020 2020 2020 2020 2023  h:.            #
+000063a0: 2041 7373 756d 6520 676c 6f62 616c 2062   Assume global b
+000063b0: 6174 6368 2e0a 2020 2020 2020 2020 2020  atch..          
+000063c0: 2020 6261 7463 6820 3d20 7365 6c66 2e62    batch = self.b
+000063d0: 6174 6368 2e67 6574 5f67 6c6f 6261 6c5f  atch.get_global_
+000063e0: 6261 7365 2829 0a20 2020 2020 2020 2069  base().        i
+000063f0: 6620 6e6f 7420 6261 7463 683a 0a20 2020  f not batch:.   
+00006400: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
+00006410: 6973 2075 7375 616c 6c79 206e 6f74 2076  is usually not v
+00006420: 616c 6964 2e20 486f 7765 7665 722c 2074  alid. However, t
+00006430: 6869 7320 6361 7365 2063 616e 2068 6170  his case can hap
+00006440: 7065 6e20 6561 726c 7920 6174 2069 6e69  pen early at ini
+00006450: 7469 616c 697a 6174 696f 6e2e 0a20 2020  tialization..   
+00006460: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00006470: 6261 7463 6820 3d3d 2073 656c 662e 6261  batch == self.ba
+00006480: 7463 6820 616e 6420 6374 7820 3d3d 2073  tch and ctx == s
+00006490: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
+000064a0: 5f63 7478 0a20 2020 2020 2020 2020 2020  _ctx.           
+000064b0: 2072 6574 7572 6e20 7365 6c66 2e64 796e   return self.dyn
+000064c0: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
+000064d0: 2020 7361 6d65 203d 2073 656c 662e 6765    same = self.ge
+000064e0: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
+000064f0: 6261 7463 682c 2063 7478 2c20 616c 6c6f  batch, ctx, allo
+00006500: 775f 6e6f 6e65 3d54 7275 6529 0a20 2020  w_none=True).   
+00006510: 2020 2020 2069 6620 6e6f 7420 7361 6d65       if not same
+00006520: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00006530: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
+00006540: 2020 7361 6d65 2e63 6f6d 706c 6574 655f    same.complete_
+00006550: 6479 6e5f 7369 7a65 2874 656d 706c 6174  dyn_size(templat
+00006560: 655f 6f6e 6c79 3d74 656d 706c 6174 655f  e_only=template_
+00006570: 6f6e 6c79 290a 2020 2020 2020 2020 7265  only).        re
+00006580: 7475 726e 2073 616d 652e 6479 6e5f 7369  turn same.dyn_si
+00006590: 7a65 5f65 7874 0a0a 2020 2020 4070 726f  ze_ext..    @pro
+000065a0: 7065 7274 790a 2020 2020 6465 6620 6479  perty.    def dy
+000065b0: 6e5f 7369 7a65 2873 656c 6629 3a0a 2020  n_size(self):.  
+000065c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000065d0: 2020 3a72 6574 7572 6e3a 2064 796e 2073    :return: dyn s
+000065e0: 697a 6520 2f20 7365 7120 6c65 6e20 2875  ize / seq len (u
+000065f0: 7375 616c 6c79 206f 6620 7368 6170 6520  sually of shape 
+00006600: 5b42 5d29 2c20 6f72 204e 6f6e 650a 2020  [B]), or None.  
+00006610: 2020 2020 2020 2020 4966 2074 6865 2064          If the d
+00006620: 796e 2073 697a 6520 6361 6e20 706f 7465  yn size can pote
+00006630: 6e74 6961 6c6c 7920 6265 206f 6620 6120  ntially be of a 
+00006640: 6469 6666 6572 656e 7420 7368 6170 652c  different shape,
+00006650: 2064 6972 6563 746c 7920 6163 6365 7373   directly access
+00006660: 2064 796e 5f73 697a 655f 6578 742e 0a20   dyn_size_ext.. 
+00006670: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
+00006680: 662e 5465 6e73 6f72 7c4e 6f6e 650a 2020  f.Tensor|None.  
+00006690: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000066a0: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
+000066b0: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
+000066c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000066d0: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
+000066e0: 6365 686f 6c64 6572 0a20 2020 2020 2020  ceholder.       
+000066f0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00006700: 2020 4064 796e 5f73 697a 652e 7365 7474    @dyn_size.sett
+00006710: 6572 0a20 2020 2064 6566 2064 796e 5f73  er.    def dyn_s
+00006720: 697a 6528 7365 6c66 2c20 6479 6e5f 7369  ize(self, dyn_si
+00006730: 7a65 293a 0a20 2020 2020 2020 2022 2222  ze):.        """
+00006740: 0a20 2020 2020 2020 2041 6c73 6f20 7365  .        Also se
+00006750: 6520 3a66 756e 633a 6073 6574 5f64 796e  e :func:`set_dyn
+00006760: 5f73 697a 655f 6578 745f 666f 725f 6261  _size_ext_for_ba
+00006770: 7463 685f 6374 7860 2e0a 0a20 2020 2020  tch_ctx`...     
+00006780: 2020 203a 7061 7261 6d20 7466 2e54 656e     :param tf.Ten
+00006790: 736f 7220 6479 6e5f 7369 7a65 3a0a 2020  sor dyn_size:.  
+000067a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000067b0: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
+000067c0: 7a65 5f65 7874 2061 6e64 2073 656c 662e  ze_ext and self.
+000067d0: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
+000067e0: 6365 686f 6c64 6572 2069 7320 6479 6e5f  ceholder is dyn_
+000067f0: 7369 7a65 3a20 2023 2066 6173 7420 7061  size:  # fast pa
+00006800: 7468 2063 6865 636b 0a20 2020 2020 2020  th check.       
+00006810: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00006820: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
+00006830: 6361 6e5f 6265 5f75 7365 645f 6173 5f64  can_be_used_as_d
+00006840: 696d 2829 0a20 2020 2020 2020 206f 7468  im().        oth
+00006850: 6572 203d 205f 642e 4469 6d2e 6765 745f  er = _d.Dim.get_
+00006860: 7461 675f 6672 6f6d 5f73 697a 655f 7465  tag_from_size_te
+00006870: 6e73 6f72 2864 796e 5f73 697a 6529 0a20  nsor(dyn_size). 
+00006880: 2020 2020 2020 2069 6620 6f74 6865 723a         if other:
+00006890: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000068a0: 662e 6465 636c 6172 655f 7361 6d65 5f61  f.declare_same_a
+000068b0: 7328 6f74 6865 7229 0a20 2020 2020 2020  s(other).       
+000068c0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
+000068d0: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
+000068e0: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
+000068f0: 6261 7463 6820 3d3d 206f 7468 6572 2e62  batch == other.b
+00006900: 6174 6368 2061 6e64 2073 656c 662e 636f  atch and self.co
+00006910: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
+00006920: 3d20 6f74 6865 722e 636f 6e74 726f 6c5f  = other.control_
+00006930: 666c 6f77 5f63 7478 0a20 2020 2020 2020  flow_ctx.       
+00006940: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00006950: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006960: 6261 7463 6820 3d20 6f74 6865 722e 6261  batch = other.ba
+00006970: 7463 680a 2020 2020 2020 2020 2020 2020  tch.            
+00006980: 2020 2020 7365 6c66 2e63 6f6e 7472 6f6c      self.control
+00006990: 5f66 6c6f 775f 6374 7820 3d20 6f74 6865  _flow_ctx = othe
+000069a0: 722e 636f 6e74 726f 6c5f 666c 6f77 5f63  r.control_flow_c
+000069b0: 7478 0a20 2020 2020 2020 2020 2020 2073  tx.            s
+000069c0: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+000069d0: 203d 206f 7468 6572 2e64 796e 5f73 697a   = other.dyn_siz
+000069e0: 655f 6578 740a 2020 2020 2020 2020 2020  e_ext.          
+000069f0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00006a00: 2073 656c 662e 5f69 6e69 745f 6465 6661   self._init_defa
+00006a10: 756c 745f 6479 6e5f 7369 7a65 5f65 7874  ult_dyn_size_ext
+00006a20: 2864 796e 5f73 697a 6529 0a20 2020 2020  (dyn_size).     
+00006a30: 2020 2073 656c 662e 7365 745f 7461 675f     self.set_tag_
+00006a40: 6f6e 5f73 697a 655f 7465 6e73 6f72 2864  on_size_tensor(d
+00006a50: 796e 5f73 697a 6529 0a0a 2020 2020 6465  yn_size)..    de
+00006a60: 6620 5f69 6e69 745f 6465 6661 756c 745f  f _init_default_
+00006a70: 6479 6e5f 7369 7a65 5f65 7874 2873 656c  dyn_size_ext(sel
+00006a80: 662c 2064 796e 5f73 697a 6529 3a0a 2020  f, dyn_size):.  
+00006a90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00006aa0: 2020 3a70 6172 616d 2074 662e 5465 6e73    :param tf.Tens
+00006ab0: 6f72 2064 796e 5f73 697a 653a 0a20 2020  or dyn_size:.   
+00006ac0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00006ad0: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
+00006ae0: 655f 6578 743a 0a20 2020 2020 2020 2020  e_ext:.         
+00006af0: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
+00006b00: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
+00006b10: 6465 7220 6973 206e 6f74 204e 6f6e 653a  der is not None:
+00006b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006b30: 2023 2044 6f20 6e6f 7420 616c 6c6f 7720   # Do not allow 
+00006b40: 7265 7365 7474 696e 6720 6974 2074 6f20  resetting it to 
+00006b50: 7374 6820 6469 6666 6572 656e 742e 0a20  sth different.. 
+00006b60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00006b70: 7373 6572 7420 7365 6c66 2e64 796e 5f73  ssert self.dyn_s
+00006b80: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
+00006b90: 6465 7220 6973 2064 796e 5f73 697a 650a  der is dyn_size.
+00006ba0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00006bb0: 2020 2020 2020 2020 2020 6265 616d 203d            beam =
+00006bc0: 2067 6574 6174 7472 2864 796e 5f73 697a   getattr(dyn_siz
+00006bd0: 652c 2022 5f52 4554 5552 4e4e 5f64 796e  e, "_RETURNN_dyn
+00006be0: 5f73 697a 655f 6265 616d 222c 204e 6f6e  _size_beam", Non
+00006bf0: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+00006c00: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00006c10: 203d 205f 742e 5465 6e73 6f72 280a 2020   = _t.Tensor(.  
+00006c20: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+00006c30: 6d65 3d28 2225 733a 6479 6e5f 7369 7a65  me=("%s:dyn_size
+00006c40: 2220 2520 7365 6c66 2e64 6573 6372 6970  " % self.descrip
+00006c50: 7469 6f6e 2920 6966 2073 656c 662e 6465  tion) if self.de
+00006c60: 7363 7269 7074 696f 6e20 656c 7365 2064  scription else d
+00006c70: 796e 5f73 697a 652e 6f70 2e6e 616d 652c  yn_size.op.name,
+00006c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c90: 2064 7479 7065 3d5f 742e 5465 6e73 6f72   dtype=_t.Tensor
+00006ca0: 2e73 697a 655f 6474 7970 652c 0a20 2020  .size_dtype,.   
+00006cb0: 2020 2020 2020 2020 2020 2020 2073 6861               sha
+00006cc0: 7065 3d28 292c 0a20 2020 2020 2020 2020  pe=(),.         
+00006cd0: 2020 2020 2020 2062 6174 6368 5f64 696d         batch_dim
+00006ce0: 5f61 7869 733d 302c 0a20 2020 2020 2020  _axis=0,.       
+00006cf0: 2020 2020 2020 2020 2062 6174 6368 3d73           batch=s
+00006d00: 656c 662e 6261 7463 682c 0a20 2020 2020  elf.batch,.     
+00006d10: 2020 2020 2020 2020 2020 2062 6561 6d3d             beam=
+00006d20: 6265 616d 2c0a 2020 2020 2020 2020 2020  beam,.          
+00006d30: 2020 2020 2020 636f 6e74 726f 6c5f 666c        control_fl
+00006d40: 6f77 5f63 7478 3d73 656c 662e 636f 6e74  ow_ctx=self.cont
+00006d50: 726f 6c5f 666c 6f77 5f63 7478 2c0a 2020  rol_flow_ctx,.  
+00006d60: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00006d70: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
+00006d80: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
+00006d90: 7220 3d20 6479 6e5f 7369 7a65 0a0a 2020  r = dyn_size..  
+00006da0: 2020 6465 6620 6765 745f 6d61 736b 2873    def get_mask(s
+00006db0: 656c 663a 2044 696d 2c20 2a2c 2064 696d  elf: Dim, *, dim
+00006dc0: 5f6f 7264 6572 3a20 4f70 7469 6f6e 616c  _order: Optional
+00006dd0: 5b53 6571 7565 6e63 655b 4469 6d5d 5d20  [Sequence[Dim]] 
+00006de0: 3d20 4e6f 6e65 2920 2d3e 205f 742e 5465  = None) -> _t.Te
+00006df0: 6e73 6f72 3a0a 2020 2020 2020 2020 2222  nsor:.        ""
+00006e00: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+00006e10: 2064 696d 5f6f 7264 6572 3a20 6966 2067   dim_order: if g
+00006e20: 6976 656e 2c20 7468 6520 6469 6d73 206f  iven, the dims o
+00006e30: 6620 7468 6520 6d61 736b 2077 696c 6c20  f the mask will 
+00006e40: 6265 2069 6e20 7468 6973 206f 7264 6572  be in this order
+00006e50: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00006e60: 6973 2063 616e 2062 6520 7573 6566 756c  is can be useful
+00006e70: 2069 6620 7468 6520 6d61 736b 2069 7320   if the mask is 
+00006e80: 6272 6f61 6463 6173 7465 6420 6167 6169  broadcasted agai
+00006e90: 6e73 7420 736f 6d65 206f 7468 6572 2074  nst some other t
+00006ea0: 656e 736f 722e 0a20 2020 2020 2020 203a  ensor..        :
+00006eb0: 7265 7475 726e 3a20 6966 206e 6565 645f  return: if need_
+00006ec0: 6d61 736b 696e 6728 292c 2074 6865 2063  masking(), the c
+00006ed0: 6f72 7265 7370 6f6e 6469 6e67 206d 6173  orresponding mas
+00006ee0: 6b2e 0a20 2020 2020 2020 2020 2020 2049  k..            I
+00006ef0: 6620 7468 6973 2069 7320 652e 672e 2074  f this is e.g. t
+00006f00: 6865 2074 696d 652d 6469 6d20 5420 6f66  he time-dim T of
+00006f10: 2073 6861 7065 205b 425d 2c20 7468 656e   shape [B], then
+00006f20: 2074 6865 206d 6173 6b20 7769 6c6c 2062   the mask will b
+00006f30: 6520 6f66 2073 6861 7065 205b 422c 545d  e of shape [B,T]
+00006f40: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00006f50: 6520 6d61 736b 2063 6f75 6c64 2062 6520  e mask could be 
+00006f60: 7573 6564 2077 6974 6820 3a66 756e 633a  used with :func:
+00006f70: 606d 6173 6b65 645f 7365 6c65 6374 6020  `masked_select` 
+00006f80: 2860 6062 6f6f 6c65 616e 5f6d 6173 6b60  (``boolean_mask`
+00006f90: 6029 206f 7220 6060 7768 6572 6560 602e  `) or ``where``.
+00006fa0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006fb0: 2020 2020 2069 6d70 6f72 7420 7265 7475       import retu
+00006fc0: 726e 6e2e 6672 6f6e 7465 6e64 2061 7320  rnn.frontend as 
+00006fd0: 7266 0a0a 2020 2020 2020 2020 6173 7365  rf..        asse
+00006fe0: 7274 2073 656c 662e 6479 6e5f 7369 7a65  rt self.dyn_size
+00006ff0: 5f65 7874 2061 6e64 2073 656c 662e 6479  _ext and self.dy
+00007000: 6e5f 7369 7a65 5f65 7874 2e72 6177 5f74  n_size_ext.raw_t
+00007010: 656e 736f 7220 6973 206e 6f74 204e 6f6e  ensor is not Non
+00007020: 650a 2020 2020 2020 2020 2320 6e6f 696e  e.        # noin
+00007030: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+00007040: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+00007050: 2020 2062 6163 6b65 6e64 203d 2073 656c     backend = sel
+00007060: 662e 6479 6e5f 7369 7a65 5f65 7874 2e5f  f.dyn_size_ext._
+00007070: 7261 775f 6261 636b 656e 640a 0a20 2020  raw_backend..   
+00007080: 2020 2020 206d 6178 5f69 6478 203d 2072       max_idx = r
+00007090: 662e 7265 6475 6365 280a 2020 2020 2020  f.reduce(.      
+000070a0: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
+000070b0: 697a 655f 6578 742c 0a20 2020 2020 2020  ize_ext,.       
+000070c0: 2020 2020 2061 7869 733d 7365 6c66 2e64       axis=self.d
+000070d0: 796e 5f73 697a 655f 6578 742e 6469 6d73  yn_size_ext.dims
+000070e0: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
+000070f0: 6465 3d22 6d61 7822 2c0a 2020 2020 2020  de="max",.      
+00007100: 2020 2020 2020 2320 4d61 736b 696e 6720        # Masking 
+00007110: 6865 7265 2069 7320 6e6f 7420 616c 7761  here is not alwa
+00007120: 7973 2070 6f73 7369 626c 652c 2065 2e67  ys possible, e.g
+00007130: 2e20 6966 2077 6520 6861 7665 0a20 2020  . if we have.   
+00007140: 2020 2020 2020 2020 2023 2074 6167 203d           # tag =
+00007150: 2044 696d 7b27 7365 6c66 2d61 7474 2d6b   Dim{'self-att-k
+00007160: 6579 7327 5b27 7469 6d65 3a76 6172 3a65  eys'['time:var:e
+00007170: 7874 6572 6e5f 6461 7461 3a63 6c61 7373  xtern_data:class
+00007180: 6573 275b 425d 5d7d 0a20 2020 2020 2020  es'[B]]}.       
+00007190: 2020 2020 2075 7365 5f6d 6173 6b3d 4661       use_mask=Fa
+000071a0: 6c73 652c 0a20 2020 2020 2020 2029 0a20  lse,.        ). 
+000071b0: 2020 2020 2020 2023 2057 6520 7573 6520         # We use 
+000071c0: 7468 6520 6173 7375 6d70 7469 6f6e 2074  the assumption t
+000071d0: 6861 7420 7365 6c66 2e70 6c61 6365 686f  hat self.placeho
+000071e0: 6c64 6572 2e73 6861 7065 5b61 7869 735d  lder.shape[axis]
+000071f0: 203d 3d20 6d61 785f 6964 782e 0a20 2020   == max_idx..   
+00007200: 2020 2020 2023 2073 697a 655f 6578 7420       # size_ext 
+00007210: 6d69 6768 7420 6861 7665 2069 6e76 616c  might have inval
+00007220: 6964 2028 7a65 726f 2920 7369 7a65 730a  id (zero) sizes.
+00007230: 2020 2020 2020 2020 2320 7768 656e 2069          # when i
+00007240: 7420 6974 7365 6c66 2068 6173 2073 6f6d  t itself has som
+00007250: 6520 7061 6464 696e 672c 2065 2e67 2e20  e padding, e.g. 
+00007260: 7768 656e 2069 7473 206f 776e 2073 6861  when its own sha
+00007270: 7065 2069 7320 6479 6e61 6d69 632e 0a20  pe is dynamic.. 
+00007280: 2020 2020 2020 2023 2041 207a 6572 6f20         # A zero 
+00007290: 7369 7a65 2063 616e 206c 6561 6420 746f  size can lead to
+000072a0: 2070 726f 626c 656d 7320 696e 2073 6f6d   problems in som
+000072b0: 6520 6361 7365 732c 2065 2e67 2e20 696e  e cases, e.g. in
+000072c0: 2053 6f66 746d 6178 4f76 6572 5370 6174   SoftmaxOverSpat
+000072d0: 6961 6c4c 6179 6572 2c0a 2020 2020 2020  ialLayer,.      
+000072e0: 2020 2320 7768 656e 2065 7665 7279 7468    # when everyth
+000072f0: 696e 6720 6973 206d 6173 6b65 6420 746f  ing is masked to
+00007300: 202d 696e 662c 2069 7420 7265 7375 6c74   -inf, it result
+00007310: 7320 696e 206e 616e 2c0a 2020 2020 2020  s in nan,.      
+00007320: 2020 2320 616e 6420 7468 6973 206c 696b    # and this lik
+00007330: 656c 7920 7072 6f64 7563 6573 206e 616e  ely produces nan
+00007340: 2069 6e20 6261 636b 7072 6f70 206f 7220   in backprop or 
+00007350: 656c 7365 7768 6572 652e 0a20 2020 2020  elsewhere..     
+00007360: 2020 2023 2054 6875 732c 206d 6173 6b20     # Thus, mask 
+00007370: 7369 7a65 5f65 7874 2069 7473 656c 662c  size_ext itself,
+00007380: 2061 6e64 2073 6574 2074 6865 2070 6164   and set the pad
+00007390: 6465 6420 7661 6c75 6573 2074 6f20 312e  ded values to 1.
+000073a0: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+000073b0: 6173 7375 6d65 7320 7468 6174 206d 6178  assumes that max
+000073c0: 5f69 6478 203e 3d20 312e 0a20 2020 2020  _idx >= 1..     
+000073d0: 2020 2073 697a 655f 6578 7420 3d20 7365     size_ext = se
+000073e0: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
+000073f0: 636f 7079 5f6d 6173 6b65 6428 6d61 785f  copy_masked(max_
+00007400: 6964 7829 0a20 2020 2020 2020 2069 6478  idx).        idx
+00007410: 5f72 616e 6765 203d 2062 6163 6b65 6e64  _range = backend
+00007420: 2e72 616e 6765 5f6f 7665 725f 6469 6d28  .range_over_dim(
+00007430: 7365 6c66 290a 2020 2020 2020 2020 7365  self).        se
+00007440: 715f 6d61 736b 203d 2072 662e 636f 6d70  q_mask = rf.comp
+00007450: 6172 6528 6964 785f 7261 6e67 652c 2022  are(idx_range, "
+00007460: 3c22 2c20 7369 7a65 5f65 7874 2c20 616c  <", size_ext, al
+00007470: 6c6f 775f 6272 6f61 6463 6173 745f 616c  low_broadcast_al
+00007480: 6c5f 736f 7572 6365 733d 5472 7565 2c20  l_sources=True, 
+00007490: 6469 6d5f 6f72 6465 723d 6469 6d5f 6f72  dim_order=dim_or
+000074a0: 6465 7229 0a20 2020 2020 2020 2072 6574  der).        ret
+000074b0: 7572 6e20 7365 715f 6d61 736b 0a0a 2020  urn seq_mask..  
+000074c0: 2020 6465 6620 6973 5f62 6174 6368 5f64    def is_batch_d
+000074d0: 696d 2873 656c 6629 3a0a 2020 2020 2020  im(self):.      
+000074e0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+000074f0: 6574 7572 6e3a 2077 6865 7468 6572 2074  eturn: whether t
+00007500: 6869 7320 6469 6d20 7461 6720 6973 206f  his dim tag is o
+00007510: 6620 6b69 6e64 2062 6174 6368 0a20 2020  f kind batch.   
+00007520: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+00007530: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
+00007540: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00007550: 662e 6b69 6e64 203d 3d20 4469 6d54 7970  f.kind == DimTyp
+00007560: 6573 2e42 6174 6368 0a0a 2020 2020 6465  es.Batch..    de
+00007570: 6620 6973 5f66 6561 7475 7265 5f64 696d  f is_feature_dim
+00007580: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007590: 2222 220a 2020 2020 2020 2020 3a72 6574  """.        :ret
+000075a0: 7572 6e3a 2077 6865 7468 6572 2074 6869  urn: whether thi
+000075b0: 7320 6469 6d20 7461 6720 6973 206f 6620  s dim tag is of 
+000075c0: 6b69 6e64 2066 6561 7475 7265 0a20 2020  kind feature.   
+000075d0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+000075e0: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
+000075f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00007600: 662e 6b69 6e64 203d 3d20 4469 6d54 7970  f.kind == DimTyp
+00007610: 6573 2e46 6561 7475 7265 0a0a 2020 2020  es.Feature..    
+00007620: 6465 6620 6973 5f73 7061 7469 616c 5f64  def is_spatial_d
+00007630: 696d 2873 656c 6629 3a0a 2020 2020 2020  im(self):.      
+00007640: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00007650: 6574 7572 6e3a 2077 6865 7468 6572 2074  eturn: whether t
+00007660: 6869 7320 6469 6d20 7461 6720 6973 206f  his dim tag is o
+00007670: 6620 6b69 6e64 2073 7061 7469 616c 0a20  f kind spatial. 
+00007680: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
+00007690: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
+000076a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000076b0: 656c 662e 6b69 6e64 203d 3d20 4469 6d54  elf.kind == DimT
+000076c0: 7970 6573 2e53 7061 7469 616c 0a0a 2020  ypes.Spatial..  
+000076d0: 2020 6465 6620 6973 5f64 696d 5f6b 6e6f    def is_dim_kno
+000076e0: 776e 2873 656c 6629 3a0a 2020 2020 2020  wn(self):.      
+000076f0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00007700: 6574 7572 6e3a 2077 6865 7468 6572 2077  eturn: whether w
+00007710: 6520 6b6e 6f77 2074 6865 2064 696d 656e  e know the dimen
+00007720: 7369 6f6e 3b20 6261 7369 6361 6c6c 7920  sion; basically 
+00007730: 7768 6574 6865 7220 7468 6973 2069 7320  whether this is 
+00007740: 6465 6669 6e65 640a 2020 2020 2020 2020  defined.        
+00007750: 2020 2861 6c74 686f 7567 6820 606e 6f74    (although `not
+00007760: 2073 656c 662e 756e 6465 6669 6e65 6460   self.undefined`
+00007770: 2069 7320 6465 6669 6e65 6420 736c 6967   is defined slig
+00007780: 6874 6c79 2064 6966 6665 7265 6e74 6c79  htly differently
+00007790: 290a 2020 2020 2020 2020 3a72 7479 7065  ).        :rtype
+000077a0: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
+000077b0: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+000077c0: 6c66 2e69 735f 6261 7463 685f 6469 6d28  lf.is_batch_dim(
+000077d0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+000077e0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+000077f0: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
+00007800: 735f 6479 6e61 6d69 6328 2920 616e 6420  s_dynamic() and 
+00007810: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
+00007820: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00007830: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00007840: 7275 650a 2020 2020 2020 2020 6966 2073  rue.        if s
+00007850: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00007860: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00007870: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+00007880: 2020 6578 7472 6120 3d20 7365 6c66 2e5f    extra = self._
+00007890: 6765 745f 7361 6d65 5f62 6173 655f 6578  get_same_base_ex
+000078a0: 7472 6128 290a 2020 2020 2020 2020 6966  tra().        if
+000078b0: 2065 7874 7261 3a0a 2020 2020 2020 2020   extra:.        
+000078c0: 2020 2020 666f 7220 5f2c 206f 7468 6572      for _, other
+000078d0: 2069 6e20 6578 7472 612e 7361 6d65 5f66   in extra.same_f
+000078e0: 6f72 5f62 6174 6368 5f63 7478 2e69 7465  or_batch_ctx.ite
+000078f0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+00007900: 2020 2020 2020 6966 206f 7468 6572 2e64        if other.d
+00007910: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
+00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007930: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00007940: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00007950: 650a 0a20 2020 2064 6566 2069 735f 6479  e..    def is_dy
+00007960: 6e61 6d69 6328 7365 6c66 2920 2d3e 2062  namic(self) -> b
+00007970: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+00007980: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00007990: 3a20 7768 6574 6865 7220 7468 6520 6469  : whether the di
+000079a0: 6d20 6973 206e 6f74 2073 7461 7469 632e  m is not static.
+000079b0: 2075 7375 616c 6c79 206d 6561 6e73 2074   usually means t
+000079c0: 6861 7420 6974 2068 6173 2073 6571 206c  hat it has seq l
+000079d0: 656e 6774 6873 0a20 2020 2020 2020 2022  engths.        "
+000079e0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+000079f0: 6e20 7365 6c66 2e64 696d 656e 7369 6f6e  n self.dimension
+00007a00: 2069 7320 4e6f 6e65 2061 6e64 206e 6f74   is None and not
+00007a10: 2073 656c 662e 6973 5f62 6174 6368 5f64   self.is_batch_d
+00007a20: 696d 2829 0a0a 2020 2020 6465 6620 6973  im()..    def is
+00007a30: 5f73 7461 7469 6328 7365 6c66 2920 2d3e  _static(self) ->
+00007a40: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
 00007a50: 2222 0a20 2020 2020 2020 203a 7265 7475  "".        :retu
-00007a60: 726e 3a20 7768 6574 6865 7220 6469 6d20  rn: whether dim 
-00007a70: 6973 2073 7461 7469 6320 6f72 2064 796e  is static or dyn
-00007a80: 616d 6963 2062 7574 2077 6974 6820 7363  amic but with sc
-00007a90: 616c 6172 2064 796e 5f73 697a 655f 6578  alar dyn_size_ex
-00007aa0: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
-00007ab0: 2020 2020 2020 6966 2073 656c 662e 6973        if self.is
-00007ac0: 5f73 7461 7469 6328 293a 0a20 2020 2020  _static():.     
-00007ad0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00007ae0: 6170 6163 6974 7920 6973 206e 6f74 204e  apacity is not N
-00007af0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00007b00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00007b10: 2e73 697a 6520 3c20 7365 6c66 2e63 6170  .size < self.cap
-00007b20: 6163 6974 790a 2020 2020 2020 2020 2020  acity.          
-00007b30: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-00007b40: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00007b50: 6170 6163 6974 7920 6973 206e 6f74 204e  apacity is not N
-00007b60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00007b70: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-00007b80: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00007b90: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
-00007ba0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00007bb0: 6e20 5472 7565 2020 2320 756e 6b6e 6f77  n True  # unknow
-00007bc0: 6e0a 2020 2020 2020 2020 7265 7475 726e  n.        return
-00007bd0: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00007be0: 7874 2e62 6174 6368 5f6e 6469 6d20 3e20  xt.batch_ndim > 
-00007bf0: 300a 0a20 2020 2064 6566 2063 616e 5f62  0..    def can_b
-00007c00: 655f 7573 6564 5f61 735f 6469 6d28 7365  e_used_as_dim(se
-00007c10: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00007c20: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00007c30: 3a20 7768 6574 6865 7220 7468 6973 2063  : whether this c
-00007c40: 616e 2062 6520 7573 6564 2061 7320 6120  an be used as a 
-00007c50: 6469 6d20 696e 203a 636c 6173 733a 6044  dim in :class:`D
-00007c60: 6174 6160 2c20 692e 652e 2069 7420 6973  ata`, i.e. it is
-00007c70: 206e 6f74 2073 7065 6369 616c 0a20 2020   not special.   
-00007c80: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00007c90: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-00007ca0: 2020 2020 2020 7265 7475 726e 206e 6f74        return not
-00007cb0: 2073 656c 662e 7370 6563 6961 6c0a 0a20   self.special.. 
-00007cc0: 2020 2064 6566 2069 735f 7361 6d65 5f73     def is_same_s
-00007cd0: 697a 655f 7465 6e73 6f72 2873 656c 662c  ize_tensor(self,
-00007ce0: 2078 293a 0a20 2020 2020 2020 2022 2222   x):.        """
-00007cf0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00007d00: 7466 2e54 656e 736f 7220 783a 0a20 2020  tf.Tensor x:.   
-00007d10: 2020 2020 203a 7265 7475 726e 3a20 7768       :return: wh
-00007d20: 6574 6865 7220 7468 6973 2064 696d 2074  ether this dim t
-00007d30: 6167 2066 6f72 2074 6869 7320 7370 6563  ag for this spec
-00007d40: 6966 6963 2062 6174 6368 2028 696e 636c  ific batch (incl
-00007d50: 2062 6561 6d29 2069 7320 7468 6520 7361   beam) is the sa
-00007d60: 6d65 2061 7320 7468 6520 6769 7665 6e20  me as the given 
-00007d70: 7369 7a65 0a20 2020 2020 2020 203a 7274  size.        :rt
-00007d80: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
-00007d90: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00007da0: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00007db0: 7874 2061 6e64 2078 2069 7320 7365 6c66  xt and x is self
-00007dc0: 2e64 796e 5f73 697a 655f 6578 742e 706c  .dyn_size_ext.pl
-00007dd0: 6163 6568 6f6c 6465 723a 0a20 2020 2020  aceholder:.     
-00007de0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00007df0: 7565 0a20 2020 2020 2020 2074 6167 203d  ue.        tag =
-00007e00: 205f 4469 6d4d 6978 696e 2e67 6574 5f74   _DimMixin.get_t
-00007e10: 6167 5f66 726f 6d5f 7369 7a65 5f74 656e  ag_from_size_ten
-00007e20: 736f 7228 7829 0a20 2020 2020 2020 2069  sor(x).        i
-00007e30: 6620 7461 6720 616e 6420 7461 6720 3d3d  f tag and tag ==
-00007e40: 2073 656c 663a 0a20 2020 2020 2020 2020   self:.         
-00007e50: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00007e60: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00007e70: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
-00007e80: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00007e90: 6c73 650a 2020 2020 2020 2020 6966 2075  lse.        if u
-00007ea0: 7469 6c2e 5265 6649 6445 7128 7829 2069  til.RefIdEq(x) i
-00007eb0: 6e20 7365 6c66 2e5f 6578 7472 612e 6479  n self._extra.dy
-00007ec0: 6e5f 7369 7a65 5f73 616d 653a 0a20 2020  n_size_same:.   
-00007ed0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007ee0: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
-00007ef0: 7572 6e20 4661 6c73 650a 0a20 2020 2064  urn False..    d
-00007f00: 6566 2073 6574 5f74 6167 5f6f 6e5f 7369  ef set_tag_on_si
-00007f10: 7a65 5f74 656e 736f 7228 7365 6c66 3a20  ze_tensor(self: 
-00007f20: 4469 6d2c 2078 2c20 6261 7463 683d 4e6f  Dim, x, batch=No
-00007f30: 6e65 2c20 7361 6d65 5f61 735f 6265 666f  ne, same_as_befo
-00007f40: 7265 3d46 616c 7365 2920 2d3e 2044 696d  re=False) -> Dim
-00007f50: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00007f60: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
-00007f70: 696f 6e20 6973 2075 7365 640a 2020 2020  ion is used.    
-00007f80: 2020 2020 746f 2063 6f75 706c 6520 6120      to couple a 
-00007f90: 7466 2e54 656e 736f 7220 696e 7374 616e  tf.Tensor instan
-00007fa0: 6365 2072 6570 7265 7365 6e74 696e 6720  ce representing 
-00007fb0: 7468 6520 6479 6e20 7369 7a65 0a20 2020  the dyn size.   
-00007fc0: 2020 2020 2077 6974 6820 7468 6520 6469       with the di
-00007fd0: 6d20 7461 672e 0a0a 2020 2020 2020 2020  m tag...        
-00007fe0: 5468 6973 2069 7320 7573 7561 6c6c 7920  This is usually 
-00007ff0: 6120 6e65 776c 7920 6372 6561 7465 6420  a newly created 
-00008000: 6469 6d20 7461 672c 0a20 2020 2020 2020  dim tag,.       
-00008010: 2077 6869 6368 2069 7320 7965 7420 756e   which is yet un
-00008020: 7365 742e 0a0a 2020 2020 2020 2020 4974  set...        It
-00008030: 2069 7320 616c 736f 2075 7365 6420 746f   is also used to
-00008040: 2063 6f75 706c 6520 616e 2065 7869 7374   couple an exist
-00008050: 696e 6720 6469 6d20 7461 6720 7769 7468  ing dim tag with
-00008060: 206f 7468 6572 2064 796e 2073 697a 6573   other dyn sizes
-00008070: 0a20 2020 2020 2020 2077 6869 6368 206a  .        which j
-00008080: 7573 7420 6469 6666 6572 2062 7920 616e  ust differ by an
-00008090: 2065 7870 616e 7369 6f6e 206f 6620 7468   expansion of th
-000080a0: 6520 6261 7463 6820 2865 2e67 2e20 7365  e batch (e.g. se
-000080b0: 6172 6368 2062 6561 6d29 2e0a 0a20 2020  arch beam)...   
-000080c0: 2020 2020 2053 6565 2061 6c73 6f20 3a66       See also :f
-000080d0: 756e 633a 6067 6574 5f74 6167 5f66 726f  unc:`get_tag_fro
-000080e0: 6d5f 7369 7a65 5f74 656e 736f 7260 2e0a  m_size_tensor`..
-000080f0: 2020 2020 2020 2020 416c 736f 2073 6565          Also see
-00008100: 203a 6675 6e63 3a60 7365 745f 6479 6e5f   :func:`set_dyn_
-00008110: 7369 7a65 5f65 7874 5f66 6f72 5f62 6174  size_ext_for_bat
-00008120: 6368 5f63 7478 602e 0a0a 2020 2020 2020  ch_ctx`...      
-00008130: 2020 3a70 6172 616d 2078 3a20 7261 7720    :param x: raw 
-00008140: 7465 6e73 6f72 2c20 666f 7220 6578 616d  tensor, for exam
-00008150: 706c 6520 7466 2e54 656e 736f 720a 2020  ple tf.Tensor.  
-00008160: 2020 2020 2020 3a70 6172 616d 2042 6174        :param Bat
-00008170: 6368 496e 666f 7c4e 6f6e 6520 6261 7463  chInfo|None batc
-00008180: 683a 0a20 2020 2020 2020 203a 7061 7261  h:.        :para
-00008190: 6d20 626f 6f6c 2073 616d 655f 6173 5f62  m bool same_as_b
-000081a0: 6566 6f72 653a 2069 6d70 6c69 6573 2069  efore: implies i
-000081b0: 7420 7761 7320 7365 7420 6265 666f 7265  t was set before
-000081c0: 2c20 616e 6420 7468 6520 6e65 7720 7369  , and the new si
-000081d0: 7a65 2069 7320 7468 6520 7361 6d65 2e0a  ze is the same..
-000081e0: 2020 2020 2020 2020 2020 652e 672e 2069            e.g. i
-000081f0: 7420 636f 756c 6420 6265 2073 6f6d 6520  t could be some 
-00008200: 6964 656e 7469 7479 2077 6974 6820 6164  identity with ad
-00008210: 6465 6420 6368 6563 6b73 2c20 6f72 206f  ded checks, or o
-00008220: 7468 6572 2063 6861 6e67 652e 0a20 2020  ther change..   
-00008230: 2020 2020 203a 7265 7475 726e 3a20 7365       :return: se
-00008240: 6c66 206f 7220 6e65 7720 6469 6d20 7461  lf or new dim ta
-00008250: 670a 2020 2020 2020 2020 2222 220a 2020  g.        """.  
-00008260: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-00008270: 662e 6361 6e5f 6265 5f75 7365 645f 6173  f.can_be_used_as
-00008280: 5f64 696d 2829 0a20 2020 2020 2020 2023  _dim().        #
-00008290: 2049 7427 7320 756e 7573 7561 6c20 6966   It's unusual if
-000082a0: 2073 656c 662e 6469 6d65 6e73 696f 6e20   self.dimension 
-000082b0: 6973 206e 6f74 204e 6f6e 652c 2062 7574  is not None, but
-000082c0: 206c 6574 2773 2061 6363 6570 7420 7468   let's accept th
-000082d0: 6174 2e0a 2020 2020 2020 2020 6966 2068  at..        if h
-000082e0: 6173 6174 7472 2878 2c20 225f 6973 5f73  asattr(x, "_is_s
-000082f0: 697a 655f 6f66 5f64 696d 5f74 6167 2229  ize_of_dim_tag")
-00008300: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00008310: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
-00008320: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
-00008330: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00008340: 7420 782e 5f69 735f 7369 7a65 5f6f 665f  t x._is_size_of_
-00008350: 6469 6d5f 7461 6720 696e 2028 4e6f 6e65  dim_tag in (None
-00008360: 2c20 7365 6c66 290a 2020 2020 2020 2020  , self).        
-00008370: 2320 4966 2077 6520 616c 7265 6164 7920  # If we already 
-00008380: 6861 7665 2061 6e6f 7468 6572 2064 796e  have another dyn
-00008390: 2073 697a 6520 7365 7420 6f72 2064 6966   size set or dif
-000083a0: 6665 7265 6e74 2062 6174 6368 2c20 6372  ferent batch, cr
-000083b0: 6561 7465 2061 206e 6577 2044 696d 2069  eate a new Dim i
-000083c0: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
-000083d0: 2069 6620 7365 6c66 2e62 6174 6368 2061   if self.batch a
-000083e0: 6e64 2062 6174 6368 2061 6e64 2073 656c  nd batch and sel
-000083f0: 662e 6261 7463 6820 213d 2062 6174 6368  f.batch != batch
-00008400: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
-00008410: 7365 7274 206e 6f74 2073 616d 655f 6173  sert not same_as
-00008420: 5f62 6566 6f72 6520 2023 2069 7420 6361  _before  # it ca
-00008430: 6e6e 6f74 2062 6520 7468 6520 7361 6d65  nnot be the same
-00008440: 2077 6865 6e20 6974 2069 7320 616e 6f74   when it is anot
-00008450: 6865 7220 6261 7463 682e 2e2e 0a20 2020  her batch....   
-00008460: 2020 2020 2020 2020 206e 6577 5f64 696d           new_dim
-00008470: 5f74 6167 203d 2073 656c 662e 6765 745f  _tag = self.get_
-00008480: 666f 725f 6261 7463 685f 6374 7828 6261  for_batch_ctx(ba
-00008490: 7463 683d 6261 7463 682c 2063 7478 3d73  tch=batch, ctx=s
-000084a0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-000084b0: 5f63 7478 290a 2020 2020 2020 2020 2020  _ctx).          
-000084c0: 2020 6e65 775f 6469 6d5f 7461 672e 7365    new_dim_tag.se
-000084d0: 745f 7461 675f 6f6e 5f73 697a 655f 7465  t_tag_on_size_te
-000084e0: 6e73 6f72 2878 2c20 6261 7463 683d 6261  nsor(x, batch=ba
-000084f0: 7463 6829 0a20 2020 2020 2020 2020 2020  tch).           
-00008500: 2072 6574 7572 6e20 6e65 775f 6469 6d5f   return new_dim_
-00008510: 7461 670a 2020 2020 2020 2020 6966 2073  tag.        if s
-00008520: 656c 662e 6479 6e5f 7369 7a65 2069 7320  elf.dyn_size is 
-00008530: 6e6f 7420 4e6f 6e65 2061 6e64 2073 656c  not None and sel
-00008540: 662e 6479 6e5f 7369 7a65 2069 7320 6e6f  f.dyn_size is no
-00008550: 7420 783a 0a20 2020 2020 2020 2020 2020  t x:.           
-00008560: 2069 6620 7365 6c66 2e5f 6578 7472 6120   if self._extra 
-00008570: 616e 6420 7574 696c 2e52 6566 4964 4571  and util.RefIdEq
-00008580: 2878 2920 696e 2073 656c 662e 5f65 7874  (x) in self._ext
-00008590: 7261 2e64 796e 5f73 697a 655f 7361 6d65  ra.dyn_size_same
-000085a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000085b0: 2020 7061 7373 2020 2320 6f6b 2c20 7061    pass  # ok, pa
-000085c0: 7373 206f 6e0a 2020 2020 2020 2020 2020  ss on.          
-000085d0: 2020 656c 6966 2073 616d 655f 6173 5f62    elif same_as_b
-000085e0: 6566 6f72 653a 0a20 2020 2020 2020 2020  efore:.         
-000085f0: 2020 2020 2020 2073 656c 662e 5f6d 616b         self._mak
-00008600: 655f 6578 7472 6128 292e 6479 6e5f 7369  e_extra().dyn_si
-00008610: 7a65 5f73 616d 652e 6164 6428 7574 696c  ze_same.add(util
-00008620: 2e52 6566 4964 4571 2878 2929 0a20 2020  .RefIdEq(x)).   
-00008630: 2020 2020 2020 2020 2020 2020 2023 2041               # A
-00008640: 6e64 206e 6f77 2070 6173 7320 6f6e 2e0a  nd now pass on..
-00008650: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00008660: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008670: 2020 6173 7365 7274 2073 656c 662e 6261    assert self.ba
-00008680: 7463 6820 616e 6420 6261 7463 680a 2020  tch and batch.  
-00008690: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000086a0: 4974 2773 206e 6f74 2063 6c65 6172 2077  It's not clear w
-000086b0: 6861 7420 746f 2064 6f2e 2057 6520 636f  hat to do. We co
-000086c0: 756c 6420 6372 6561 7465 2061 206e 6577  uld create a new
-000086d0: 2064 696d 2074 6167 2c20 6275 7420 7468   dim tag, but th
-000086e0: 6520 7369 7a65 7320 6d69 6768 7420 6265  e sizes might be
-000086f0: 2064 6966 6665 7265 6e74 2e0a 2020 2020   different..    
-00008700: 2020 2020 2020 2020 2020 2020 2320 5573              # Us
-00008710: 7561 6c6c 7920 7765 2073 686f 756c 6420  ually we should 
-00008720: 6e6f 7420 6765 7420 6865 7265 2e0a 2020  not get here..  
-00008730: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00008740: 536f 2066 6f72 206e 6f77 2c20 6a75 7374  So for now, just
-00008750: 2065 7272 6f72 2e0a 2020 2020 2020 2020   error..        
-00008760: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
-00008770: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
-00008780: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
-00008790: 2020 2020 2020 2020 2066 726f 6d20 7265           from re
-000087a0: 7475 726e 6e2e 6672 6f6e 7465 6e64 2e5f  turnn.frontend._
-000087b0: 6261 636b 656e 6420 696d 706f 7274 2067  backend import g
-000087c0: 6574 5f62 6163 6b65 6e64 5f62 795f 7261  et_backend_by_ra
-000087d0: 775f 7465 6e73 6f72 5f74 7970 650a 0a20  w_tensor_type.. 
-000087e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000087f0: 6169 7365 2045 7863 6570 7469 6f6e 280a  aise Exception(.
-00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 2020 225c 6e22 2e6a 6f69 6e28 0a20      "\n".join(. 
-00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008830: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00008840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008850: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
-00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008870: 2020 2020 2020 2022 2572 2028 2572 2920         "%r (%r) 
-00008880: 616c 7265 6164 7920 6861 7320 7369 7a65  already has size
-00008890: 2025 722c 220a 2020 2020 2020 2020 2020   %r,".          
-000088a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088b0: 2020 2020 2020 2220 616e 6420 616e 6f74        " and anot
-000088c0: 6865 7220 696e 636f 6d70 6174 6962 6c65  her incompatible
-000088d0: 2073 697a 6520 2572 2028 6261 7463 6820   size %r (batch 
-000088e0: 2572 2920 6973 2062 6569 6e67 2061 7373  %r) is being ass
-000088f0: 6967 6e65 642e 220a 2020 2020 2020 2020  igned.".        
-00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008910: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 2520 2873 656c 662c 2073 656c 662e    % (self, self.
-00008940: 6465 7363 7269 7074 696f 6e2c 2073 656c  description, sel
-00008950: 662e 6479 6e5f 7369 7a65 2c20 782c 2062  f.dyn_size, x, b
-00008960: 6174 6368 292c 0a20 2020 2020 2020 2020  atch),.         
+00007a60: 726e 3a20 7374 6174 6963 0a20 2020 2020  rn: static.     
+00007a70: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00007a80: 6574 7572 6e20 6e6f 7420 7365 6c66 2e69  eturn not self.i
+00007a90: 735f 6479 6e61 6d69 6328 290a 0a20 2020  s_dynamic()..   
+00007aa0: 2064 6566 206e 6565 645f 6d61 736b 696e   def need_maskin
+00007ab0: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+00007ac0: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
+00007ad0: 7475 726e 3a20 7768 6574 6865 7220 6469  turn: whether di
+00007ae0: 6d20 6973 2073 7461 7469 6320 6f72 2064  m is static or d
+00007af0: 796e 616d 6963 2062 7574 2077 6974 6820  ynamic but with 
+00007b00: 7363 616c 6172 2064 796e 5f73 697a 655f  scalar dyn_size_
+00007b10: 6578 740a 2020 2020 2020 2020 2222 220a  ext.        """.
+00007b20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007b30: 6973 5f73 7461 7469 6328 293a 0a20 2020  is_static():.   
+00007b40: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00007b50: 2e63 6170 6163 6974 7920 6973 206e 6f74  .capacity is not
+00007b60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00007b70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00007b80: 6c66 2e73 697a 6520 3c20 7365 6c66 2e63  lf.size < self.c
+00007b90: 6170 6163 6974 790a 2020 2020 2020 2020  apacity.        
+00007ba0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00007bb0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00007bc0: 2e63 6170 6163 6974 7920 6973 206e 6f74  .capacity is not
+00007bd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00007be0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+00007bf0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+00007c00: 6c66 2e64 796e 5f73 697a 655f 6578 743a  lf.dyn_size_ext:
+00007c10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00007c20: 7572 6e20 5472 7565 2020 2320 756e 6b6e  urn True  # unkn
+00007c30: 6f77 6e0a 2020 2020 2020 2020 7265 7475  own.        retu
+00007c40: 726e 2073 656c 662e 6479 6e5f 7369 7a65  rn self.dyn_size
+00007c50: 5f65 7874 2e62 6174 6368 5f6e 6469 6d20  _ext.batch_ndim 
+00007c60: 3e20 300a 0a20 2020 2064 6566 2063 616e  > 0..    def can
+00007c70: 5f62 655f 7573 6564 5f61 735f 6469 6d28  _be_used_as_dim(
+00007c80: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00007c90: 2222 0a20 2020 2020 2020 203a 7265 7475  "".        :retu
+00007ca0: 726e 3a20 7768 6574 6865 7220 7468 6973  rn: whether this
+00007cb0: 2063 616e 2062 6520 7573 6564 2061 7320   can be used as 
+00007cc0: 6120 6469 6d20 696e 203a 636c 6173 733a  a dim in :class:
+00007cd0: 6044 6174 6160 2c20 692e 652e 2069 7420  `Data`, i.e. it 
+00007ce0: 6973 206e 6f74 2073 7065 6369 616c 0a20  is not special. 
+00007cf0: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
+00007d00: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
+00007d10: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00007d20: 6f74 2073 656c 662e 7370 6563 6961 6c0a  ot self.special.
+00007d30: 0a20 2020 2064 6566 2069 735f 7361 6d65  .    def is_same
+00007d40: 5f73 697a 655f 7465 6e73 6f72 2873 656c  _size_tensor(sel
+00007d50: 662c 2078 293a 0a20 2020 2020 2020 2022  f, x):.        "
+00007d60: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00007d70: 6d20 7466 2e54 656e 736f 7220 783a 0a20  m tf.Tensor x:. 
+00007d80: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00007d90: 7768 6574 6865 7220 7468 6973 2064 696d  whether this dim
+00007da0: 2074 6167 2066 6f72 2074 6869 7320 7370   tag for this sp
+00007db0: 6563 6966 6963 2062 6174 6368 2028 696e  ecific batch (in
+00007dc0: 636c 2062 6561 6d29 2069 7320 7468 6520  cl beam) is the 
+00007dd0: 7361 6d65 2061 7320 7468 6520 6769 7665  same as the give
+00007de0: 6e20 7369 7a65 0a20 2020 2020 2020 203a  n size.        :
+00007df0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
+00007e00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00007e10: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
+00007e20: 5f65 7874 2061 6e64 2078 2069 7320 7365  _ext and x is se
+00007e30: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
+00007e40: 706c 6163 6568 6f6c 6465 723a 0a20 2020  placeholder:.   
+00007e50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007e60: 5472 7565 0a20 2020 2020 2020 2074 6167  True.        tag
+00007e70: 203d 205f 4469 6d4d 6978 696e 2e67 6574   = _DimMixin.get
+00007e80: 5f74 6167 5f66 726f 6d5f 7369 7a65 5f74  _tag_from_size_t
+00007e90: 656e 736f 7228 7829 0a20 2020 2020 2020  ensor(x).       
+00007ea0: 2069 6620 7461 6720 616e 6420 7461 6720   if tag and tag 
+00007eb0: 3d3d 2073 656c 663a 0a20 2020 2020 2020  == self:.       
+00007ec0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00007ed0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00007ee0: 7365 6c66 2e5f 6578 7472 613a 0a20 2020  self._extra:.   
+00007ef0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007f00: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
+00007f10: 2075 7469 6c2e 5265 6649 6445 7128 7829   util.RefIdEq(x)
+00007f20: 2069 6e20 7365 6c66 2e5f 6578 7472 612e   in self._extra.
+00007f30: 6479 6e5f 7369 7a65 5f73 616d 653a 0a20  dyn_size_same:. 
+00007f40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007f50: 6e20 5472 7565 0a20 2020 2020 2020 2072  n True.        r
+00007f60: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00007f70: 2064 6566 2073 6574 5f74 6167 5f6f 6e5f   def set_tag_on_
+00007f80: 7369 7a65 5f74 656e 736f 7228 7365 6c66  size_tensor(self
+00007f90: 3a20 4469 6d2c 2078 2c20 6261 7463 683d  : Dim, x, batch=
+00007fa0: 4e6f 6e65 2c20 7361 6d65 5f61 735f 6265  None, same_as_be
+00007fb0: 666f 7265 3d46 616c 7365 2920 2d3e 2044  fore=False) -> D
+00007fc0: 696d 3a0a 2020 2020 2020 2020 2222 220a  im:.        """.
+00007fd0: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
+00007fe0: 6374 696f 6e20 6973 2075 7365 640a 2020  ction is used.  
+00007ff0: 2020 2020 2020 746f 2063 6f75 706c 6520        to couple 
+00008000: 6120 7466 2e54 656e 736f 7220 696e 7374  a tf.Tensor inst
+00008010: 616e 6365 2072 6570 7265 7365 6e74 696e  ance representin
+00008020: 6720 7468 6520 6479 6e20 7369 7a65 0a20  g the dyn size. 
+00008030: 2020 2020 2020 2077 6974 6820 7468 6520         with the 
+00008040: 6469 6d20 7461 672e 0a0a 2020 2020 2020  dim tag...      
+00008050: 2020 5468 6973 2069 7320 7573 7561 6c6c    This is usuall
+00008060: 7920 6120 6e65 776c 7920 6372 6561 7465  y a newly create
+00008070: 6420 6469 6d20 7461 672c 0a20 2020 2020  d dim tag,.     
+00008080: 2020 2077 6869 6368 2069 7320 7965 7420     which is yet 
+00008090: 756e 7365 742e 0a0a 2020 2020 2020 2020  unset...        
+000080a0: 4974 2069 7320 616c 736f 2075 7365 6420  It is also used 
+000080b0: 746f 2063 6f75 706c 6520 616e 2065 7869  to couple an exi
+000080c0: 7374 696e 6720 6469 6d20 7461 6720 7769  sting dim tag wi
+000080d0: 7468 206f 7468 6572 2064 796e 2073 697a  th other dyn siz
+000080e0: 6573 0a20 2020 2020 2020 2077 6869 6368  es.        which
+000080f0: 206a 7573 7420 6469 6666 6572 2062 7920   just differ by 
+00008100: 616e 2065 7870 616e 7369 6f6e 206f 6620  an expansion of 
+00008110: 7468 6520 6261 7463 6820 2865 2e67 2e20  the batch (e.g. 
+00008120: 7365 6172 6368 2062 6561 6d29 2e0a 0a20  search beam)... 
+00008130: 2020 2020 2020 2053 6565 2061 6c73 6f20         See also 
+00008140: 3a66 756e 633a 6067 6574 5f74 6167 5f66  :func:`get_tag_f
+00008150: 726f 6d5f 7369 7a65 5f74 656e 736f 7260  rom_size_tensor`
+00008160: 2e0a 2020 2020 2020 2020 416c 736f 2073  ..        Also s
+00008170: 6565 203a 6675 6e63 3a60 7365 745f 6479  ee :func:`set_dy
+00008180: 6e5f 7369 7a65 5f65 7874 5f66 6f72 5f62  n_size_ext_for_b
+00008190: 6174 6368 5f63 7478 602e 0a0a 2020 2020  atch_ctx`...    
+000081a0: 2020 2020 3a70 6172 616d 2078 3a20 7261      :param x: ra
+000081b0: 7720 7465 6e73 6f72 2c20 666f 7220 6578  w tensor, for ex
+000081c0: 616d 706c 6520 7466 2e54 656e 736f 720a  ample tf.Tensor.
+000081d0: 2020 2020 2020 2020 3a70 6172 616d 2042          :param B
+000081e0: 6174 6368 496e 666f 7c4e 6f6e 6520 6261  atchInfo|None ba
+000081f0: 7463 683a 0a20 2020 2020 2020 203a 7061  tch:.        :pa
+00008200: 7261 6d20 626f 6f6c 2073 616d 655f 6173  ram bool same_as
+00008210: 5f62 6566 6f72 653a 2069 6d70 6c69 6573  _before: implies
+00008220: 2069 7420 7761 7320 7365 7420 6265 666f   it was set befo
+00008230: 7265 2c20 616e 6420 7468 6520 6e65 7720  re, and the new 
+00008240: 7369 7a65 2069 7320 7468 6520 7361 6d65  size is the same
+00008250: 2e0a 2020 2020 2020 2020 2020 652e 672e  ..          e.g.
+00008260: 2069 7420 636f 756c 6420 6265 2073 6f6d   it could be som
+00008270: 6520 6964 656e 7469 7479 2077 6974 6820  e identity with 
+00008280: 6164 6465 6420 6368 6563 6b73 2c20 6f72  added checks, or
+00008290: 206f 7468 6572 2063 6861 6e67 652e 0a20   other change.. 
+000082a0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+000082b0: 7365 6c66 206f 7220 6e65 7720 6469 6d20  self or new dim 
+000082c0: 7461 670a 2020 2020 2020 2020 2222 220a  tag.        """.
+000082d0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+000082e0: 656c 662e 6361 6e5f 6265 5f75 7365 645f  elf.can_be_used_
+000082f0: 6173 5f64 696d 2829 0a20 2020 2020 2020  as_dim().       
+00008300: 2023 2049 7427 7320 756e 7573 7561 6c20   # It's unusual 
+00008310: 6966 2073 656c 662e 6469 6d65 6e73 696f  if self.dimensio
+00008320: 6e20 6973 206e 6f74 204e 6f6e 652c 2062  n is not None, b
+00008330: 7574 206c 6574 2773 2061 6363 6570 7420  ut let's accept 
+00008340: 7468 6174 2e0a 2020 2020 2020 2020 6966  that..        if
+00008350: 2068 6173 6174 7472 2878 2c20 225f 6973   hasattr(x, "_is
+00008360: 5f73 697a 655f 6f66 5f64 696d 5f74 6167  _size_of_dim_tag
+00008370: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00008380: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+00008390: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+000083a0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+000083b0: 6572 7420 782e 5f69 735f 7369 7a65 5f6f  ert x._is_size_o
+000083c0: 665f 6469 6d5f 7461 6720 696e 2028 4e6f  f_dim_tag in (No
+000083d0: 6e65 2c20 7365 6c66 290a 2020 2020 2020  ne, self).      
+000083e0: 2020 2320 4966 2077 6520 616c 7265 6164    # If we alread
+000083f0: 7920 6861 7665 2061 6e6f 7468 6572 2064  y have another d
+00008400: 796e 2073 697a 6520 7365 7420 6f72 2064  yn size set or d
+00008410: 6966 6665 7265 6e74 2062 6174 6368 2c20  ifferent batch, 
+00008420: 6372 6561 7465 2061 206e 6577 2044 696d  create a new Dim
+00008430: 2069 6e73 7461 6e63 652e 0a20 2020 2020   instance..     
+00008440: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
+00008450: 2061 6e64 2062 6174 6368 2061 6e64 2073   and batch and s
+00008460: 656c 662e 6261 7463 6820 213d 2062 6174  elf.batch != bat
+00008470: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
+00008480: 6173 7365 7274 206e 6f74 2073 616d 655f  assert not same_
+00008490: 6173 5f62 6566 6f72 6520 2023 2069 7420  as_before  # it 
+000084a0: 6361 6e6e 6f74 2062 6520 7468 6520 7361  cannot be the sa
+000084b0: 6d65 2077 6865 6e20 6974 2069 7320 616e  me when it is an
+000084c0: 6f74 6865 7220 6261 7463 682e 2e2e 0a20  other batch.... 
+000084d0: 2020 2020 2020 2020 2020 206e 6577 5f64             new_d
+000084e0: 696d 5f74 6167 203d 2073 656c 662e 6765  im_tag = self.ge
+000084f0: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
+00008500: 6261 7463 683d 6261 7463 682c 2063 7478  batch=batch, ctx
+00008510: 3d73 656c 662e 636f 6e74 726f 6c5f 666c  =self.control_fl
+00008520: 6f77 5f63 7478 290a 2020 2020 2020 2020  ow_ctx).        
+00008530: 2020 2020 6e65 775f 6469 6d5f 7461 672e      new_dim_tag.
+00008540: 7365 745f 7461 675f 6f6e 5f73 697a 655f  set_tag_on_size_
+00008550: 7465 6e73 6f72 2878 2c20 6261 7463 683d  tensor(x, batch=
+00008560: 6261 7463 6829 0a20 2020 2020 2020 2020  batch).         
+00008570: 2020 2072 6574 7572 6e20 6e65 775f 6469     return new_di
+00008580: 6d5f 7461 670a 2020 2020 2020 2020 6966  m_tag.        if
+00008590: 2073 656c 662e 6479 6e5f 7369 7a65 2069   self.dyn_size i
+000085a0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
+000085b0: 656c 662e 6479 6e5f 7369 7a65 2069 7320  elf.dyn_size is 
+000085c0: 6e6f 7420 783a 0a20 2020 2020 2020 2020  not x:.         
+000085d0: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
+000085e0: 6120 616e 6420 7574 696c 2e52 6566 4964  a and util.RefId
+000085f0: 4571 2878 2920 696e 2073 656c 662e 5f65  Eq(x) in self._e
+00008600: 7874 7261 2e64 796e 5f73 697a 655f 7361  xtra.dyn_size_sa
+00008610: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+00008620: 2020 2020 7061 7373 2020 2320 6f6b 2c20      pass  # ok, 
+00008630: 7061 7373 206f 6e0a 2020 2020 2020 2020  pass on.        
+00008640: 2020 2020 656c 6966 2073 616d 655f 6173      elif same_as
+00008650: 5f62 6566 6f72 653a 0a20 2020 2020 2020  _before:.       
+00008660: 2020 2020 2020 2020 2073 656c 662e 5f6d           self._m
+00008670: 616b 655f 6578 7472 6128 292e 6479 6e5f  ake_extra().dyn_
+00008680: 7369 7a65 5f73 616d 652e 6164 6428 7574  size_same.add(ut
+00008690: 696c 2e52 6566 4964 4571 2878 2929 0a20  il.RefIdEq(x)). 
+000086a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000086b0: 2041 6e64 206e 6f77 2070 6173 7320 6f6e   And now pass on
+000086c0: 2e0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+000086d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000086e0: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
+000086f0: 6261 7463 6820 616e 6420 6261 7463 680a  batch and batch.
+00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008710: 2320 4974 2773 206e 6f74 2063 6c65 6172  # It's not clear
+00008720: 2077 6861 7420 746f 2064 6f2e 2057 6520   what to do. We 
+00008730: 636f 756c 6420 6372 6561 7465 2061 206e  could create a n
+00008740: 6577 2064 696d 2074 6167 2c20 6275 7420  ew dim tag, but 
+00008750: 7468 6520 7369 7a65 7320 6d69 6768 7420  the sizes might 
+00008760: 6265 2064 6966 6665 7265 6e74 2e0a 2020  be different..  
+00008770: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00008780: 5573 7561 6c6c 7920 7765 2073 686f 756c  Usually we shoul
+00008790: 6420 6e6f 7420 6765 7420 6865 7265 2e0a  d not get here..
+000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087b0: 2320 536f 2066 6f72 206e 6f77 2c20 6a75  # So for now, ju
+000087c0: 7374 2065 7272 6f72 2e0a 2020 2020 2020  st error..      
+000087d0: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
+000087e0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+000087f0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+00008800: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
+00008810: 7265 7475 726e 6e2e 6672 6f6e 7465 6e64  returnn.frontend
+00008820: 2e5f 6261 636b 656e 6420 696d 706f 7274  ._backend import
+00008830: 2067 6574 5f62 6163 6b65 6e64 5f62 795f   get_backend_by_
+00008840: 7261 775f 7465 6e73 6f72 5f74 7970 650a  raw_tensor_type.
+00008850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008860: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+00008870: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008880: 2020 2020 2020 225c 6e22 2e6a 6f69 6e28        "\n".join(
+00008890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000088a0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
+000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088c0: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
+000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088e0: 2020 2020 2020 2020 2022 2572 2028 2572           "%r (%r
+000088f0: 2920 616c 7265 6164 7920 6861 7320 7369  ) already has si
+00008900: 7a65 2025 722c 220a 2020 2020 2020 2020  ze %r,".        
+00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008920: 2020 2020 2020 2020 2220 616e 6420 616e          " and an
+00008930: 6f74 6865 7220 696e 636f 6d70 6174 6962  other incompatib
+00008940: 6c65 2073 697a 6520 2572 2028 6261 7463  le size %r (batc
+00008950: 6820 2572 2920 6973 2062 6569 6e67 2061  h %r) is being a
+00008960: 7373 6967 6e65 642e 220a 2020 2020 2020  ssigned.".      
 00008970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008980: 2020 2022 5c6e 4e65 7720 7369 7a65 2063     "\nNew size c
-00008990: 6f6d 7075 7461 7469 6f6e 2067 7261 7068  omputation graph
-000089a0: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
-000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089c0: 6765 745f 6261 636b 656e 645f 6279 5f72  get_backend_by_r
-000089d0: 6177 5f74 656e 736f 725f 7479 7065 2874  aw_tensor_type(t
-000089e0: 7970 6528 7829 292e 666f 726d 6174 5f67  ype(x)).format_g
-000089f0: 7261 7068 5f6f 7574 7075 7428 782c 206d  raph_output(x, m
-00008a00: 6178 5f64 6570 7468 3d33 292c 0a20 2020  ax_depth=3),.   
-00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a20: 2020 2020 2020 2020 2022 5c6e 5468 6973           "\nThis
-00008a30: 2069 7320 6d61 7962 6520 7468 6520 7265   is maybe the re
-00008a40: 7375 6c74 206f 6620 616e 2069 6e63 6f72  sult of an incor
-00008a50: 7265 6374 2064 6563 6c61 7265 5f73 616d  rect declare_sam
-00008a60: 655f 6173 2e20 222c 0a20 2020 2020 2020  e_as. ",.       
-00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a80: 2020 2020 2022 7361 6d65 5f61 7320 3d20       "same_as = 
-00008a90: 2573 2220 2520 7365 6c66 2e73 616d 655f  %s" % self.same_
-00008aa0: 6173 2c0a 2020 2020 2020 2020 2020 2020  as,.            
-00008ab0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00008ae0: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
-00008af0: 2062 6174 6368 2061 6e64 2067 6574 6174   batch and getat
-00008b00: 7472 2878 2c20 225f 5245 5455 524e 4e5f  tr(x, "_RETURNN_
-00008b10: 6479 6e5f 7369 7a65 5f62 6561 6d22 2c20  dyn_size_beam", 
-00008b20: 4e6f 6e65 293a 0a20 2020 2020 2020 2020  None):.         
-00008b30: 2020 2061 7373 6572 7420 6261 7463 682e     assert batch.
-00008b40: 6265 616d 203d 3d20 6765 7461 7474 7228  beam == getattr(
-00008b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008b60: 2078 2c20 225f 5245 5455 524e 4e5f 6479   x, "_RETURNN_dy
-00008b70: 6e5f 7369 7a65 5f62 6561 6d22 0a20 2020  n_size_beam".   
-00008b80: 2020 2020 2020 2020 2029 2c20 2225 733a           ), "%s:
-00008b90: 2064 796e 2073 697a 6520 2573 2068 6173   dyn size %s has
-00008ba0: 2075 6e65 7870 6563 7465 6420 6261 7463   unexpected batc
-00008bb0: 6820 2573 2c20 6578 7065 6374 6564 2025  h %s, expected %
-00008bc0: 7322 2025 2028 0a20 2020 2020 2020 2020  s" % (.         
-00008bd0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00008be0: 2020 2020 2020 2020 2020 2020 2078 2c0a               x,.
-00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c00: 6261 7463 682c 0a20 2020 2020 2020 2020  batch,.         
-00008c10: 2020 2020 2020 2067 6574 6174 7472 2878         getattr(x
-00008c20: 2c20 225f 5245 5455 524e 4e5f 6479 6e5f  , "_RETURNN_dyn_
-00008c30: 7369 7a65 5f62 6561 6d22 292c 0a20 2020  size_beam"),.   
-00008c40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00008c50: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
-00008c60: 2061 6e64 2062 6174 6368 3a0a 2020 2020   and batch:.    
-00008c70: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00008c80: 656c 662e 6261 7463 6820 3d3d 2062 6174  elf.batch == bat
-00008c90: 6368 0a20 2020 2020 2020 2065 6c69 6620  ch.        elif 
-00008ca0: 6261 7463 6820 616e 6420 6e6f 7420 7365  batch and not se
-00008cb0: 6c66 2e62 6174 6368 3a0a 2020 2020 2020  lf.batch:.      
-00008cc0: 2020 2020 2020 7365 6c66 2e62 6174 6368        self.batch
-00008cd0: 203d 2062 6174 6368 2020 2320 6f76 6572   = batch  # over
-00008ce0: 7461 6b65 0a20 2020 2020 2020 2069 6620  take.        if 
-00008cf0: 6e6f 7420 7365 6c66 2e69 735f 6261 7463  not self.is_batc
-00008d00: 685f 6469 6d28 2920 616e 6420 7365 6c66  h_dim() and self
-00008d10: 2e69 735f 6479 6e61 6d69 6328 293a 0a20  .is_dynamic():. 
-00008d20: 2020 2020 2020 2020 2020 2069 6620 7361             if sa
-00008d30: 6d65 5f61 735f 6265 666f 7265 3a0a 2020  me_as_before:.  
-00008d40: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00008d50: 7365 7274 2073 656c 662e 6479 6e5f 7369  sert self.dyn_si
-00008d60: 7a65 5f65 7874 2061 6e64 2073 656c 662e  ze_ext and self.
-00008d70: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
-00008d80: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
-00008d90: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00008da0: 2020 2020 2023 2044 6f20 6e6f 7420 6f76       # Do not ov
-00008db0: 6572 7772 6974 6520 6974 2e0a 2020 2020  erwrite it..    
-00008dc0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00008dd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008de0: 6c66 2e5f 696e 6974 5f64 6566 6175 6c74  lf._init_default
-00008df0: 5f64 796e 5f73 697a 655f 6578 7428 7829  _dyn_size_ext(x)
-00008e00: 0a20 2020 2020 2020 2069 6620 6765 7461  .        if geta
-00008e10: 7474 7228 782c 2022 5f69 735f 7369 7a65  ttr(x, "_is_size
-00008e20: 5f6f 665f 6469 6d5f 7461 6722 2c20 4e6f  _of_dim_tag", No
-00008e30: 6e65 2920 6973 204e 6f6e 653a 0a20 2020  ne) is None:.   
-00008e40: 2020 2020 2020 2020 2073 6574 6174 7472           setattr
-00008e50: 2878 2c20 225f 6973 5f73 697a 655f 6f66  (x, "_is_size_of
-00008e60: 5f64 696d 5f74 6167 222c 2073 656c 6629  _dim_tag", self)
-00008e70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008e80: 7365 6c66 0a0a 2020 2020 4063 6c61 7373  self..    @class
-00008e90: 6d65 7468 6f64 0a20 2020 2064 6566 2067  method.    def g
-00008ea0: 6574 5f74 6167 5f66 726f 6d5f 7369 7a65  et_tag_from_size
-00008eb0: 5f74 656e 736f 7228 636c 732c 2078 2920  _tensor(cls, x) 
-00008ec0: 2d3e 204f 7074 696f 6e61 6c5b 5f64 2e44  -> Optional[_d.D
-00008ed0: 696d 5d3a 0a20 2020 2020 2020 2022 2222  im]:.        """
-00008ee0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00008ef0: 7466 2e54 656e 736f 7220 783a 2073 697a  tf.Tensor x: siz
-00008f00: 6520 7465 6e73 6f72 2e20 6861 7320 6265  e tensor. has be
-00008f10: 656e 2073 6574 2062 6566 6f72 6520 7669  en set before vi
-00008f20: 6120 3a66 756e 633a 6073 6574 5f74 6167  a :func:`set_tag
-00008f30: 5f6f 6e5f 7369 7a65 5f74 656e 736f 7260  _on_size_tensor`
-00008f40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00008f50: 2020 2020 2072 6574 7572 6e20 6765 7461       return geta
-00008f60: 7474 7228 782c 2022 5f69 735f 7369 7a65  ttr(x, "_is_size
-00008f70: 5f6f 665f 6469 6d5f 7461 6722 2c20 4e6f  _of_dim_tag", No
-00008f80: 6e65 290a 0a20 2020 2064 6566 2063 6f6d  ne)..    def com
-00008f90: 706c 6574 655f 6479 6e5f 7369 7a65 2873  plete_dyn_size(s
-00008fa0: 656c 662c 2074 656d 706c 6174 655f 6f6e  elf, template_on
-00008fb0: 6c79 3d46 616c 7365 293a 0a20 2020 2020  ly=False):.     
-00008fc0: 2020 2022 2222 0a20 2020 2020 2020 2049     """.        I
-00008fd0: 6e20 6361 7365 2077 6520 6361 6e20 6361  n case we can ca
-00008fe0: 6c63 756c 6174 6520 7468 6520 6479 6e20  lculate the dyn 
-00008ff0: 7369 7a65 2c20 646f 2074 6861 7420 6e6f  size, do that no
-00009000: 772e 0a0a 2020 2020 2020 2020 3a70 6172  w...        :par
-00009010: 616d 2062 6f6f 6c20 7465 6d70 6c61 7465  am bool template
-00009020: 5f6f 6e6c 793a 0a20 2020 2020 2020 2022  _only:.        "
-00009030: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-00009040: 7420 7365 6c66 2e69 735f 6479 6e61 6d69  t self.is_dynami
-00009050: 6328 293a 0a20 2020 2020 2020 2020 2020  c():.           
-00009060: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00009070: 7365 6c66 2e5f 7661 6c69 6461 7465 5f69  self._validate_i
-00009080: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
-00009090: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000090a0: 662e 6479 6e5f 7369 7a65 5f65 7874 2061  f.dyn_size_ext a
-000090b0: 6e64 2028 7365 6c66 2e64 796e 5f73 697a  nd (self.dyn_siz
-000090c0: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
-000090d0: 7220 6973 206e 6f74 204e 6f6e 6520 6f72  r is not None or
-000090e0: 2074 656d 706c 6174 655f 6f6e 6c79 293a   template_only):
-000090f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00009100: 7572 6e0a 2020 2020 2020 2020 7361 6d65  urn.        same
-00009110: 5f62 6173 6520 3d20 7365 6c66 2e67 6574  _base = self.get
-00009120: 5f73 616d 655f 6261 7365 2829 0a20 2020  _same_base().   
-00009130: 2020 2020 206f 7020 3d20 7365 6c66 2e64       op = self.d
-00009140: 6572 6976 6564 5f66 726f 6d5f 6f70 206f  erived_from_op o
-00009150: 7220 7361 6d65 5f62 6173 652e 6465 7269  r same_base.deri
-00009160: 7665 645f 6672 6f6d 5f6f 700a 2020 2020  ved_from_op.    
-00009170: 2020 2020 6966 206e 6f74 206f 703a 0a20      if not op:. 
-00009180: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009190: 6e0a 0a20 2020 2020 2020 2066 6f72 2078  n..        for x
-000091a0: 2069 6e20 6f70 2e69 6e70 7574 733a 0a20   in op.inputs:. 
-000091b0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000091c0: 6c66 2e62 6174 6368 3a0a 2020 2020 2020  lf.batch:.      
-000091d0: 2020 2020 2020 2020 2020 7820 3d20 782e            x = x.
-000091e0: 6765 745f 666f 725f 6261 7463 685f 6374  get_for_batch_ct
-000091f0: 7828 7365 6c66 2e62 6174 6368 2c20 7365  x(self.batch, se
-00009200: 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  lf.control_flow_
-00009210: 6374 7829 0a20 2020 2020 2020 2020 2020  ctx).           
-00009220: 2078 2e63 6f6d 706c 6574 655f 6479 6e5f   x.complete_dyn_
-00009230: 7369 7a65 2874 656d 706c 6174 655f 6f6e  size(template_on
-00009240: 6c79 3d74 656d 706c 6174 655f 6f6e 6c79  ly=template_only
-00009250: 290a 0a20 2020 2020 2020 2062 6163 6b65  )..        backe
-00009260: 6e64 203d 204e 6f6e 650a 2020 2020 2020  nd = None.      
-00009270: 2020 666f 7220 7820 696e 206f 702e 696e    for x in op.in
-00009280: 7075 7473 3a0a 2020 2020 2020 2020 2020  puts:.          
-00009290: 2020 6966 2073 656c 662e 6261 7463 683a    if self.batch:
-000092a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000092b0: 2078 203d 2078 2e67 6574 5f66 6f72 5f62   x = x.get_for_b
-000092c0: 6174 6368 5f63 7478 2873 656c 662e 6261  atch_ctx(self.ba
-000092d0: 7463 682c 2073 656c 662e 636f 6e74 726f  tch, self.contro
-000092e0: 6c5f 666c 6f77 5f63 7478 290a 2020 2020  l_flow_ctx).    
-000092f0: 2020 2020 2020 2020 6966 2078 2e64 796e          if x.dyn
-00009300: 5f73 697a 655f 6578 7420 616e 6420 782e  _size_ext and x.
-00009310: 6479 6e5f 7369 7a65 5f65 7874 2e72 6177  dyn_size_ext.raw
-00009320: 5f74 656e 736f 7220 6973 206e 6f74 204e  _tensor is not N
-00009330: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00009340: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
-00009350: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
-00009360: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
-00009370: 2020 2020 2020 6261 636b 656e 6420 3d20        backend = 
-00009380: 782e 6479 6e5f 7369 7a65 5f65 7874 2e5f  x.dyn_size_ext._
-00009390: 7261 775f 6261 636b 656e 640a 2020 2020  raw_backend.    
-000093a0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-000093b0: 6b0a 0a20 2020 2020 2020 2073 697a 655f  k..        size_
-000093c0: 6474 7970 6520 3d20 4e6f 6e65 0a20 2020  dtype = None.   
-000093d0: 2020 2020 2066 6f72 2078 2069 6e20 6f70       for x in op
-000093e0: 2e69 6e70 7574 733a 0a20 2020 2020 2020  .inputs:.       
-000093f0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
-00009400: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-00009410: 2020 2020 7820 3d20 782e 6765 745f 666f      x = x.get_fo
-00009420: 725f 6261 7463 685f 6374 7828 7365 6c66  r_batch_ctx(self
-00009430: 2e62 6174 6368 2c20 7365 6c66 2e63 6f6e  .batch, self.con
-00009440: 7472 6f6c 5f66 6c6f 775f 6374 7829 0a20  trol_flow_ctx). 
-00009450: 2020 2020 2020 2020 2020 2069 6620 782e             if x.
-00009460: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
-00009470: 2020 2020 2020 2020 2020 2020 2020 7369                si
-00009480: 7a65 5f64 7479 7065 203d 2078 2e64 796e  ze_dtype = x.dyn
-00009490: 5f73 697a 655f 6578 742e 6474 7970 650a  _size_ext.dtype.
-000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094b0: 6272 6561 6b0a 2020 2020 2020 2020 6966  break.        if
-000094c0: 206e 6f74 2073 697a 655f 6474 7970 653a   not size_dtype:
-000094d0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-000094e0: 655f 6474 7970 6520 3d20 5f74 2e54 656e  e_dtype = _t.Ten
-000094f0: 736f 722e 7369 7a65 5f64 7479 7065 0a0a  sor.size_dtype..
-00009500: 2020 2020 2020 2020 696d 706f 7274 206e          import n
-00009510: 756d 7079 0a20 2020 2020 2020 2069 6d70  umpy.        imp
-00009520: 6f72 7420 7265 7475 726e 6e2e 6672 6f6e  ort returnn.fron
-00009530: 7465 6e64 2061 7320 7266 0a0a 2020 2020  tend as rf..    
-00009540: 2020 2020 7466 203d 2074 665f 7574 696c      tf = tf_util
-00009550: 203d 2074 656e 736f 725f 7574 696c 203d   = tensor_util =
-00009560: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-00009570: 2062 6163 6b65 6e64 2061 6e64 2062 6163   backend and bac
-00009580: 6b65 6e64 2e69 735f 7465 6e73 6f72 666c  kend.is_tensorfl
-00009590: 6f77 3a0a 2020 2020 2020 2020 2020 2020  ow:.            
-000095a0: 696d 706f 7274 2074 656e 736f 7266 6c6f  import tensorflo
-000095b0: 7720 6173 2074 660a 0a20 2020 2020 2020  w as tf..       
-000095c0: 2020 2020 2069 6620 6261 636b 656e 642e       if backend.
-000095d0: 5261 7754 656e 736f 7254 7970 6520 3d3d  RawTensorType ==
-000095e0: 2074 662e 5465 6e73 6f72 3a0a 2020 2020   tf.Tensor:.    
-000095f0: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
-00009600: 2072 6574 7572 6e6e 2e74 662e 7574 696c   returnn.tf.util
-00009610: 2069 6d70 6f72 7420 6261 7369 6320 6173   import basic as
-00009620: 2074 665f 7574 696c 0a20 2020 2020 2020   tf_util.       
-00009630: 2020 2020 2020 2020 2066 726f 6d20 7465           from te
-00009640: 6e73 6f72 666c 6f77 2e70 7974 686f 6e2e  nsorflow.python.
-00009650: 6672 616d 6577 6f72 6b20 696d 706f 7274  framework import
-00009660: 2074 656e 736f 725f 7574 696c 0a20 2020   tensor_util.   
-00009670: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00009680: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00009690: 6620 3d20 4e6f 6e65 0a0a 2020 2020 2020  f = None..      
-000096a0: 2020 6b69 6e64 203d 206f 702e 6b69 6e64    kind = op.kind
-000096b0: 0a20 2020 2020 2020 2069 6620 6b69 6e64  .        if kind
-000096c0: 2e65 6e64 7377 6974 6828 225f 7269 6768  .endswith("_righ
-000096d0: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
-000096e0: 206b 696e 6420 3d20 6b69 6e64 5b3a 202d   kind = kind[: -
-000096f0: 6c65 6e28 225f 7269 6768 7422 295d 2020  len("_right")]  
-00009700: 2320 6f72 6465 7220 646f 6573 206e 6f74  # order does not
-00009710: 206d 6174 7465 7220 6865 7265 0a20 2020   matter here.   
-00009720: 2020 2020 2069 6620 6b69 6e64 2e65 6e64       if kind.end
-00009730: 7377 6974 6828 225f 6c65 6674 2229 3a0a  swith("_left"):.
-00009740: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
-00009750: 203d 206b 696e 645b 3a20 2d6c 656e 2822   = kind[: -len("
-00009760: 5f6c 6566 7422 295d 0a0a 2020 2020 2020  _left")]..      
-00009770: 2020 6465 6620 5f69 735f 6e65 6761 7469    def _is_negati
-00009780: 7665 2878 5f5f 293a 0a20 2020 2020 2020  ve(x__):.       
-00009790: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-000097a0: 6365 2878 5f5f 2c20 6e75 6d70 792e 6e64  ce(x__, numpy.nd
-000097b0: 6172 7261 7929 3a0a 2020 2020 2020 2020  array):.        
-000097c0: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-000097d0: 785f 5f20 3c20 3029 2e61 6e79 2829 0a20  x__ < 0).any(). 
-000097e0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-000097f0: 696e 7374 616e 6365 2878 5f5f 2c20 2869  instance(x__, (i
-00009800: 6e74 2c20 666c 6f61 742c 206e 756d 7079  nt, float, numpy
-00009810: 2e6e 756d 6265 7229 293a 0a20 2020 2020  .number)):.     
-00009820: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009830: 6e20 785f 5f20 3c20 300a 2020 2020 2020  n x__ < 0.      
-00009840: 2020 2020 2020 6966 206e 6f74 2074 663a        if not tf:
-00009850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009860: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-00009870: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00009880: 2069 7369 6e73 7461 6e63 6528 785f 5f2c   isinstance(x__,
-00009890: 2074 662e 5465 6e73 6f72 290a 2020 2020   tf.Tensor).    
-000098a0: 2020 2020 2020 2020 785f 5f20 3d20 7465          x__ = te
-000098b0: 6e73 6f72 5f75 7469 6c2e 636f 6e73 7461  nsor_util.consta
-000098c0: 6e74 5f76 616c 7565 2878 5f5f 290a 2020  nt_value(x__).  
-000098d0: 2020 2020 2020 2020 2020 6966 2078 5f5f            if x__
-000098e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000098f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00009900: 7475 726e 205f 6973 5f6e 6567 6174 6976  turn _is_negativ
-00009910: 6528 785f 5f29 0a20 2020 2020 2020 2020  e(x__).         
-00009920: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00009930: 0a20 2020 2020 2020 2064 6566 205f 6269  .        def _bi
-00009940: 6e5f 6f70 5f74 6628 612c 2062 293a 0a20  n_op_tf(a, b):. 
-00009950: 2020 2020 2020 2020 2020 2069 6620 7465             if te
-00009960: 6d70 6c61 7465 5f6f 6e6c 793a 0a20 2020  mplate_only:.   
-00009970: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00009980: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-00009990: 2020 2020 2069 6620 6120 6973 204e 6f6e       if a is Non
-000099a0: 6520 6f72 2062 2069 7320 4e6f 6e65 3a0a  e or b is None:.
-000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099c0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-000099d0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-000099e0: 7369 6e73 7461 6e63 6528 612c 2074 662e  sinstance(a, tf.
-000099f0: 5465 6e73 6f72 2920 616e 6420 6973 696e  Tensor) and isin
-00009a00: 7374 616e 6365 2862 2c20 2869 6e74 2c20  stance(b, (int, 
-00009a10: 7466 2e54 656e 736f 7229 290a 2020 2020  tf.Tensor)).    
-00009a20: 2020 2020 2020 2020 7769 7468 2074 665f          with tf_
-00009a30: 7574 696c 2e73 616d 655f 636f 6e74 726f  util.same_contro
-00009a40: 6c5f 666c 6f77 5f63 7478 285b 612c 2062  l_flow_ctx([a, b
-00009a50: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-00009a60: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
-00009a70: 6164 6422 3a0a 2020 2020 2020 2020 2020  add":.          
-00009a80: 2020 2020 2020 2020 2020 7573 655f 7265            use_re
-00009a90: 6c75 203d 205f 6973 5f6e 6567 6174 6976  lu = _is_negativ
-00009aa0: 6528 6129 206f 7220 5f69 735f 6e65 6761  e(a) or _is_nega
-00009ab0: 7469 7665 2862 2920 2023 2066 6f72 2064  tive(b)  # for d
-00009ac0: 796e 616d 6963 2074 656e 736f 7273 2c20  ynamic tensors, 
-00009ad0: 6173 7375 6d65 2061 6c6c 2070 6f73 6974  assume all posit
-00009ae0: 6976 650a 2020 2020 2020 2020 2020 2020  ive.            
-00009af0: 2020 2020 2020 2020 6966 2075 7365 5f72          if use_r
-00009b00: 656c 753a 0a20 2020 2020 2020 2020 2020  elu:.           
-00009b10: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00009b20: 7572 6e20 7466 2e63 6f6e 7665 7274 5f74  urn tf.convert_t
-00009b30: 6f5f 7465 6e73 6f72 2874 665f 7574 696c  o_tensor(tf_util
-00009b40: 2e73 696d 706c 6966 795f 6e6f 6e5f 6e65  .simplify_non_ne
-00009b50: 6761 7469 7665 5f73 6571 5f6c 656e 6774  gative_seq_lengt
-00009b60: 6828 6120 2b20 6229 290a 2020 2020 2020  h(a + b)).      
-00009b70: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00009b80: 7475 726e 2061 202b 2062 0a20 2020 2020  turn a + b.     
-00009b90: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00009ba0: 6b69 6e64 203d 3d20 2273 7562 223a 0a20  kind == "sub":. 
-00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bc0: 2020 2072 6574 7572 6e20 7466 2e63 6f6e     return tf.con
-00009bd0: 7665 7274 5f74 6f5f 7465 6e73 6f72 2874  vert_to_tensor(t
-00009be0: 665f 7574 696c 2e73 696d 706c 6966 795f  f_util.simplify_
-00009bf0: 6e6f 6e5f 6e65 6761 7469 7665 5f73 6571  non_negative_seq
-00009c00: 5f6c 656e 6774 6828 6120 2d20 6229 290a  _length(a - b)).
-00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c20: 656c 6966 206b 696e 6420 3d3d 2022 6d75  elif kind == "mu
-00009c30: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
-00009c40: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00009c50: 202a 2062 0a20 2020 2020 2020 2020 2020   * b.           
-00009c60: 2020 2020 2065 6c69 6620 6b69 6e64 2069       elif kind i
-00009c70: 6e20 2822 666c 6f6f 7264 6976 222c 2022  n ("floordiv", "
-00009c80: 7472 7565 6469 7622 293a 2020 2320 7472  truediv"):  # tr
-00009c90: 7565 6469 7620 6173 7375 6d65 7320 7468  uediv assumes th
-00009ca0: 6572 6520 6973 206e 6f20 7265 6d61 696e  ere is no remain
-00009cb0: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
-00009cc0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00009cd0: 202f 2f20 620a 2020 2020 2020 2020 2020   // b.          
-00009ce0: 2020 2020 2020 656c 6966 206b 696e 6420        elif kind 
-00009cf0: 3d3d 2022 6365 696c 6469 7622 3a0a 2020  == "ceildiv":.  
-00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d10: 2020 7265 7475 726e 202d 282d 6120 2f2f    return -(-a //
-00009d20: 2062 290a 2020 2020 2020 2020 2020 2020   b).            
-00009d30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00009d40: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00009d50: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00009d60: 756e 6b6e 6f77 6e20 6f70 206b 696e 6420  unknown op kind 
-00009d70: 2572 2220 2520 6f70 2e6b 696e 6429 0a0a  %r" % op.kind)..
-00009d80: 2020 2020 2020 2020 6465 6620 5f62 696e          def _bin
-00009d90: 5f6f 7028 612c 2062 293a 0a20 2020 2020  _op(a, b):.     
-00009da0: 2020 2020 2020 2069 6620 7465 6d70 6c61         if templa
-00009db0: 7465 5f6f 6e6c 7920 6f72 206e 6f74 2062  te_only or not b
-00009dc0: 6163 6b65 6e64 3a0a 2020 2020 2020 2020  ackend:.        
-00009dd0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00009de0: 7461 6e63 6528 612c 205f 742e 5465 6e73  tance(a, _t.Tens
-00009df0: 6f72 2920 616e 6420 6973 696e 7374 616e  or) and isinstan
-00009e00: 6365 2862 2c20 5f74 2e54 656e 736f 7229  ce(b, _t.Tensor)
-00009e10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009e20: 2020 2020 2020 7265 7475 726e 205f 742e        return _t.
-00009e30: 5465 6e73 6f72 2e67 6574 5f63 6f6d 6d6f  Tensor.get_commo
-00009e40: 6e5f 6461 7461 285b 612c 2062 5d2c 2061  n_data([a, b], a
-00009e50: 6c6c 6f77 5f62 726f 6164 6361 7374 5f61  llow_broadcast_a
-00009e60: 6c6c 5f73 6f75 7263 6573 3d54 7275 6529  ll_sources=True)
-00009e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e80: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
-00009e90: 2c20 5f74 2e54 656e 736f 7229 3a0a 2020  , _t.Tensor):.  
-00009ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009eb0: 2020 7265 7475 726e 2061 0a20 2020 2020    return a.     
-00009ec0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-00009ed0: 696e 7374 616e 6365 2862 2c20 5f74 2e54  instance(b, _t.T
-00009ee0: 656e 736f 7229 3a0a 2020 2020 2020 2020  ensor):.        
-00009ef0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009f00: 726e 2062 0a20 2020 2020 2020 2020 2020  rn b.           
-00009f10: 2069 6620 6b69 6e64 203d 3d20 2261 6464   if kind == "add
-00009f20: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00009f30: 2020 2072 6574 7572 6e20 5f72 656c 7528     return _relu(
-00009f40: 6120 2b20 6229 0a20 2020 2020 2020 2020  a + b).         
-00009f50: 2020 2065 6c69 6620 6b69 6e64 203d 3d20     elif kind == 
-00009f60: 2273 7562 223a 0a20 2020 2020 2020 2020  "sub":.         
-00009f70: 2020 2020 2020 2072 6574 7572 6e20 5f72         return _r
-00009f80: 656c 7528 6120 2d20 6229 0a20 2020 2020  elu(a - b).     
-00009f90: 2020 2020 2020 2065 6c69 6620 6b69 6e64         elif kind
-00009fa0: 203d 3d20 226d 756c 223a 0a20 2020 2020   == "mul":.     
-00009fb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00009fc0: 6e20 6120 2a20 620a 2020 2020 2020 2020  n a * b.        
-00009fd0: 2020 2020 656c 6966 206b 696e 6420 696e      elif kind in
-00009fe0: 2028 2266 6c6f 6f72 6469 7622 2c20 2274   ("floordiv", "t
-00009ff0: 7275 6564 6976 2229 3a20 2023 2074 7275  ruediv"):  # tru
-0000a000: 6564 6976 2061 7373 756d 6573 2074 6865  ediv assumes the
-0000a010: 7265 2069 7320 6e6f 2072 656d 6169 6e64  re is no remaind
-0000a020: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-0000a030: 2020 2072 6574 7572 6e20 6120 2f2f 2062     return a // b
-0000a040: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0000a050: 6620 6b69 6e64 203d 3d20 2263 6569 6c64  f kind == "ceild
-0000a060: 6976 223a 0a20 2020 2020 2020 2020 2020  iv":.           
-0000a070: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0000a080: 6365 2861 2c20 5f74 2e54 656e 736f 7229  ce(a, _t.Tensor)
-0000a090: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a0a0: 2020 2020 2020 7265 7475 726e 2072 662e        return rf.
-0000a0b0: 6365 696c 5f64 6976 6964 6528 612c 2062  ceil_divide(a, b
-0000a0c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a0d0: 2020 7265 7475 726e 202d 282d 6120 2f2f    return -(-a //
-0000a0e0: 2062 290a 2020 2020 2020 2020 2020 2020   b).            
-0000a0f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000a100: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000a110: 6545 7272 6f72 2822 756e 6b6e 6f77 6e20  eError("unknown 
-0000a120: 6f70 206b 696e 6420 2572 2220 2520 6f70  op kind %r" % op
-0000a130: 2e6b 696e 6429 0a0a 2020 2020 2020 2020  .kind)..        
-0000a140: 6465 6620 5f72 656c 7528 6129 3a0a 2020  def _relu(a):.  
-0000a150: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-0000a160: 6e73 7461 6e63 6528 612c 205f 742e 5465  nstance(a, _t.Te
-0000a170: 6e73 6f72 293a 0a20 2020 2020 2020 2020  nsor):.         
-0000a180: 2020 2020 2020 2072 6574 7572 6e20 7266         return rf
-0000a190: 2e72 656c 7528 6129 0a20 2020 2020 2020  .relu(a).       
-0000a1a0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-0000a1b0: 616e 6365 2861 2c20 696e 7429 3a0a 2020  ance(a, int):.  
-0000a1c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000a1d0: 7475 726e 206d 6178 2861 2c20 3029 0a20  turn max(a, 0). 
-0000a1e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000a1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a200: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-0000a210: 2866 2263 6f6d 706c 6574 655f 6479 6e5f  (f"complete_dyn_
-0000a220: 7369 7a65 3a20 5f72 656c 753a 2075 6e65  size: _relu: une
-0000a230: 7870 6563 7465 6420 7479 7065 207b 7479  xpected type {ty
-0000a240: 7065 2861 297d 2229 0a0a 2020 2020 2020  pe(a)}")..      
-0000a250: 2020 795f 6e61 6d65 203d 2073 656c 662e    y_name = self.
-0000a260: 6465 7363 7269 7074 696f 6e20 2b20 223a  description + ":
-0000a270: 7365 712d 6c65 6e67 7468 220a 2020 2020  seq-length".    
-0000a280: 2020 2020 793a 204f 7074 696f 6e61 6c5b      y: Optional[
-0000a290: 5f74 2e54 656e 736f 725d 203d 204e 6f6e  _t.Tensor] = Non
-0000a2a0: 6520 2023 2072 6573 756c 7469 6e67 2064  e  # resulting d
-0000a2b0: 796e 2073 697a 650a 2020 2020 2020 2020  yn size.        
-0000a2c0: 696e 7075 7473 203d 206c 6973 7428 6f70  inputs = list(op
-0000a2d0: 2e69 6e70 7574 7329 0a20 2020 2020 2020  .inputs).       
-0000a2e0: 2061 7373 6572 7420 696e 7075 7473 0a20   assert inputs. 
-0000a2f0: 2020 2020 2020 2077 6869 6c65 2069 6e70         while inp
-0000a300: 7574 733a 0a20 2020 2020 2020 2020 2020  uts:.           
-0000a310: 2078 203d 2069 6e70 7574 732e 706f 7028   x = inputs.pop(
-0000a320: 3029 0a20 2020 2020 2020 2020 2020 2069  0).            i
-0000a330: 6620 6e6f 7420 782e 6973 5f64 796e 616d  f not x.is_dynam
-0000a340: 6963 2829 3a20 2023 2073 7461 7469 630a  ic():  # static.
-0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a360: 6173 7365 7274 2078 2e64 696d 656e 7369  assert x.dimensi
-0000a370: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 0a20  on is not None. 
-0000a380: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000a390: 6620 7920 6973 204e 6f6e 653a 0a20 2020  f y is None:.   
-0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3b0: 2069 6620 6e6f 7420 7465 6d70 6c61 7465   if not template
-0000a3c0: 5f6f 6e6c 7920 616e 6420 6261 636b 656e  _only and backen
-0000a3d0: 6420 616e 6420 6e6f 7420 7466 3a0a 2020  d and not tf:.  
-0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3f0: 2020 2020 2020 7920 3d20 6261 636b 656e        y = backen
-0000a400: 642e 636f 6e76 6572 745f 746f 5f74 656e  d.convert_to_ten
-0000a410: 736f 7228 782e 6469 6d65 6e73 696f 6e2c  sor(x.dimension,
-0000a420: 2064 696d 733d 5b5d 2c20 6474 7970 653d   dims=[], dtype=
-0000a430: 7369 7a65 5f64 7479 7065 2c20 6e61 6d65  size_dtype, name
-0000a440: 3d79 5f6e 616d 6529 0a20 2020 2020 2020  =y_name).       
-0000a450: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000a460: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000a470: 2020 2020 2020 2020 2020 2079 203d 205f             y = _
-0000a480: 742e 5465 6e73 6f72 280a 2020 2020 2020  t.Tensor(.      
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 2020 2020 6e61 6d65 3d79 5f6e 616d        name=y_nam
-0000a4b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000a4d0: 696d 5f74 6167 733d 5b5d 2c0a 2020 2020  im_tags=[],.    
-0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4f0: 2020 2020 2020 2020 6474 7970 653d 7369          dtype=si
-0000a500: 7a65 5f64 7479 7065 2c0a 2020 2020 2020  ze_dtype,.      
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000a530: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000a540: 6f74 2074 656d 706c 6174 655f 6f6e 6c79  ot template_only
-0000a550: 2061 6e64 2074 663a 0a20 2020 2020 2020   and tf:.       
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a570: 2020 2020 2077 6974 6820 7466 2e63 6f6e       with tf.con
-0000a580: 7472 6f6c 5f64 6570 656e 6465 6e63 6965  trol_dependencie
-0000a590: 7328 4e6f 6e65 293a 2020 2320 7468 6973  s(None):  # this
-0000a5a0: 2077 696c 6c20 7265 7365 7420 7468 6520   will reset the 
-0000a5b0: 636f 6e74 6578 740a 2020 2020 2020 2020  context.        
-0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 2020 2020 2020 792e 7261 775f 7465          y.raw_te
-0000a5e0: 6e73 6f72 203d 2074 662e 636f 6e73 7461  nsor = tf.consta
-0000a5f0: 6e74 2878 2e64 696d 656e 7369 6f6e 290a  nt(x.dimension).
-0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a610: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-0000a620: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a630: 7466 3a0a 2020 2020 2020 2020 2020 2020  tf:.            
-0000a640: 2020 2020 2020 2020 792e 706c 6163 6568          y.placeh
-0000a650: 6f6c 6465 7220 3d20 5f62 696e 5f6f 705f  older = _bin_op_
-0000a660: 7466 2879 2e70 6c61 6365 686f 6c64 6572  tf(y.placeholder
-0000a670: 2c20 782e 6469 6d65 6e73 696f 6e29 0a20  , x.dimension). 
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000a690: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000a6a0: 2020 2020 2020 2020 2079 203d 205f 6269           y = _bi
-0000a6b0: 6e5f 6f70 2879 2c20 782e 6469 6d65 6e73  n_op(y, x.dimens
-0000a6c0: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
-0000a6d0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-0000a6e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000a6f0: 662e 6261 7463 683a 0a20 2020 2020 2020  f.batch:.       
-0000a700: 2020 2020 2020 2020 2078 203d 2078 2e67           x = x.g
-0000a710: 6574 5f66 6f72 5f62 6174 6368 5f63 7478  et_for_batch_ctx
-0000a720: 2873 656c 662e 6261 7463 682c 2073 656c  (self.batch, sel
-0000a730: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
-0000a740: 7478 290a 2020 2020 2020 2020 2020 2020  tx).            
-0000a750: 782e 636f 6d70 6c65 7465 5f64 796e 5f73  x.complete_dyn_s
-0000a760: 697a 6528 7465 6d70 6c61 7465 5f6f 6e6c  ize(template_onl
-0000a770: 793d 7465 6d70 6c61 7465 5f6f 6e6c 7929  y=template_only)
-0000a780: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000a790: 6e6f 7420 782e 6479 6e5f 7369 7a65 5f65  not x.dyn_size_e
-0000a7a0: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
-0000a7b0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000a7c0: 2020 2020 2020 2078 203d 2078 2e64 796e         x = x.dyn
-0000a7d0: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
-0000a7e0: 2020 2020 2020 6966 2079 2069 7320 4e6f        if y is No
-0000a7f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000a800: 2020 2020 7920 3d20 782e 636f 7079 286e      y = x.copy(n
-0000a810: 616d 653d 795f 6e61 6d65 290a 2020 2020  ame=y_name).    
-0000a820: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0000a830: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-0000a840: 2069 6620 782e 6469 6d5f 7461 6773 2021   if x.dim_tags !
-0000a850: 3d20 792e 6469 6d5f 7461 6773 3a0a 2020  = y.dim_tags:.  
-0000a860: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000a870: 6d6d 6f6e 203d 205f 742e 5465 6e73 6f72  mmon = _t.Tensor
-0000a880: 2e67 6574 5f63 6f6d 6d6f 6e5f 6461 7461  .get_common_data
-0000a890: 285b 782c 2079 5d2c 2061 6c6c 6f77 5f62  ([x, y], allow_b
-0000a8a0: 726f 6164 6361 7374 5f61 6c6c 5f73 6f75  roadcast_all_sou
-0000a8b0: 7263 6573 3d54 7275 6529 0a20 2020 2020  rces=True).     
-0000a8c0: 2020 2020 2020 2020 2020 2078 5f20 3d20             x_ = 
-0000a8d0: 782e 636f 7079 5f63 6f6d 7061 7469 626c  x.copy_compatibl
-0000a8e0: 655f 746f 2863 6f6d 6d6f 6e29 2069 6620  e_to(common) if 
-0000a8f0: 782e 6469 6d5f 7461 6773 2065 6c73 6520  x.dim_tags else 
-0000a900: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
-0000a910: 2020 795f 203d 2079 2e63 6f70 795f 636f    y_ = y.copy_co
-0000a920: 6d70 6174 6962 6c65 5f74 6f28 636f 6d6d  mpatible_to(comm
-0000a930: 6f6e 2920 6966 2079 2e64 696d 5f74 6167  on) if y.dim_tag
-0000a940: 7320 656c 7365 2079 0a20 2020 2020 2020  s else y.       
-0000a950: 2020 2020 2020 2020 2079 203d 2063 6f6d           y = com
-0000a960: 6d6f 6e0a 2020 2020 2020 2020 2020 2020  mon.            
-0000a970: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000a980: 2020 2020 2020 785f 2c20 795f 203d 2078        x_, y_ = x
-0000a990: 2c20 790a 2020 2020 2020 2020 2020 2020  , y.            
-0000a9a0: 6966 2074 663a 0a20 2020 2020 2020 2020  if tf:.         
-0000a9b0: 2020 2020 2020 2079 2e70 6c61 6365 686f         y.placeho
-0000a9c0: 6c64 6572 203d 205f 6269 6e5f 6f70 5f74  lder = _bin_op_t
-0000a9d0: 6628 795f 2e70 6c61 6365 686f 6c64 6572  f(y_.placeholder
-0000a9e0: 2c20 785f 2e70 6c61 6365 686f 6c64 6572  , x_.placeholder
-0000a9f0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0000aa00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000aa10: 2020 2020 7920 3d20 5f62 696e 5f6f 7028      y = _bin_op(
-0000aa20: 795f 2c20 785f 290a 2020 2020 2020 2020  y_, x_).        
-0000aa30: 6173 7365 7274 2079 2c20 6622 6f70 207b  assert y, f"op {
-0000aa40: 6f70 7d3f 220a 2020 2020 2020 2020 6966  op}?".        if
-0000aa50: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-0000aa60: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
-0000aa70: 6173 7365 7274 2073 656c 662e 6479 6e5f  assert self.dyn_
-0000aa80: 7369 7a65 5f65 7874 2e64 696d 5f74 6167  size_ext.dim_tag
-0000aa90: 7320 3d3d 2079 2e64 696d 5f74 6167 730a  s == y.dim_tags.
-0000aaa0: 2020 2020 2020 2020 6966 2079 2e62 6174          if y.bat
-0000aab0: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-0000aac0: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
-0000aad0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000aae0: 7373 6572 7420 7365 6c66 2e62 6174 6368  ssert self.batch
-0000aaf0: 203d 3d20 792e 6261 7463 680a 2020 2020   == y.batch.    
-0000ab00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ab10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ab20: 6c66 2e62 6174 6368 203d 2079 2e62 6174  lf.batch = y.bat
-0000ab30: 6368 0a20 2020 2020 2020 2073 656c 662e  ch.        self.
-0000ab40: 6479 6e5f 7369 7a65 5f65 7874 203d 2079  dyn_size_ext = y
-0000ab50: 0a20 2020 2020 2020 2069 6620 7466 2061  .        if tf a
-0000ab60: 6e64 2079 2e70 6c61 6365 686f 6c64 6572  nd y.placeholder
-0000ab70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000ab80: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000ab90: 6574 5f74 6167 5f6f 6e5f 7369 7a65 5f74  et_tag_on_size_t
-0000aba0: 656e 736f 7228 792e 706c 6163 6568 6f6c  ensor(y.placehol
-0000abb0: 6465 7229 0a0a 2020 2020 6465 6620 6973  der)..    def is
-0000abc0: 5f65 7175 616c 280a 2020 2020 2020 2020  _equal(.        
-0000abd0: 7365 6c66 2c0a 2020 2020 2020 2020 6f74  self,.        ot
-0000abe0: 6865 722c 0a20 2020 2020 2020 2069 676e  her,.        ign
-0000abf0: 6f72 655f 6665 6174 7572 655f 6469 6d3d  ore_feature_dim=
-0000ac00: 4661 6c73 652c 0a20 2020 2020 2020 2061  False,.        a
-0000ac10: 6c6c 6f77 5f73 616d 655f 6665 6174 7572  llow_same_featur
-0000ac20: 655f 6469 6d3d 4661 6c73 652c 0a20 2020  e_dim=False,.   
-0000ac30: 2020 2020 2061 6c6c 6f77 5f73 616d 655f       allow_same_
-0000ac40: 7370 6174 6961 6c5f 6469 6d3d 4e6f 6e65  spatial_dim=None
-0000ac50: 2c0a 2020 2020 2020 2020 7472 6561 745f  ,.        treat_
-0000ac60: 6665 6174 7572 655f 6173 5f73 7061 7469  feature_as_spati
-0000ac70: 616c 3d46 616c 7365 2c0a 2020 2020 2020  al=False,.      
-0000ac80: 2020 6272 6f61 6463 6173 745f 6d61 7463    broadcast_matc
-0000ac90: 6865 733d 4661 6c73 652c 0a20 2020 2020  hes=False,.     
-0000aca0: 2020 2075 6e6b 6e6f 776e 5f73 7061 7469     unknown_spati
-0000acb0: 616c 5f6d 6174 6368 6573 3d46 616c 7365  al_matches=False
-0000acc0: 2c0a 2020 2020 2020 2020 756e 6465 6669  ,.        undefi
-0000acd0: 6e65 645f 6d61 7463 6865 733d 4661 6c73  ned_matches=Fals
-0000ace0: 652c 0a20 2020 2020 2020 2064 6572 6976  e,.        deriv
-0000acf0: 6564 5f6d 6174 6368 6573 3d46 616c 7365  ed_matches=False
-0000ad00: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0000ad10: 2022 2222 0a20 2020 2020 2020 2043 6f6d   """.        Com
-0000ad20: 7061 7265 7320 7365 6c66 2074 6f20 6f74  pares self to ot
-0000ad30: 6865 7220 666f 7220 6571 7561 6c69 7479  her for equality
-0000ad40: 2e0a 0a20 2020 2020 2020 204e 6f74 6520  ...        Note 
-0000ad50: 7468 6174 2074 6865 2064 6566 6175 6c74  that the default
-0000ad60: 2062 6568 6176 696f 7220 6973 2076 6572   behavior is ver
-0000ad70: 7920 7265 7374 7269 6374 6976 652e 0a20  y restrictive.. 
-0000ad80: 2020 2020 2020 2055 7365 2066 756e 6374         Use funct
-0000ad90: 696f 6e73 2073 7563 6820 6173 203a 6675  ions such as :fu
-0000ada0: 6e63 3a60 6765 745f 616c 6c5f 6469 6d65  nc:`get_all_dime
-0000adb0: 6e73 696f 6e5f 7461 6773 6020 6f72 203a  nsion_tags` or :
-0000adc0: 6675 6e63 3a60 6765 745f 6578 6973 7469  func:`get_existi
-0000add0: 6e67 5f74 6167 5f66 726f 6d5f 636f 6c6c  ng_tag_from_coll
-0000ade0: 6563 7469 6f6e 600a 2020 2020 2020 2020  ection`.        
-0000adf0: 746f 2065 7870 6c69 6369 746c 7920 7370  to explicitly sp
-0000ae00: 6563 6966 7920 7468 6520 6265 6861 7669  ecify the behavi
-0000ae10: 6f72 2066 6f72 2074 6865 2063 6f6d 7061  or for the compa
-0000ae20: 7269 736f 6e2e 0a0a 2020 2020 2020 2020  rison...        
-0000ae30: 416c 736f 206e 6f74 6520 7468 6174 2074  Also note that t
-0000ae40: 6865 2064 6566 696e 6974 696f 6e20 6973  he definition is
-0000ae50: 2073 6c69 6768 746c 7920 6164 2d68 6f63   slightly ad-hoc
-0000ae60: 2066 6f72 2073 6f6d 6520 6361 7365 732c   for some cases,
-0000ae70: 0a20 2020 2020 2020 2061 6e64 206d 6967  .        and mig
-0000ae80: 6874 2070 6f74 656e 7469 616c 6c79 2063  ht potentially c
-0000ae90: 6861 6e67 6520 696e 2074 6865 2066 7574  hange in the fut
-0000aea0: 7572 652e 0a20 2020 2020 2020 2020 2068  ure..          h
-0000aeb0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000aec0: 6d2f 7277 7468 2d69 362f 7265 7475 726e  m/rwth-i6/return
-0000aed0: 6e2f 6973 7375 6573 2f36 3334 0a0a 2020  n/issues/634..  
-0000aee0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-0000aef0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
-0000af00: 3a70 6172 616d 2062 6f6f 6c20 6967 6e6f  :param bool igno
-0000af10: 7265 5f66 6561 7475 7265 5f64 696d 3a0a  re_feature_dim:.
-0000af20: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
-0000af30: 6f6f 6c20 616c 6c6f 775f 7361 6d65 5f66  ool allow_same_f
-0000af40: 6561 7475 7265 5f64 696d 3a0a 2020 2020  eature_dim:.    
-0000af50: 2020 2020 3a70 6172 616d 2062 6f6f 6c7c      :param bool|
-0000af60: 4e6f 6e65 2061 6c6c 6f77 5f73 616d 655f  None allow_same_
-0000af70: 7370 6174 6961 6c5f 6469 6d3a 0a20 2020  spatial_dim:.   
-0000af80: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
-0000af90: 2074 7265 6174 5f66 6561 7475 7265 5f61   treat_feature_a
-0000afa0: 735f 7370 6174 6961 6c3a 0a20 2020 2020  s_spatial:.     
-0000afb0: 2020 203a 7061 7261 6d20 626f 6f6c 2062     :param bool b
-0000afc0: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
-0000afd0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-0000afe0: 2062 6f6f 6c20 756e 6b6e 6f77 6e5f 7370   bool unknown_sp
-0000aff0: 6174 6961 6c5f 6d61 7463 6865 733a 0a20  atial_matches:. 
-0000b000: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
-0000b010: 6f6c 2075 6e64 6566 696e 6564 5f6d 6174  ol undefined_mat
-0000b020: 6368 6573 3a0a 2020 2020 2020 2020 3a70  ches:.        :p
-0000b030: 6172 616d 2062 6f6f 6c20 6465 7269 7665  aram bool derive
-0000b040: 645f 6d61 7463 6865 733a 0a20 2020 2020  d_matches:.     
-0000b050: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-0000b060: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000b070: 2020 2020 6672 6f6d 2072 6574 7572 6e6e      from returnn
-0000b080: 2e75 7469 6c20 696d 706f 7274 2042 6568  .util import Beh
-0000b090: 6176 696f 7256 6572 7369 6f6e 0a0a 2020  aviorVersion..  
-0000b0a0: 2020 2020 2020 6966 2073 656c 6620 6973        if self is
-0000b0b0: 206f 7468 6572 3a20 2023 2066 6972 7374   other:  # first
-0000b0c0: 2073 6f6d 6520 6661 7374 2070 6174 6820   some fast path 
-0000b0d0: 6368 6563 6b0a 2020 2020 2020 2020 2020  check.          
-0000b0e0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0000b0f0: 2020 2020 2020 6966 2073 656c 662e 7370        if self.sp
-0000b100: 6563 6961 6c20 6f72 206f 7468 6572 2e73  ecial or other.s
-0000b110: 7065 6369 616c 3a0a 2020 2020 2020 2020  pecial:.        
-0000b120: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0000b130: 2020 2320 6f6e 6c79 2074 7275 6520 6966    # only true if
-0000b140: 2073 616d 6520 696e 7374 616e 6365 2c20   same instance, 
-0000b150: 6368 6563 6b20 6162 6f76 650a 2020 2020  check above.    
-0000b160: 2020 2020 6966 2061 6c6c 6f77 5f73 616d      if allow_sam
-0000b170: 655f 7370 6174 6961 6c5f 6469 6d20 6973  e_spatial_dim is
-0000b180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000b190: 2020 2061 6c6c 6f77 5f73 616d 655f 7370     allow_same_sp
-0000b1a0: 6174 6961 6c5f 6469 6d20 3d20 616c 6c6f  atial_dim = allo
-0000b1b0: 775f 7361 6d65 5f66 6561 7475 7265 5f64  w_same_feature_d
-0000b1c0: 696d 0a20 2020 2020 2020 2073 656c 665f  im.        self_
-0000b1d0: 6261 7365 203d 2073 656c 662e 6765 745f  base = self.get_
-0000b1e0: 7361 6d65 5f64 6572 6976 6564 5f62 6173  same_derived_bas
-0000b1f0: 6528 2920 6966 2064 6572 6976 6564 5f6d  e() if derived_m
-0000b200: 6174 6368 6573 2065 6c73 6520 7365 6c66  atches else self
-0000b210: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
-0000b220: 0a20 2020 2020 2020 206f 7468 6572 5f62  .        other_b
-0000b230: 6173 6520 3d20 6f74 6865 722e 6765 745f  ase = other.get_
-0000b240: 7361 6d65 5f64 6572 6976 6564 5f62 6173  same_derived_bas
-0000b250: 6528 2920 6966 2064 6572 6976 6564 5f6d  e() if derived_m
-0000b260: 6174 6368 6573 2065 6c73 6520 6f74 6865  atches else othe
-0000b270: 722e 6765 745f 7361 6d65 5f62 6173 6528  r.get_same_base(
-0000b280: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000b290: 665f 6261 7365 2069 7320 6f74 6865 725f  f_base is other_
-0000b2a0: 6261 7365 3a0a 2020 2020 2020 2020 2020  base:.          
-0000b2b0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0000b2c0: 2020 2020 2020 6966 2073 656c 665f 6261        if self_ba
-0000b2d0: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
-0000b2e0: 6f70 2061 6e64 206f 7468 6572 5f62 6173  op and other_bas
-0000b2f0: 652e 6465 7269 7665 645f 6672 6f6d 5f6f  e.derived_from_o
-0000b300: 703a 0a20 2020 2020 2020 2020 2020 2069  p:.            i
-0000b310: 6620 7365 6c66 5f62 6173 652e 6465 7269  f self_base.deri
-0000b320: 7665 645f 6672 6f6d 5f6f 7020 3d3d 206f  ved_from_op == o
-0000b330: 7468 6572 5f62 6173 652e 6465 7269 7665  ther_base.derive
-0000b340: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
-0000b350: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b360: 6e20 5472 7565 0a20 2020 2020 2020 2073  n True.        s
-0000b370: 656c 665f 6b69 6e64 203d 2073 656c 662e  elf_kind = self.
-0000b380: 6b69 6e64 0a20 2020 2020 2020 206f 7468  kind.        oth
-0000b390: 6572 5f6b 696e 6420 3d20 6f74 6865 722e  er_kind = other.
-0000b3a0: 6b69 6e64 0a20 2020 2020 2020 2069 6620  kind.        if 
-0000b3b0: 7365 6c66 5f6b 696e 6420 3d3d 206f 7468  self_kind == oth
-0000b3c0: 6572 5f6b 696e 6420 3d3d 2044 696d 5479  er_kind == DimTy
-0000b3d0: 7065 732e 4665 6174 7572 6520 616e 6420  pes.Feature and 
-0000b3e0: 6967 6e6f 7265 5f66 6561 7475 7265 5f64  ignore_feature_d
-0000b3f0: 696d 3a0a 2020 2020 2020 2020 2020 2020  im:.            
-0000b400: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000b410: 2020 2020 6966 2074 7265 6174 5f66 6561      if treat_fea
-0000b420: 7475 7265 5f61 735f 7370 6174 6961 6c3a  ture_as_spatial:
-0000b430: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
-0000b440: 6f74 653a 204e 6f20 6b69 6e64 2061 7420  ote: No kind at 
-0000b450: 616c 6c3a 2052 6569 6e74 6572 7072 6574  all: Reinterpret
-0000b460: 2074 7265 6174 5f66 6561 7475 7265 5f61   treat_feature_a
-0000b470: 735f 7370 6174 6961 6c20 6120 6269 743a  s_spatial a bit:
-0000b480: 0a20 2020 2020 2020 2020 2020 2023 2041  .            # A
-0000b490: 7373 756d 6520 7468 6174 2077 6520 7761  ssume that we wa
-0000b4a0: 6e74 2074 6865 6d20 616c 6c20 746f 2062  nt them all to b
-0000b4b0: 6520 6861 6e64 6c65 6420 7468 6520 7361  e handled the sa
-0000b4c0: 6d65 2c20 6e6f 206d 6174 7465 7220 7468  me, no matter th
-0000b4d0: 6520 6b69 6e64 2e0a 2020 2020 2020 2020  e kind..        
-0000b4e0: 2020 2020 2320 2845 7863 6570 7420 6f66      # (Except of
-0000b4f0: 2062 6174 6368 2064 696d 206b 696e 642c   batch dim kind,
-0000b500: 2077 6869 6368 2069 7320 7374 696c 6c20   which is still 
-0000b510: 6578 636c 7564 6564 2068 6572 652e 290a  excluded here.).
-0000b520: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000b530: 656c 665f 6b69 6e64 203d 3d20 4469 6d54  elf_kind == DimT
-0000b540: 7970 6573 2e46 6561 7475 7265 206f 7220  ypes.Feature or 
-0000b550: 6e6f 7420 7365 6c66 5f6b 696e 643a 0a20  not self_kind:. 
-0000b560: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b570: 656c 665f 6b69 6e64 203d 2044 696d 5479  elf_kind = DimTy
-0000b580: 7065 732e 5370 6174 6961 6c0a 2020 2020  pes.Spatial.    
-0000b590: 2020 2020 2020 2020 6966 206f 7468 6572          if other
-0000b5a0: 5f6b 696e 6420 3d3d 2044 696d 5479 7065  _kind == DimType
-0000b5b0: 732e 4665 6174 7572 6520 6f72 206e 6f74  s.Feature or not
-0000b5c0: 206f 7468 6572 5f6b 696e 643a 0a20 2020   other_kind:.   
-0000b5d0: 2020 2020 2020 2020 2020 2020 206f 7468               oth
-0000b5e0: 6572 5f6b 696e 6420 3d20 4469 6d54 7970  er_kind = DimTyp
-0000b5f0: 6573 2e53 7061 7469 616c 0a20 2020 2020  es.Spatial.     
-0000b600: 2020 2069 6620 7365 6c66 2e64 696d 656e     if self.dimen
-0000b610: 7369 6f6e 2021 3d20 6f74 6865 722e 6469  sion != other.di
-0000b620: 6d65 6e73 696f 6e3a 0a20 2020 2020 2020  mension:.       
-0000b630: 2020 2020 2069 6620 6272 6f61 6463 6173       if broadcas
-0000b640: 745f 6d61 7463 6865 7320 616e 6420 2873  t_matches and (s
-0000b650: 656c 662e 6469 6d65 6e73 696f 6e20 3d3d  elf.dimension ==
-0000b660: 2031 206f 7220 6f74 6865 722e 6469 6d65   1 or other.dime
-0000b670: 6e73 696f 6e20 3d3d 2031 293a 0a20 2020  nsion == 1):.   
-0000b680: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-0000b690: 7320 2023 2070 6173 7320 6f6e 0a20 2020  s  # pass on.   
-0000b6a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000b6c0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-0000b6d0: 2020 2020 6966 2073 656c 665f 6b69 6e64      if self_kind
-0000b6e0: 2021 3d20 6f74 6865 725f 6b69 6e64 3a0a   != other_kind:.
-0000b6f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000b700: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0000b710: 2069 6620 7365 6c66 5f6b 696e 6420 3d3d   if self_kind ==
-0000b720: 206f 7468 6572 5f6b 696e 6420 3d3d 2044   other_kind == D
-0000b730: 696d 5479 7065 732e 4261 7463 683a 0a20  imTypes.Batch:. 
-0000b740: 2020 2020 2020 2020 2020 2023 204e 6f74             # Not
-0000b750: 653a 2054 6869 7320 6d69 6768 7420 6265  e: This might be
-0000b760: 2069 6e63 6f72 7265 6374 2069 6e20 736f   incorrect in so
-0000b770: 6d65 2063 6173 6573 2c0a 2020 2020 2020  me cases,.      
-0000b780: 2020 2020 2020 2320 652e 672e 2066 6f72        # e.g. for
-0000b790: 2062 6561 6d20 7365 6172 6368 2077 6865   beam search whe
-0000b7a0: 6e20 7765 2068 6176 6520 7468 6520 6265  n we have the be
-0000b7b0: 616d 2068 6964 6465 6e20 696e 2074 6865  am hidden in the
-0000b7c0: 2062 6174 6368 2064 696d 2c0a 2020 2020   batch dim,.    
-0000b7d0: 2020 2020 2020 2020 2320 6f72 2077 6865          # or whe
-0000b7e0: 6e20 7765 2075 7365 6420 4d65 7267 6544  n we used MergeD
-0000b7f0: 696d 734c 6179 6572 206f 6e20 7468 6520  imsLayer on the 
-0000b800: 6261 7463 6820 6178 6973 2c20 6f72 2073  batch axis, or s
-0000b810: 6f2e 0a20 2020 2020 2020 2020 2020 2023  o..            #
-0000b820: 2057 6520 6d69 6768 7420 6e65 6564 2074   We might need t
-0000b830: 6f20 6578 7465 6e64 2074 6865 206c 6f67  o extend the log
-0000b840: 6963 2068 6572 6520 6c61 7465 722e 0a20  ic here later.. 
-0000b850: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b860: 6e20 5472 7565 0a20 2020 2020 2020 2069  n True.        i
-0000b870: 6620 4265 6861 7669 6f72 5665 7273 696f  f BehaviorVersio
-0000b880: 6e2e 6765 7428 2920 3e3d 2031 363a 0a20  n.get() >= 16:. 
-0000b890: 2020 2020 2020 2020 2020 2023 2045 6974             # Eit
-0000b8a0: 6865 7220 7365 6c66 206f 7220 6f74 6865  her self or othe
-0000b8b0: 7220 6973 2073 6f6d 6520 6469 6d20 7461  r is some dim ta
-0000b8c0: 6720 6578 706c 6963 6974 6c79 2063 7265  g explicitly cre
-0000b8d0: 6174 6564 2062 7920 7468 6520 7573 6572  ated by the user
-0000b8e0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-0000b8f0: 616e 6420 7468 6579 2061 7265 206e 6f74  and they are not
-0000b900: 2074 6865 2073 616d 652c 2073 6f20 7765   the same, so we
-0000b910: 206e 6576 6572 2074 7265 6174 2074 6865   never treat the
-0000b920: 6d20 6173 2065 7175 616c 2e0a 2020 2020  m as equal..    
-0000b930: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-0000b940: 656c 662e 6175 746f 5f67 656e 6572 6174  elf.auto_generat
-0000b950: 6564 206f 7220 6e6f 7420 6f74 6865 722e  ed or not other.
-0000b960: 6175 746f 5f67 656e 6572 6174 6564 3a0a  auto_generated:.
-0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b980: 6966 2062 726f 6164 6361 7374 5f6d 6174  if broadcast_mat
-0000b990: 6368 6573 2061 6e64 2028 0a20 2020 2020  ches and (.     
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0000b9b0: 7365 6c66 2e64 696d 656e 7369 6f6e 203d  self.dimension =
-0000b9c0: 3d20 3120 616e 6420 7365 6c66 2e61 7574  = 1 and self.aut
-0000b9d0: 6f5f 6765 6e65 7261 7465 6429 206f 7220  o_generated) or 
-0000b9e0: 286f 7468 6572 2e64 696d 656e 7369 6f6e  (other.dimension
-0000b9f0: 203d 3d20 3120 616e 6420 6f74 6865 722e   == 1 and other.
-0000ba00: 6175 746f 5f67 656e 6572 6174 6564 290a  auto_generated).
+00008980: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089a0: 2020 2020 2520 2873 656c 662c 2073 656c      % (self, sel
+000089b0: 662e 6465 7363 7269 7074 696f 6e2c 2073  f.description, s
+000089c0: 656c 662e 6479 6e5f 7369 7a65 2c20 782c  elf.dyn_size, x,
+000089d0: 2062 6174 6368 292c 0a20 2020 2020 2020   batch),.       
+000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089f0: 2020 2020 2022 5c6e 4e65 7720 7369 7a65       "\nNew size
+00008a00: 2063 6f6d 7075 7461 7469 6f6e 2067 7261   computation gra
+00008a10: 7068 3a22 2c0a 2020 2020 2020 2020 2020  ph:",.          
+00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a30: 2020 6765 745f 6261 636b 656e 645f 6279    get_backend_by
+00008a40: 5f72 6177 5f74 656e 736f 725f 7479 7065  _raw_tensor_type
+00008a50: 2874 7970 6528 7829 292e 666f 726d 6174  (type(x)).format
+00008a60: 5f67 7261 7068 5f6f 7574 7075 7428 782c  _graph_output(x,
+00008a70: 206d 6178 5f64 6570 7468 3d33 292c 0a20   max_depth=3),. 
+00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a90: 2020 2020 2020 2020 2020 2022 5c6e 5468             "\nTh
+00008aa0: 6973 2069 7320 6d61 7962 6520 7468 6520  is is maybe the 
+00008ab0: 7265 7375 6c74 206f 6620 616e 2069 6e63  result of an inc
+00008ac0: 6f72 7265 6374 2064 6563 6c61 7265 5f73  orrect declare_s
+00008ad0: 616d 655f 6173 2e20 222c 0a20 2020 2020  ame_as. ",.     
+00008ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008af0: 2020 2020 2020 2022 7361 6d65 5f61 7320         "same_as 
+00008b00: 3d20 2573 2220 2520 7365 6c66 2e73 616d  = %s" % self.sam
+00008b10: 655f 6173 2c0a 2020 2020 2020 2020 2020  e_as,.          
+00008b20: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
+00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b40: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00008b50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00008b60: 6966 2062 6174 6368 2061 6e64 2067 6574  if batch and get
+00008b70: 6174 7472 2878 2c20 225f 5245 5455 524e  attr(x, "_RETURN
+00008b80: 4e5f 6479 6e5f 7369 7a65 5f62 6561 6d22  N_dyn_size_beam"
+00008b90: 2c20 4e6f 6e65 293a 0a20 2020 2020 2020  , None):.       
+00008ba0: 2020 2020 2061 7373 6572 7420 6261 7463       assert batc
+00008bb0: 682e 6265 616d 203d 3d20 6765 7461 7474  h.beam == getatt
+00008bc0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00008bd0: 2020 2078 2c20 225f 5245 5455 524e 4e5f     x, "_RETURNN_
+00008be0: 6479 6e5f 7369 7a65 5f62 6561 6d22 0a20  dyn_size_beam". 
+00008bf0: 2020 2020 2020 2020 2020 2029 2c20 2225             ), "%
+00008c00: 733a 2064 796e 2073 697a 6520 2573 2068  s: dyn size %s h
+00008c10: 6173 2075 6e65 7870 6563 7465 6420 6261  as unexpected ba
+00008c20: 7463 6820 2573 2c20 6578 7065 6374 6564  tch %s, expected
+00008c30: 2025 7322 2025 2028 0a20 2020 2020 2020   %s" % (.       
+00008c40: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00008c50: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00008c60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008c70: 2020 6261 7463 682c 0a20 2020 2020 2020    batch,.       
+00008c80: 2020 2020 2020 2020 2067 6574 6174 7472           getattr
+00008c90: 2878 2c20 225f 5245 5455 524e 4e5f 6479  (x, "_RETURNN_dy
+00008ca0: 6e5f 7369 7a65 5f62 6561 6d22 292c 0a20  n_size_beam"),. 
+00008cb0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00008cc0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
+00008cd0: 6368 2061 6e64 2062 6174 6368 3a0a 2020  ch and batch:.  
+00008ce0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00008cf0: 2073 656c 662e 6261 7463 6820 3d3d 2062   self.batch == b
+00008d00: 6174 6368 0a20 2020 2020 2020 2065 6c69  atch.        eli
+00008d10: 6620 6261 7463 6820 616e 6420 6e6f 7420  f batch and not 
+00008d20: 7365 6c66 2e62 6174 6368 3a0a 2020 2020  self.batch:.    
+00008d30: 2020 2020 2020 2020 7365 6c66 2e62 6174          self.bat
+00008d40: 6368 203d 2062 6174 6368 2020 2320 6f76  ch = batch  # ov
+00008d50: 6572 7461 6b65 0a20 2020 2020 2020 2069  ertake.        i
+00008d60: 6620 6e6f 7420 7365 6c66 2e69 735f 6261  f not self.is_ba
+00008d70: 7463 685f 6469 6d28 2920 616e 6420 7365  tch_dim() and se
+00008d80: 6c66 2e69 735f 6479 6e61 6d69 6328 293a  lf.is_dynamic():
+00008d90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00008da0: 7361 6d65 5f61 735f 6265 666f 7265 3a0a  same_as_before:.
+00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dc0: 6173 7365 7274 2073 656c 662e 6479 6e5f  assert self.dyn_
+00008dd0: 7369 7a65 5f65 7874 2061 6e64 2073 656c  size_ext and sel
+00008de0: 662e 6479 6e5f 7369 7a65 5f65 7874 2e70  f.dyn_size_ext.p
+00008df0: 6c61 6365 686f 6c64 6572 2069 7320 6e6f  laceholder is no
+00008e00: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
+00008e10: 2020 2020 2020 2023 2044 6f20 6e6f 7420         # Do not 
+00008e20: 6f76 6572 7772 6974 6520 6974 2e0a 2020  overwrite it..  
+00008e30: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e50: 7365 6c66 2e5f 696e 6974 5f64 6566 6175  self._init_defau
+00008e60: 6c74 5f64 796e 5f73 697a 655f 6578 7428  lt_dyn_size_ext(
+00008e70: 7829 0a20 2020 2020 2020 2069 6620 6765  x).        if ge
+00008e80: 7461 7474 7228 782c 2022 5f69 735f 7369  tattr(x, "_is_si
+00008e90: 7a65 5f6f 665f 6469 6d5f 7461 6722 2c20  ze_of_dim_tag", 
+00008ea0: 4e6f 6e65 2920 6973 204e 6f6e 653a 0a20  None) is None:. 
+00008eb0: 2020 2020 2020 2020 2020 2073 6574 6174             setat
+00008ec0: 7472 2878 2c20 225f 6973 5f73 697a 655f  tr(x, "_is_size_
+00008ed0: 6f66 5f64 696d 5f74 6167 222c 2073 656c  of_dim_tag", sel
+00008ee0: 6629 0a20 2020 2020 2020 2072 6574 7572  f).        retur
+00008ef0: 6e20 7365 6c66 0a0a 2020 2020 4063 6c61  n self..    @cla
+00008f00: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00008f10: 2067 6574 5f74 6167 5f66 726f 6d5f 7369   get_tag_from_si
+00008f20: 7a65 5f74 656e 736f 7228 636c 732c 2078  ze_tensor(cls, x
+00008f30: 2920 2d3e 204f 7074 696f 6e61 6c5b 5f64  ) -> Optional[_d
+00008f40: 2e44 696d 5d3a 0a20 2020 2020 2020 2022  .Dim]:.        "
+00008f50: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00008f60: 6d20 7466 2e54 656e 736f 7220 783a 2073  m tf.Tensor x: s
+00008f70: 697a 6520 7465 6e73 6f72 2e20 6861 7320  ize tensor. has 
+00008f80: 6265 656e 2073 6574 2062 6566 6f72 6520  been set before 
+00008f90: 7669 6120 3a66 756e 633a 6073 6574 5f74  via :func:`set_t
+00008fa0: 6167 5f6f 6e5f 7369 7a65 5f74 656e 736f  ag_on_size_tenso
+00008fb0: 7260 0a20 2020 2020 2020 2022 2222 0a20  r`.        """. 
+00008fc0: 2020 2020 2020 2072 6574 7572 6e20 6765         return ge
+00008fd0: 7461 7474 7228 782c 2022 5f69 735f 7369  tattr(x, "_is_si
+00008fe0: 7a65 5f6f 665f 6469 6d5f 7461 6722 2c20  ze_of_dim_tag", 
+00008ff0: 4e6f 6e65 290a 0a20 2020 2064 6566 2063  None)..    def c
+00009000: 6f6d 706c 6574 655f 6479 6e5f 7369 7a65  omplete_dyn_size
+00009010: 2873 656c 662c 2074 656d 706c 6174 655f  (self, template_
+00009020: 6f6e 6c79 3d46 616c 7365 293a 0a20 2020  only=False):.   
+00009030: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00009040: 2049 6e20 6361 7365 2077 6520 6361 6e20   In case we can 
+00009050: 6361 6c63 756c 6174 6520 7468 6520 6479  calculate the dy
+00009060: 6e20 7369 7a65 2c20 646f 2074 6861 7420  n size, do that 
+00009070: 6e6f 772e 0a0a 2020 2020 2020 2020 3a70  now...        :p
+00009080: 6172 616d 2062 6f6f 6c20 7465 6d70 6c61  aram bool templa
+00009090: 7465 5f6f 6e6c 793a 0a20 2020 2020 2020  te_only:.       
+000090a0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+000090b0: 6e6f 7420 7365 6c66 2e69 735f 6479 6e61  not self.is_dyna
+000090c0: 6d69 6328 293a 0a20 2020 2020 2020 2020  mic():.         
+000090d0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+000090e0: 2020 7365 6c66 2e5f 7661 6c69 6461 7465    self._validate
+000090f0: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
+00009100: 6828 290a 2020 2020 2020 2020 6966 2073  h().        if s
+00009110: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00009120: 2061 6e64 2028 7365 6c66 2e64 796e 5f73   and (self.dyn_s
+00009130: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
+00009140: 6465 7220 6973 206e 6f74 204e 6f6e 6520  der is not None 
+00009150: 6f72 2074 656d 706c 6174 655f 6f6e 6c79  or template_only
+00009160: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00009170: 6574 7572 6e0a 2020 2020 2020 2020 7361  eturn.        sa
+00009180: 6d65 5f62 6173 6520 3d20 7365 6c66 2e67  me_base = self.g
+00009190: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
+000091a0: 2020 2020 2020 206f 7020 3d20 7365 6c66         op = self
+000091b0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+000091c0: 206f 7220 7361 6d65 5f62 6173 652e 6465   or same_base.de
+000091d0: 7269 7665 645f 6672 6f6d 5f6f 700a 2020  rived_from_op.  
+000091e0: 2020 2020 2020 6966 206e 6f74 206f 703a        if not op:
+000091f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009200: 7572 6e0a 0a20 2020 2020 2020 2066 6f72  urn..        for
+00009210: 2078 2069 6e20 6f70 2e69 6e70 7574 733a   x in op.inputs:
+00009220: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009230: 7365 6c66 2e62 6174 6368 3a0a 2020 2020  self.batch:.    
+00009240: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+00009250: 782e 6765 745f 666f 725f 6261 7463 685f  x.get_for_batch_
+00009260: 6374 7828 7365 6c66 2e62 6174 6368 2c20  ctx(self.batch, 
+00009270: 7365 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f  self.control_flo
+00009280: 775f 6374 7829 0a20 2020 2020 2020 2020  w_ctx).         
+00009290: 2020 2078 2e63 6f6d 706c 6574 655f 6479     x.complete_dy
+000092a0: 6e5f 7369 7a65 2874 656d 706c 6174 655f  n_size(template_
+000092b0: 6f6e 6c79 3d74 656d 706c 6174 655f 6f6e  only=template_on
+000092c0: 6c79 290a 0a20 2020 2020 2020 2062 6163  ly)..        bac
+000092d0: 6b65 6e64 203d 204e 6f6e 650a 2020 2020  kend = None.    
+000092e0: 2020 2020 666f 7220 7820 696e 206f 702e      for x in op.
+000092f0: 696e 7075 7473 3a0a 2020 2020 2020 2020  inputs:.        
+00009300: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
+00009310: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+00009320: 2020 2078 203d 2078 2e67 6574 5f66 6f72     x = x.get_for
+00009330: 5f62 6174 6368 5f63 7478 2873 656c 662e  _batch_ctx(self.
+00009340: 6261 7463 682c 2073 656c 662e 636f 6e74  batch, self.cont
+00009350: 726f 6c5f 666c 6f77 5f63 7478 290a 2020  rol_flow_ctx).  
+00009360: 2020 2020 2020 2020 2020 6966 2078 2e64            if x.d
+00009370: 796e 5f73 697a 655f 6578 7420 616e 6420  yn_size_ext and 
+00009380: 782e 6479 6e5f 7369 7a65 5f65 7874 2e72  x.dyn_size_ext.r
+00009390: 6177 5f74 656e 736f 7220 6973 206e 6f74  aw_tensor is not
+000093a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000093b0: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
+000093c0: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
+000093d0: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
+000093e0: 2020 2020 2020 2020 6261 636b 656e 6420          backend 
+000093f0: 3d20 782e 6479 6e5f 7369 7a65 5f65 7874  = x.dyn_size_ext
+00009400: 2e5f 7261 775f 6261 636b 656e 640a 2020  ._raw_backend.  
+00009410: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00009420: 6561 6b0a 0a20 2020 2020 2020 2073 697a  eak..        siz
+00009430: 655f 6474 7970 6520 3d20 4e6f 6e65 0a20  e_dtype = None. 
+00009440: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
+00009450: 6f70 2e69 6e70 7574 733a 0a20 2020 2020  op.inputs:.     
+00009460: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00009470: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
+00009480: 2020 2020 2020 7820 3d20 782e 6765 745f        x = x.get_
+00009490: 666f 725f 6261 7463 685f 6374 7828 7365  for_batch_ctx(se
+000094a0: 6c66 2e62 6174 6368 2c20 7365 6c66 2e63  lf.batch, self.c
+000094b0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7829  ontrol_flow_ctx)
+000094c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000094d0: 782e 6479 6e5f 7369 7a65 5f65 7874 3a0a  x.dyn_size_ext:.
+000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094f0: 7369 7a65 5f64 7479 7065 203d 2078 2e64  size_dtype = x.d
+00009500: 796e 5f73 697a 655f 6578 742e 6474 7970  yn_size_ext.dtyp
+00009510: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00009520: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+00009530: 6966 206e 6f74 2073 697a 655f 6474 7970  if not size_dtyp
+00009540: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00009550: 697a 655f 6474 7970 6520 3d20 5f74 2e54  ize_dtype = _t.T
+00009560: 656e 736f 722e 7369 7a65 5f64 7479 7065  ensor.size_dtype
+00009570: 0a0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+00009580: 206e 756d 7079 0a20 2020 2020 2020 2069   numpy.        i
+00009590: 6d70 6f72 7420 7265 7475 726e 6e2e 6672  mport returnn.fr
+000095a0: 6f6e 7465 6e64 2061 7320 7266 0a0a 2020  ontend as rf..  
+000095b0: 2020 2020 2020 7466 203d 2074 665f 7574        tf = tf_ut
+000095c0: 696c 203d 2074 656e 736f 725f 7574 696c  il = tensor_util
+000095d0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+000095e0: 6966 2062 6163 6b65 6e64 2061 6e64 2062  if backend and b
+000095f0: 6163 6b65 6e64 2e69 735f 7465 6e73 6f72  ackend.is_tensor
+00009600: 666c 6f77 3a0a 2020 2020 2020 2020 2020  flow:.          
+00009610: 2020 696d 706f 7274 2074 656e 736f 7266    import tensorf
+00009620: 6c6f 7720 6173 2074 660a 0a20 2020 2020  low as tf..     
+00009630: 2020 2020 2020 2069 6620 6261 636b 656e         if backen
+00009640: 642e 5261 7754 656e 736f 7254 7970 6520  d.RawTensorType 
+00009650: 3d3d 2074 662e 5465 6e73 6f72 3a0a 2020  == tf.Tensor:.  
+00009660: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00009670: 6f6d 2072 6574 7572 6e6e 2e74 662e 7574  om returnn.tf.ut
+00009680: 696c 2069 6d70 6f72 7420 6261 7369 6320  il import basic 
+00009690: 6173 2074 665f 7574 696c 0a20 2020 2020  as tf_util.     
+000096a0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
+000096b0: 7465 6e73 6f72 666c 6f77 2e70 7974 686f  tensorflow.pytho
+000096c0: 6e2e 6672 616d 6577 6f72 6b20 696d 706f  n.framework impo
+000096d0: 7274 2074 656e 736f 725f 7574 696c 0a20  rt tensor_util. 
+000096e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000096f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009700: 2074 6620 3d20 4e6f 6e65 0a0a 2020 2020   tf = None..    
+00009710: 2020 2020 6b69 6e64 203d 206f 702e 6b69      kind = op.ki
+00009720: 6e64 0a20 2020 2020 2020 2069 6620 6b69  nd.        if ki
+00009730: 6e64 2e65 6e64 7377 6974 6828 225f 7269  nd.endswith("_ri
+00009740: 6768 7422 293a 0a20 2020 2020 2020 2020  ght"):.         
+00009750: 2020 206b 696e 6420 3d20 6b69 6e64 5b3a     kind = kind[:
+00009760: 202d 6c65 6e28 225f 7269 6768 7422 295d   -len("_right")]
+00009770: 2020 2320 6f72 6465 7220 646f 6573 206e    # order does n
+00009780: 6f74 206d 6174 7465 7220 6865 7265 0a20  ot matter here. 
+00009790: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
+000097a0: 6e64 7377 6974 6828 225f 6c65 6674 2229  ndswith("_left")
+000097b0: 3a0a 2020 2020 2020 2020 2020 2020 6b69  :.            ki
+000097c0: 6e64 203d 206b 696e 645b 3a20 2d6c 656e  nd = kind[: -len
+000097d0: 2822 5f6c 6566 7422 295d 0a0a 2020 2020  ("_left")]..    
+000097e0: 2020 2020 6465 6620 5f69 735f 6e65 6761      def _is_nega
+000097f0: 7469 7665 2878 5f5f 293a 0a20 2020 2020  tive(x__):.     
+00009800: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00009810: 616e 6365 2878 5f5f 2c20 6e75 6d70 792e  ance(x__, numpy.
+00009820: 6e64 6172 7261 7929 3a0a 2020 2020 2020  ndarray):.      
+00009830: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009840: 2028 785f 5f20 3c20 3029 2e61 6e79 2829   (x__ < 0).any()
+00009850: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009860: 6973 696e 7374 616e 6365 2878 5f5f 2c20  isinstance(x__, 
+00009870: 2869 6e74 2c20 666c 6f61 742c 206e 756d  (int, float, num
+00009880: 7079 2e6e 756d 6265 7229 293a 0a20 2020  py.number)):.   
+00009890: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000098a0: 7572 6e20 785f 5f20 3c20 300a 2020 2020  urn x__ < 0.    
+000098b0: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
+000098c0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+000098d0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+000098e0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+000098f0: 7274 2069 7369 6e73 7461 6e63 6528 785f  rt isinstance(x_
+00009900: 5f2c 2074 662e 5465 6e73 6f72 290a 2020  _, tf.Tensor).  
+00009910: 2020 2020 2020 2020 2020 785f 5f20 3d20            x__ = 
+00009920: 7465 6e73 6f72 5f75 7469 6c2e 636f 6e73  tensor_util.cons
+00009930: 7461 6e74 5f76 616c 7565 2878 5f5f 290a  tant_value(x__).
+00009940: 2020 2020 2020 2020 2020 2020 6966 2078              if x
+00009950: 5f5f 2069 7320 6e6f 7420 4e6f 6e65 3a0a  __ is not None:.
+00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009970: 7265 7475 726e 205f 6973 5f6e 6567 6174  return _is_negat
+00009980: 6976 6528 785f 5f29 0a20 2020 2020 2020  ive(x__).       
+00009990: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000099a0: 650a 0a20 2020 2020 2020 2064 6566 205f  e..        def _
+000099b0: 6269 6e5f 6f70 5f74 6628 612c 2062 293a  bin_op_tf(a, b):
+000099c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000099d0: 7465 6d70 6c61 7465 5f6f 6e6c 793a 0a20  template_only:. 
+000099e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000099f0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
+00009a00: 2020 2020 2020 2069 6620 6120 6973 204e         if a is N
+00009a10: 6f6e 6520 6f72 2062 2069 7320 4e6f 6e65  one or b is None
+00009a20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009a30: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+00009a40: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00009a50: 2069 7369 6e73 7461 6e63 6528 612c 2074   isinstance(a, t
+00009a60: 662e 5465 6e73 6f72 2920 616e 6420 6973  f.Tensor) and is
+00009a70: 696e 7374 616e 6365 2862 2c20 2869 6e74  instance(b, (int
+00009a80: 2c20 7466 2e54 656e 736f 7229 290a 2020  , tf.Tensor)).  
+00009a90: 2020 2020 2020 2020 2020 7769 7468 2074            with t
+00009aa0: 665f 7574 696c 2e73 616d 655f 636f 6e74  f_util.same_cont
+00009ab0: 726f 6c5f 666c 6f77 5f63 7478 285b 612c  rol_flow_ctx([a,
+00009ac0: 2062 5d29 3a0a 2020 2020 2020 2020 2020   b]):.          
+00009ad0: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
+00009ae0: 2022 6164 6422 3a0a 2020 2020 2020 2020   "add":.        
+00009af0: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+00009b00: 7265 6c75 203d 205f 6973 5f6e 6567 6174  relu = _is_negat
+00009b10: 6976 6528 6129 206f 7220 5f69 735f 6e65  ive(a) or _is_ne
+00009b20: 6761 7469 7665 2862 2920 2023 2066 6f72  gative(b)  # for
+00009b30: 2064 796e 616d 6963 2074 656e 736f 7273   dynamic tensors
+00009b40: 2c20 6173 7375 6d65 2061 6c6c 2070 6f73  , assume all pos
+00009b50: 6974 6976 650a 2020 2020 2020 2020 2020  itive.          
+00009b60: 2020 2020 2020 2020 2020 6966 2075 7365            if use
+00009b70: 5f72 656c 753a 0a20 2020 2020 2020 2020  _relu:.         
+00009b80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009b90: 6574 7572 6e20 7466 2e63 6f6e 7665 7274  eturn tf.convert
+00009ba0: 5f74 6f5f 7465 6e73 6f72 2874 665f 7574  _to_tensor(tf_ut
+00009bb0: 696c 2e73 696d 706c 6966 795f 6e6f 6e5f  il.simplify_non_
+00009bc0: 6e65 6761 7469 7665 5f73 6571 5f6c 656e  negative_seq_len
+00009bd0: 6774 6828 6120 2b20 6229 290a 2020 2020  gth(a + b)).    
+00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bf0: 7265 7475 726e 2061 202b 2062 0a20 2020  return a + b.   
+00009c00: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00009c10: 6620 6b69 6e64 203d 3d20 2273 7562 223a  f kind == "sub":
+00009c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c30: 2020 2020 2072 6574 7572 6e20 7466 2e63       return tf.c
+00009c40: 6f6e 7665 7274 5f74 6f5f 7465 6e73 6f72  onvert_to_tensor
+00009c50: 2874 665f 7574 696c 2e73 696d 706c 6966  (tf_util.simplif
+00009c60: 795f 6e6f 6e5f 6e65 6761 7469 7665 5f73  y_non_negative_s
+00009c70: 6571 5f6c 656e 6774 6828 6120 2d20 6229  eq_length(a - b)
+00009c80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009c90: 2020 656c 6966 206b 696e 6420 3d3d 2022    elif kind == "
+00009ca0: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
+00009cb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009cc0: 2061 202a 2062 0a20 2020 2020 2020 2020   a * b.         
+00009cd0: 2020 2020 2020 2065 6c69 6620 6b69 6e64         elif kind
+00009ce0: 2069 6e20 2822 666c 6f6f 7264 6976 222c   in ("floordiv",
+00009cf0: 2022 7472 7565 6469 7622 293a 2020 2320   "truediv"):  # 
+00009d00: 7472 7565 6469 7620 6173 7375 6d65 7320  truediv assumes 
+00009d10: 7468 6572 6520 6973 206e 6f20 7265 6d61  there is no rema
+00009d20: 696e 6465 720a 2020 2020 2020 2020 2020  inder.          
+00009d30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009d40: 2061 202f 2f20 620a 2020 2020 2020 2020   a // b.        
+00009d50: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
+00009d60: 6420 3d3d 2022 6365 696c 6469 7622 3a0a  d == "ceildiv":.
+00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d80: 2020 2020 7265 7475 726e 202d 282d 6120      return -(-a 
+00009d90: 2f2f 2062 290a 2020 2020 2020 2020 2020  // b).          
+00009da0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009dc0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00009dd0: 2822 756e 6b6e 6f77 6e20 6f70 206b 696e  ("unknown op kin
+00009de0: 6420 2572 2220 2520 6f70 2e6b 696e 6429  d %r" % op.kind)
+00009df0: 0a0a 2020 2020 2020 2020 6465 6620 5f62  ..        def _b
+00009e00: 696e 5f6f 7028 612c 2062 293a 0a20 2020  in_op(a, b):.   
+00009e10: 2020 2020 2020 2020 2069 6620 7465 6d70           if temp
+00009e20: 6c61 7465 5f6f 6e6c 7920 6f72 206e 6f74  late_only or not
+00009e30: 2062 6163 6b65 6e64 3a0a 2020 2020 2020   backend:.      
+00009e40: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00009e50: 6e73 7461 6e63 6528 612c 205f 742e 5465  nstance(a, _t.Te
+00009e60: 6e73 6f72 2920 616e 6420 6973 696e 7374  nsor) and isinst
+00009e70: 616e 6365 2862 2c20 5f74 2e54 656e 736f  ance(b, _t.Tenso
+00009e80: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00009e90: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00009ea0: 742e 5465 6e73 6f72 2e67 6574 5f63 6f6d  t.Tensor.get_com
+00009eb0: 6d6f 6e5f 6461 7461 285b 612c 2062 5d2c  mon_data([a, b],
+00009ec0: 2061 6c6c 6f77 5f62 726f 6164 6361 7374   allow_broadcast
+00009ed0: 5f61 6c6c 5f73 6f75 7263 6573 3d54 7275  _all_sources=Tru
+00009ee0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00009ef0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00009f00: 2861 2c20 5f74 2e54 656e 736f 7229 3a0a  (a, _t.Tensor):.
+00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f20: 2020 2020 7265 7475 726e 2061 0a20 2020      return a.   
+00009f30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00009f40: 6973 696e 7374 616e 6365 2862 2c20 5f74  isinstance(b, _t
+00009f50: 2e54 656e 736f 7229 3a0a 2020 2020 2020  .Tensor):.      
+00009f60: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00009f70: 7475 726e 2062 0a20 2020 2020 2020 2020  turn b.         
+00009f80: 2020 2069 6620 6b69 6e64 203d 3d20 2261     if kind == "a
+00009f90: 6464 223a 0a20 2020 2020 2020 2020 2020  dd":.           
+00009fa0: 2020 2020 2072 6574 7572 6e20 5f72 656c       return _rel
+00009fb0: 7528 6120 2b20 6229 0a20 2020 2020 2020  u(a + b).       
+00009fc0: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
+00009fd0: 3d20 2273 7562 223a 0a20 2020 2020 2020  = "sub":.       
+00009fe0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009ff0: 5f72 656c 7528 6120 2d20 6229 0a20 2020  _relu(a - b).   
+0000a000: 2020 2020 2020 2020 2065 6c69 6620 6b69           elif ki
+0000a010: 6e64 203d 3d20 226d 756c 223a 0a20 2020  nd == "mul":.   
+0000a020: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000a030: 7572 6e20 6120 2a20 620a 2020 2020 2020  urn a * b.      
+0000a040: 2020 2020 2020 656c 6966 206b 696e 6420        elif kind 
+0000a050: 696e 2028 2266 6c6f 6f72 6469 7622 2c20  in ("floordiv", 
+0000a060: 2274 7275 6564 6976 2229 3a20 2023 2074  "truediv"):  # t
+0000a070: 7275 6564 6976 2061 7373 756d 6573 2074  ruediv assumes t
+0000a080: 6865 7265 2069 7320 6e6f 2072 656d 6169  here is no remai
+0000a090: 6e64 6572 0a20 2020 2020 2020 2020 2020  nder.           
+0000a0a0: 2020 2020 2072 6574 7572 6e20 6120 2f2f       return a //
+0000a0b0: 2062 0a20 2020 2020 2020 2020 2020 2065   b.            e
+0000a0c0: 6c69 6620 6b69 6e64 203d 3d20 2263 6569  lif kind == "cei
+0000a0d0: 6c64 6976 223a 0a20 2020 2020 2020 2020  ldiv":.         
+0000a0e0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000a0f0: 616e 6365 2861 2c20 5f74 2e54 656e 736f  ance(a, _t.Tenso
+0000a100: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0000a110: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000a120: 662e 6365 696c 5f64 6976 6964 6528 612c  f.ceil_divide(a,
+0000a130: 2062 290a 2020 2020 2020 2020 2020 2020   b).            
+0000a140: 2020 2020 7265 7475 726e 202d 282d 6120      return -(-a 
+0000a150: 2f2f 2062 290a 2020 2020 2020 2020 2020  // b).          
+0000a160: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a170: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0000a180: 6c75 6545 7272 6f72 2822 756e 6b6e 6f77  lueError("unknow
+0000a190: 6e20 6f70 206b 696e 6420 2572 2220 2520  n op kind %r" % 
+0000a1a0: 6f70 2e6b 696e 6429 0a0a 2020 2020 2020  op.kind)..      
+0000a1b0: 2020 6465 6620 5f72 656c 7528 6129 3a0a    def _relu(a):.
+0000a1c0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000a1d0: 7369 6e73 7461 6e63 6528 612c 205f 742e  sinstance(a, _t.
+0000a1e0: 5465 6e73 6f72 293a 0a20 2020 2020 2020  Tensor):.       
+0000a1f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000a200: 7266 2e72 656c 7528 6129 0a20 2020 2020  rf.relu(a).     
+0000a210: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+0000a220: 7374 616e 6365 2861 2c20 696e 7429 3a0a  stance(a, int):.
+0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a240: 7265 7475 726e 206d 6178 2861 2c20 3029  return max(a, 0)
+0000a250: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000a260: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000a270: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+0000a280: 6f72 2866 2263 6f6d 706c 6574 655f 6479  or(f"complete_dy
+0000a290: 6e5f 7369 7a65 3a20 5f72 656c 753a 2075  n_size: _relu: u
+0000a2a0: 6e65 7870 6563 7465 6420 7479 7065 207b  nexpected type {
+0000a2b0: 7479 7065 2861 297d 2229 0a0a 2020 2020  type(a)}")..    
+0000a2c0: 2020 2020 795f 6e61 6d65 203d 2073 656c      y_name = sel
+0000a2d0: 662e 6465 7363 7269 7074 696f 6e20 2b20  f.description + 
+0000a2e0: 223a 7365 712d 6c65 6e67 7468 220a 2020  ":seq-length".  
+0000a2f0: 2020 2020 2020 793a 204f 7074 696f 6e61        y: Optiona
+0000a300: 6c5b 5f74 2e54 656e 736f 725d 203d 204e  l[_t.Tensor] = N
+0000a310: 6f6e 6520 2023 2072 6573 756c 7469 6e67  one  # resulting
+0000a320: 2064 796e 2073 697a 650a 2020 2020 2020   dyn size.      
+0000a330: 2020 696e 7075 7473 203d 206c 6973 7428    inputs = list(
+0000a340: 6f70 2e69 6e70 7574 7329 0a20 2020 2020  op.inputs).     
+0000a350: 2020 2061 7373 6572 7420 696e 7075 7473     assert inputs
+0000a360: 0a20 2020 2020 2020 2077 6869 6c65 2069  .        while i
+0000a370: 6e70 7574 733a 0a20 2020 2020 2020 2020  nputs:.         
+0000a380: 2020 2078 203d 2069 6e70 7574 732e 706f     x = inputs.po
+0000a390: 7028 3029 0a20 2020 2020 2020 2020 2020  p(0).           
+0000a3a0: 2069 6620 6e6f 7420 782e 6973 5f64 796e   if not x.is_dyn
+0000a3b0: 616d 6963 2829 3a20 2023 2073 7461 7469  amic():  # stati
+0000a3c0: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
+0000a3d0: 2020 6173 7365 7274 2078 2e64 696d 656e    assert x.dimen
+0000a3e0: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
+0000a3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a400: 2069 6620 7920 6973 204e 6f6e 653a 0a20   if y is None:. 
+0000a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a420: 2020 2069 6620 6e6f 7420 7465 6d70 6c61     if not templa
+0000a430: 7465 5f6f 6e6c 7920 616e 6420 6261 636b  te_only and back
+0000a440: 656e 6420 616e 6420 6e6f 7420 7466 3a0a  end and not tf:.
+0000a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a460: 2020 2020 2020 2020 7920 3d20 6261 636b          y = back
+0000a470: 656e 642e 636f 6e76 6572 745f 746f 5f74  end.convert_to_t
+0000a480: 656e 736f 7228 782e 6469 6d65 6e73 696f  ensor(x.dimensio
+0000a490: 6e2c 2064 696d 733d 5b5d 2c20 6474 7970  n, dims=[], dtyp
+0000a4a0: 653d 7369 7a65 5f64 7479 7065 2c20 6e61  e=size_dtype, na
+0000a4b0: 6d65 3d79 5f6e 616d 6529 0a20 2020 2020  me=y_name).     
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000a4d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000a4e0: 2020 2020 2020 2020 2020 2020 2079 203d               y =
+0000a4f0: 205f 742e 5465 6e73 6f72 280a 2020 2020   _t.Tensor(.    
+0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a510: 2020 2020 2020 2020 6e61 6d65 3d79 5f6e          name=y_n
+0000a520: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a540: 2064 696d 5f74 6167 733d 5b5d 2c0a 2020   dim_tags=[],.  
+0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 2020 2020 2020 2020 2020 6474 7970 653d            dtype=
+0000a570: 7369 7a65 5f64 7479 7065 2c0a 2020 2020  size_dtype,.    
+0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a590: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000a5b0: 206e 6f74 2074 656d 706c 6174 655f 6f6e   not template_on
+0000a5c0: 6c79 2061 6e64 2074 663a 0a20 2020 2020  ly and tf:.     
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5e0: 2020 2020 2020 2077 6974 6820 7466 2e63         with tf.c
+0000a5f0: 6f6e 7472 6f6c 5f64 6570 656e 6465 6e63  ontrol_dependenc
+0000a600: 6965 7328 4e6f 6e65 293a 2020 2320 7468  ies(None):  # th
+0000a610: 6973 2077 696c 6c20 7265 7365 7420 7468  is will reset th
+0000a620: 6520 636f 6e74 6578 740a 2020 2020 2020  e context.      
+0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a640: 2020 2020 2020 2020 2020 792e 7261 775f            y.raw_
+0000a650: 7465 6e73 6f72 203d 2074 662e 636f 6e73  tensor = tf.cons
+0000a660: 7461 6e74 2878 2e64 696d 656e 7369 6f6e  tant(x.dimension
+0000a670: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a680: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000a6a0: 6620 7466 3a0a 2020 2020 2020 2020 2020  f tf:.          
+0000a6b0: 2020 2020 2020 2020 2020 792e 706c 6163            y.plac
+0000a6c0: 6568 6f6c 6465 7220 3d20 5f62 696e 5f6f  eholder = _bin_o
+0000a6d0: 705f 7466 2879 2e70 6c61 6365 686f 6c64  p_tf(y.placehold
+0000a6e0: 6572 2c20 782e 6469 6d65 6e73 696f 6e29  er, x.dimension)
+0000a6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a700: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000a710: 2020 2020 2020 2020 2020 2079 203d 205f             y = _
+0000a720: 6269 6e5f 6f70 2879 2c20 782e 6469 6d65  bin_op(y, x.dime
+0000a730: 6e73 696f 6e29 0a20 2020 2020 2020 2020  nsion).         
+0000a740: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+0000a750: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000a760: 656c 662e 6261 7463 683a 0a20 2020 2020  elf.batch:.     
+0000a770: 2020 2020 2020 2020 2020 2078 203d 2078             x = x
+0000a780: 2e67 6574 5f66 6f72 5f62 6174 6368 5f63  .get_for_batch_c
+0000a790: 7478 2873 656c 662e 6261 7463 682c 2073  tx(self.batch, s
+0000a7a0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
+0000a7b0: 5f63 7478 290a 2020 2020 2020 2020 2020  _ctx).          
+0000a7c0: 2020 782e 636f 6d70 6c65 7465 5f64 796e    x.complete_dyn
+0000a7d0: 5f73 697a 6528 7465 6d70 6c61 7465 5f6f  _size(template_o
+0000a7e0: 6e6c 793d 7465 6d70 6c61 7465 5f6f 6e6c  nly=template_onl
+0000a7f0: 7929 0a20 2020 2020 2020 2020 2020 2069  y).            i
+0000a800: 6620 6e6f 7420 782e 6479 6e5f 7369 7a65  f not x.dyn_size
+0000a810: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
+0000a820: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000a830: 2020 2020 2020 2020 2078 203d 2078 2e64           x = x.d
+0000a840: 796e 5f73 697a 655f 6578 740a 2020 2020  yn_size_ext.    
+0000a850: 2020 2020 2020 2020 6966 2079 2069 7320          if y is 
+0000a860: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000a870: 2020 2020 2020 7920 3d20 782e 636f 7079        y = x.copy
+0000a880: 286e 616d 653d 795f 6e61 6d65 290a 2020  (name=y_name).  
+0000a890: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000a8a0: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+0000a8b0: 2020 2069 6620 782e 6469 6d5f 7461 6773     if x.dim_tags
+0000a8c0: 2021 3d20 792e 6469 6d5f 7461 6773 3a0a   != y.dim_tags:.
+0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8e0: 636f 6d6d 6f6e 203d 205f 742e 5465 6e73  common = _t.Tens
+0000a8f0: 6f72 2e67 6574 5f63 6f6d 6d6f 6e5f 6461  or.get_common_da
+0000a900: 7461 285b 782c 2079 5d2c 2061 6c6c 6f77  ta([x, y], allow
+0000a910: 5f62 726f 6164 6361 7374 5f61 6c6c 5f73  _broadcast_all_s
+0000a920: 6f75 7263 6573 3d54 7275 6529 0a20 2020  ources=True).   
+0000a930: 2020 2020 2020 2020 2020 2020 2078 5f20               x_ 
+0000a940: 3d20 782e 636f 7079 5f63 6f6d 7061 7469  = x.copy_compati
+0000a950: 626c 655f 746f 2863 6f6d 6d6f 6e29 2069  ble_to(common) i
+0000a960: 6620 782e 6469 6d5f 7461 6773 2065 6c73  f x.dim_tags els
+0000a970: 6520 780a 2020 2020 2020 2020 2020 2020  e x.            
+0000a980: 2020 2020 795f 203d 2079 2e63 6f70 795f      y_ = y.copy_
+0000a990: 636f 6d70 6174 6962 6c65 5f74 6f28 636f  compatible_to(co
+0000a9a0: 6d6d 6f6e 2920 6966 2079 2e64 696d 5f74  mmon) if y.dim_t
+0000a9b0: 6167 7320 656c 7365 2079 0a20 2020 2020  ags else y.     
+0000a9c0: 2020 2020 2020 2020 2020 2079 203d 2063             y = c
+0000a9d0: 6f6d 6d6f 6e0a 2020 2020 2020 2020 2020  ommon.          
+0000a9e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000a9f0: 2020 2020 2020 2020 785f 2c20 795f 203d          x_, y_ =
+0000aa00: 2078 2c20 790a 2020 2020 2020 2020 2020   x, y.          
+0000aa10: 2020 6966 2074 663a 0a20 2020 2020 2020    if tf:.       
+0000aa20: 2020 2020 2020 2020 2079 2e70 6c61 6365           y.place
+0000aa30: 686f 6c64 6572 203d 205f 6269 6e5f 6f70  holder = _bin_op
+0000aa40: 5f74 6628 795f 2e70 6c61 6365 686f 6c64  _tf(y_.placehold
+0000aa50: 6572 2c20 785f 2e70 6c61 6365 686f 6c64  er, x_.placehold
+0000aa60: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
+0000aa70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000aa80: 2020 2020 2020 7920 3d20 5f62 696e 5f6f        y = _bin_o
+0000aa90: 7028 795f 2c20 785f 290a 2020 2020 2020  p(y_, x_).      
+0000aaa0: 2020 6173 7365 7274 2079 2c20 6622 6f70    assert y, f"op
+0000aab0: 207b 6f70 7d3f 220a 2020 2020 2020 2020   {op}?".        
+0000aac0: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
+0000aad0: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
+0000aae0: 2020 6173 7365 7274 2073 656c 662e 6479    assert self.dy
+0000aaf0: 6e5f 7369 7a65 5f65 7874 2e64 696d 5f74  n_size_ext.dim_t
+0000ab00: 6167 7320 3d3d 2079 2e64 696d 5f74 6167  ags == y.dim_tag
+0000ab10: 730a 2020 2020 2020 2020 6966 2079 2e62  s.        if y.b
+0000ab20: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
+0000ab30: 2020 6966 2073 656c 662e 6261 7463 683a    if self.batch:
+0000ab40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ab50: 2061 7373 6572 7420 7365 6c66 2e62 6174   assert self.bat
+0000ab60: 6368 203d 3d20 792e 6261 7463 680a 2020  ch == y.batch.  
+0000ab70: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab90: 7365 6c66 2e62 6174 6368 203d 2079 2e62  self.batch = y.b
+0000aba0: 6174 6368 0a20 2020 2020 2020 2073 656c  atch.        sel
+0000abb0: 662e 6479 6e5f 7369 7a65 5f65 7874 203d  f.dyn_size_ext =
+0000abc0: 2079 0a20 2020 2020 2020 2069 6620 7466   y.        if tf
+0000abd0: 2061 6e64 2079 2e70 6c61 6365 686f 6c64   and y.placehold
+0000abe0: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+0000abf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ac00: 2e73 6574 5f74 6167 5f6f 6e5f 7369 7a65  .set_tag_on_size
+0000ac10: 5f74 656e 736f 7228 792e 706c 6163 6568  _tensor(y.placeh
+0000ac20: 6f6c 6465 7229 0a0a 2020 2020 6465 6620  older)..    def 
+0000ac30: 6973 5f65 7175 616c 280a 2020 2020 2020  is_equal(.      
+0000ac40: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000ac50: 6f74 6865 722c 0a20 2020 2020 2020 2069  other,.        i
+0000ac60: 676e 6f72 655f 6665 6174 7572 655f 6469  gnore_feature_di
+0000ac70: 6d3d 4661 6c73 652c 0a20 2020 2020 2020  m=False,.       
+0000ac80: 2061 6c6c 6f77 5f73 616d 655f 6665 6174   allow_same_feat
+0000ac90: 7572 655f 6469 6d3d 4661 6c73 652c 0a20  ure_dim=False,. 
+0000aca0: 2020 2020 2020 2061 6c6c 6f77 5f73 616d         allow_sam
+0000acb0: 655f 7370 6174 6961 6c5f 6469 6d3d 4e6f  e_spatial_dim=No
+0000acc0: 6e65 2c0a 2020 2020 2020 2020 7472 6561  ne,.        trea
+0000acd0: 745f 6665 6174 7572 655f 6173 5f73 7061  t_feature_as_spa
+0000ace0: 7469 616c 3d46 616c 7365 2c0a 2020 2020  tial=False,.    
+0000acf0: 2020 2020 6272 6f61 6463 6173 745f 6d61      broadcast_ma
+0000ad00: 7463 6865 733d 4661 6c73 652c 0a20 2020  tches=False,.   
+0000ad10: 2020 2020 2075 6e6b 6e6f 776e 5f73 7061       unknown_spa
+0000ad20: 7469 616c 5f6d 6174 6368 6573 3d46 616c  tial_matches=Fal
+0000ad30: 7365 2c0a 2020 2020 2020 2020 756e 6465  se,.        unde
+0000ad40: 6669 6e65 645f 6d61 7463 6865 733d 4661  fined_matches=Fa
+0000ad50: 6c73 652c 0a20 2020 2020 2020 2064 6572  lse,.        der
+0000ad60: 6976 6564 5f6d 6174 6368 6573 3d46 616c  ived_matches=Fal
+0000ad70: 7365 2c0a 2020 2020 293a 0a20 2020 2020  se,.    ):.     
+0000ad80: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+0000ad90: 6f6d 7061 7265 7320 7365 6c66 2074 6f20  ompares self to 
+0000ada0: 6f74 6865 7220 666f 7220 6571 7561 6c69  other for equali
+0000adb0: 7479 2e0a 0a20 2020 2020 2020 204e 6f74  ty...        Not
+0000adc0: 6520 7468 6174 2074 6865 2064 6566 6175  e that the defau
+0000add0: 6c74 2062 6568 6176 696f 7220 6973 2076  lt behavior is v
+0000ade0: 6572 7920 7265 7374 7269 6374 6976 652e  ery restrictive.
+0000adf0: 0a20 2020 2020 2020 2055 7365 2066 756e  .        Use fun
+0000ae00: 6374 696f 6e73 2073 7563 6820 6173 203a  ctions such as :
+0000ae10: 6675 6e63 3a60 6765 745f 616c 6c5f 6469  func:`get_all_di
+0000ae20: 6d65 6e73 696f 6e5f 7461 6773 6020 6f72  mension_tags` or
+0000ae30: 203a 6675 6e63 3a60 6765 745f 6578 6973   :func:`get_exis
+0000ae40: 7469 6e67 5f74 6167 5f66 726f 6d5f 636f  ting_tag_from_co
+0000ae50: 6c6c 6563 7469 6f6e 600a 2020 2020 2020  llection`.      
+0000ae60: 2020 746f 2065 7870 6c69 6369 746c 7920    to explicitly 
+0000ae70: 7370 6563 6966 7920 7468 6520 6265 6861  specify the beha
+0000ae80: 7669 6f72 2066 6f72 2074 6865 2063 6f6d  vior for the com
+0000ae90: 7061 7269 736f 6e2e 0a0a 2020 2020 2020  parison...      
+0000aea0: 2020 416c 736f 206e 6f74 6520 7468 6174    Also note that
+0000aeb0: 2074 6865 2064 6566 696e 6974 696f 6e20   the definition 
+0000aec0: 6973 2073 6c69 6768 746c 7920 6164 2d68  is slightly ad-h
+0000aed0: 6f63 2066 6f72 2073 6f6d 6520 6361 7365  oc for some case
+0000aee0: 732c 0a20 2020 2020 2020 2061 6e64 206d  s,.        and m
+0000aef0: 6967 6874 2070 6f74 656e 7469 616c 6c79  ight potentially
+0000af00: 2063 6861 6e67 6520 696e 2074 6865 2066   change in the f
+0000af10: 7574 7572 652e 0a20 2020 2020 2020 2020  uture..         
+0000af20: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+0000af30: 636f 6d2f 7277 7468 2d69 362f 7265 7475  com/rwth-i6/retu
+0000af40: 726e 6e2f 6973 7375 6573 2f36 3334 0a0a  rnn/issues/634..
+0000af50: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
+0000af60: 696d 206f 7468 6572 3a0a 2020 2020 2020  im other:.      
+0000af70: 2020 3a70 6172 616d 2062 6f6f 6c20 6967    :param bool ig
+0000af80: 6e6f 7265 5f66 6561 7475 7265 5f64 696d  nore_feature_dim
+0000af90: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+0000afa0: 2062 6f6f 6c20 616c 6c6f 775f 7361 6d65   bool allow_same
+0000afb0: 5f66 6561 7475 7265 5f64 696d 3a0a 2020  _feature_dim:.  
+0000afc0: 2020 2020 2020 3a70 6172 616d 2062 6f6f        :param boo
+0000afd0: 6c7c 4e6f 6e65 2061 6c6c 6f77 5f73 616d  l|None allow_sam
+0000afe0: 655f 7370 6174 6961 6c5f 6469 6d3a 0a20  e_spatial_dim:. 
+0000aff0: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
+0000b000: 6f6c 2074 7265 6174 5f66 6561 7475 7265  ol treat_feature
+0000b010: 5f61 735f 7370 6174 6961 6c3a 0a20 2020  _as_spatial:.   
+0000b020: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
+0000b030: 2062 726f 6164 6361 7374 5f6d 6174 6368   broadcast_match
+0000b040: 6573 3a0a 2020 2020 2020 2020 3a70 6172  es:.        :par
+0000b050: 616d 2062 6f6f 6c20 756e 6b6e 6f77 6e5f  am bool unknown_
+0000b060: 7370 6174 6961 6c5f 6d61 7463 6865 733a  spatial_matches:
+0000b070: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000b080: 626f 6f6c 2075 6e64 6566 696e 6564 5f6d  bool undefined_m
+0000b090: 6174 6368 6573 3a0a 2020 2020 2020 2020  atches:.        
+0000b0a0: 3a70 6172 616d 2062 6f6f 6c20 6465 7269  :param bool deri
+0000b0b0: 7665 645f 6d61 7463 6865 733a 0a20 2020  ved_matches:.   
+0000b0c0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+0000b0d0: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
+0000b0e0: 2020 2020 2020 6672 6f6d 2072 6574 7572        from retur
+0000b0f0: 6e6e 2e75 7469 6c20 696d 706f 7274 2042  nn.util import B
+0000b100: 6568 6176 696f 7256 6572 7369 6f6e 0a0a  ehaviorVersion..
+0000b110: 2020 2020 2020 2020 6966 2073 656c 6620          if self 
+0000b120: 6973 206f 7468 6572 3a20 2023 2066 6972  is other:  # fir
+0000b130: 7374 2073 6f6d 6520 6661 7374 2070 6174  st some fast pat
+0000b140: 6820 6368 6563 6b0a 2020 2020 2020 2020  h check.        
+0000b150: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000b160: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000b170: 7370 6563 6961 6c20 6f72 206f 7468 6572  special or other
+0000b180: 2e73 7065 6369 616c 3a0a 2020 2020 2020  .special:.      
+0000b190: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0000b1a0: 7365 2020 2320 6f6e 6c79 2074 7275 6520  se  # only true 
+0000b1b0: 6966 2073 616d 6520 696e 7374 616e 6365  if same instance
+0000b1c0: 2c20 6368 6563 6b20 6162 6f76 650a 2020  , check above.  
+0000b1d0: 2020 2020 2020 6966 2061 6c6c 6f77 5f73        if allow_s
+0000b1e0: 616d 655f 7370 6174 6961 6c5f 6469 6d20  ame_spatial_dim 
+0000b1f0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000b200: 2020 2020 2061 6c6c 6f77 5f73 616d 655f       allow_same_
+0000b210: 7370 6174 6961 6c5f 6469 6d20 3d20 616c  spatial_dim = al
+0000b220: 6c6f 775f 7361 6d65 5f66 6561 7475 7265  low_same_feature
+0000b230: 5f64 696d 0a20 2020 2020 2020 2073 656c  _dim.        sel
+0000b240: 665f 6261 7365 203d 2073 656c 662e 6765  f_base = self.ge
+0000b250: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
+0000b260: 6173 6528 2920 6966 2064 6572 6976 6564  ase() if derived
+0000b270: 5f6d 6174 6368 6573 2065 6c73 6520 7365  _matches else se
+0000b280: 6c66 2e67 6574 5f73 616d 655f 6261 7365  lf.get_same_base
+0000b290: 2829 0a20 2020 2020 2020 206f 7468 6572  ().        other
+0000b2a0: 5f62 6173 6520 3d20 6f74 6865 722e 6765  _base = other.ge
+0000b2b0: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
+0000b2c0: 6173 6528 2920 6966 2064 6572 6976 6564  ase() if derived
+0000b2d0: 5f6d 6174 6368 6573 2065 6c73 6520 6f74  _matches else ot
+0000b2e0: 6865 722e 6765 745f 7361 6d65 5f62 6173  her.get_same_bas
+0000b2f0: 6528 290a 2020 2020 2020 2020 6966 2073  e().        if s
+0000b300: 656c 665f 6261 7365 2069 7320 6f74 6865  elf_base is othe
+0000b310: 725f 6261 7365 3a0a 2020 2020 2020 2020  r_base:.        
+0000b320: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000b330: 2020 2020 2020 2020 6966 2073 656c 665f          if self_
+0000b340: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000b350: 6d5f 6f70 2061 6e64 206f 7468 6572 5f62  m_op and other_b
+0000b360: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
+0000b370: 5f6f 703a 0a20 2020 2020 2020 2020 2020  _op:.           
+0000b380: 2069 6620 7365 6c66 5f62 6173 652e 6465   if self_base.de
+0000b390: 7269 7665 645f 6672 6f6d 5f6f 7020 3d3d  rived_from_op ==
+0000b3a0: 206f 7468 6572 5f62 6173 652e 6465 7269   other_base.deri
+0000b3b0: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
+0000b3c0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000b3d0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+0000b3e0: 2073 656c 665f 6b69 6e64 203d 2073 656c   self_kind = sel
+0000b3f0: 662e 6b69 6e64 0a20 2020 2020 2020 206f  f.kind.        o
+0000b400: 7468 6572 5f6b 696e 6420 3d20 6f74 6865  ther_kind = othe
+0000b410: 722e 6b69 6e64 0a20 2020 2020 2020 2069  r.kind.        i
+0000b420: 6620 7365 6c66 5f6b 696e 6420 3d3d 206f  f self_kind == o
+0000b430: 7468 6572 5f6b 696e 6420 3d3d 2044 696d  ther_kind == Dim
+0000b440: 5479 7065 732e 4665 6174 7572 6520 616e  Types.Feature an
+0000b450: 6420 6967 6e6f 7265 5f66 6561 7475 7265  d ignore_feature
+0000b460: 5f64 696d 3a0a 2020 2020 2020 2020 2020  _dim:.          
+0000b470: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000b480: 2020 2020 2020 6966 2074 7265 6174 5f66        if treat_f
+0000b490: 6561 7475 7265 5f61 735f 7370 6174 6961  eature_as_spatia
+0000b4a0: 6c3a 0a20 2020 2020 2020 2020 2020 2023  l:.            #
+0000b4b0: 204e 6f74 653a 204e 6f20 6b69 6e64 2061   Note: No kind a
+0000b4c0: 7420 616c 6c3a 2052 6569 6e74 6572 7072  t all: Reinterpr
+0000b4d0: 6574 2074 7265 6174 5f66 6561 7475 7265  et treat_feature
+0000b4e0: 5f61 735f 7370 6174 6961 6c20 6120 6269  _as_spatial a bi
+0000b4f0: 743a 0a20 2020 2020 2020 2020 2020 2023  t:.            #
+0000b500: 2041 7373 756d 6520 7468 6174 2077 6520   Assume that we 
+0000b510: 7761 6e74 2074 6865 6d20 616c 6c20 746f  want them all to
+0000b520: 2062 6520 6861 6e64 6c65 6420 7468 6520   be handled the 
+0000b530: 7361 6d65 2c20 6e6f 206d 6174 7465 7220  same, no matter 
+0000b540: 7468 6520 6b69 6e64 2e0a 2020 2020 2020  the kind..      
+0000b550: 2020 2020 2020 2320 2845 7863 6570 7420        # (Except 
+0000b560: 6f66 2062 6174 6368 2064 696d 206b 696e  of batch dim kin
+0000b570: 642c 2077 6869 6368 2069 7320 7374 696c  d, which is stil
+0000b580: 6c20 6578 636c 7564 6564 2068 6572 652e  l excluded here.
+0000b590: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000b5a0: 2073 656c 665f 6b69 6e64 203d 3d20 4469   self_kind == Di
+0000b5b0: 6d54 7970 6573 2e46 6561 7475 7265 206f  mTypes.Feature o
+0000b5c0: 7220 6e6f 7420 7365 6c66 5f6b 696e 643a  r not self_kind:
+0000b5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b5e0: 2073 656c 665f 6b69 6e64 203d 2044 696d   self_kind = Dim
+0000b5f0: 5479 7065 732e 5370 6174 6961 6c0a 2020  Types.Spatial.  
+0000b600: 2020 2020 2020 2020 2020 6966 206f 7468            if oth
+0000b610: 6572 5f6b 696e 6420 3d3d 2044 696d 5479  er_kind == DimTy
+0000b620: 7065 732e 4665 6174 7572 6520 6f72 206e  pes.Feature or n
+0000b630: 6f74 206f 7468 6572 5f6b 696e 643a 0a20  ot other_kind:. 
+0000b640: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000b650: 7468 6572 5f6b 696e 6420 3d20 4469 6d54  ther_kind = DimT
+0000b660: 7970 6573 2e53 7061 7469 616c 0a20 2020  ypes.Spatial.   
+0000b670: 2020 2020 2069 6620 7365 6c66 2e64 696d       if self.dim
+0000b680: 656e 7369 6f6e 2021 3d20 6f74 6865 722e  ension != other.
+0000b690: 6469 6d65 6e73 696f 6e3a 0a20 2020 2020  dimension:.     
+0000b6a0: 2020 2020 2020 2069 6620 6272 6f61 6463         if broadc
+0000b6b0: 6173 745f 6d61 7463 6865 7320 616e 6420  ast_matches and 
+0000b6c0: 2873 656c 662e 6469 6d65 6e73 696f 6e20  (self.dimension 
+0000b6d0: 3d3d 2031 206f 7220 6f74 6865 722e 6469  == 1 or other.di
+0000b6e0: 6d65 6e73 696f 6e20 3d3d 2031 293a 0a20  mension == 1):. 
+0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000b700: 6173 7320 2023 2070 6173 7320 6f6e 0a20  ass  # pass on. 
+0000b710: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000b720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b730: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0000b740: 2020 2020 2020 6966 2073 656c 665f 6b69        if self_ki
+0000b750: 6e64 2021 3d20 6f74 6865 725f 6b69 6e64  nd != other_kind
+0000b760: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000b770: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+0000b780: 2020 2069 6620 7365 6c66 5f6b 696e 6420     if self_kind 
+0000b790: 3d3d 206f 7468 6572 5f6b 696e 6420 3d3d  == other_kind ==
+0000b7a0: 2044 696d 5479 7065 732e 4261 7463 683a   DimTypes.Batch:
+0000b7b0: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
+0000b7c0: 6f74 653a 2054 6869 7320 6d69 6768 7420  ote: This might 
+0000b7d0: 6265 2069 6e63 6f72 7265 6374 2069 6e20  be incorrect in 
+0000b7e0: 736f 6d65 2063 6173 6573 2c0a 2020 2020  some cases,.    
+0000b7f0: 2020 2020 2020 2020 2320 652e 672e 2066          # e.g. f
+0000b800: 6f72 2062 6561 6d20 7365 6172 6368 2077  or beam search w
+0000b810: 6865 6e20 7765 2068 6176 6520 7468 6520  hen we have the 
+0000b820: 6265 616d 2068 6964 6465 6e20 696e 2074  beam hidden in t
+0000b830: 6865 2062 6174 6368 2064 696d 2c0a 2020  he batch dim,.  
+0000b840: 2020 2020 2020 2020 2020 2320 6f72 2077            # or w
+0000b850: 6865 6e20 7765 2075 7365 6420 4d65 7267  hen we used Merg
+0000b860: 6544 696d 734c 6179 6572 206f 6e20 7468  eDimsLayer on th
+0000b870: 6520 6261 7463 6820 6178 6973 2c20 6f72  e batch axis, or
+0000b880: 2073 6f2e 0a20 2020 2020 2020 2020 2020   so..           
+0000b890: 2023 2057 6520 6d69 6768 7420 6e65 6564   # We might need
+0000b8a0: 2074 6f20 6578 7465 6e64 2074 6865 206c   to extend the l
+0000b8b0: 6f67 6963 2068 6572 6520 6c61 7465 722e  ogic here later.
+0000b8c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000b8d0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+0000b8e0: 2069 6620 4265 6861 7669 6f72 5665 7273   if BehaviorVers
+0000b8f0: 696f 6e2e 6765 7428 2920 3e3d 2031 363a  ion.get() >= 16:
+0000b900: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
+0000b910: 6974 6865 7220 7365 6c66 206f 7220 6f74  ither self or ot
+0000b920: 6865 7220 6973 2073 6f6d 6520 6469 6d20  her is some dim 
+0000b930: 7461 6720 6578 706c 6963 6974 6c79 2063  tag explicitly c
+0000b940: 7265 6174 6564 2062 7920 7468 6520 7573  reated by the us
+0000b950: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0000b960: 2320 616e 6420 7468 6579 2061 7265 206e  # and they are n
+0000b970: 6f74 2074 6865 2073 616d 652c 2073 6f20  ot the same, so 
+0000b980: 7765 206e 6576 6572 2074 7265 6174 2074  we never treat t
+0000b990: 6865 6d20 6173 2065 7175 616c 2e0a 2020  hem as equal..  
+0000b9a0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000b9b0: 2073 656c 662e 6175 746f 5f67 656e 6572   self.auto_gener
+0000b9c0: 6174 6564 206f 7220 6e6f 7420 6f74 6865  ated or not othe
+0000b9d0: 722e 6175 746f 5f67 656e 6572 6174 6564  r.auto_generated
+0000b9e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b9f0: 2020 6966 2062 726f 6164 6361 7374 5f6d    if broadcast_m
+0000ba00: 6174 6368 6573 2061 6e64 2028 0a20 2020  atches and (.   
 0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba20: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000ba30: 2020 2020 2020 2070 6173 7320 2023 2065         pass  # e
-0000ba40: 7863 6570 7469 6f6e 2c20 616c 6c6f 7720  xception, allow 
-0000ba50: 6272 6f61 6463 6173 7420 6c6f 6769 630a  broadcast logic.
-0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000ba80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000ba90: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
-0000baa0: 6620 7365 6c66 5f6b 696e 6420 3d3d 206f  f self_kind == o
-0000bab0: 7468 6572 5f6b 696e 6420 3d3d 2044 696d  ther_kind == Dim
-0000bac0: 5479 7065 732e 4665 6174 7572 653a 0a20  Types.Feature:. 
-0000bad0: 2020 2020 2020 2020 2020 2069 6620 616c             if al
-0000bae0: 6c6f 775f 7361 6d65 5f66 6561 7475 7265  low_same_feature
-0000baf0: 5f64 696d 3a0a 2020 2020 2020 2020 2020  _dim:.          
-0000bb00: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0000bb10: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0000bb20: 665f 6b69 6e64 203d 3d20 6f74 6865 725f  f_kind == other_
-0000bb30: 6b69 6e64 203d 3d20 4469 6d54 7970 6573  kind == DimTypes
-0000bb40: 2e53 7061 7469 616c 3a0a 2020 2020 2020  .Spatial:.      
-0000bb50: 2020 2020 2020 6966 2061 6c6c 6f77 5f73        if allow_s
-0000bb60: 616d 655f 7370 6174 6961 6c5f 6469 6d3a  ame_spatial_dim:
-0000bb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bb80: 2069 6620 7365 6c66 2e64 696d 656e 7369   if self.dimensi
-0000bb90: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbb0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbd0: 6966 2062 726f 6164 6361 7374 5f6d 6174  if broadcast_mat
-0000bbe0: 6368 6573 2061 6e64 2028 7365 6c66 2e64  ches and (self.d
-0000bbf0: 696d 656e 7369 6f6e 203d 3d20 3120 6f72  imension == 1 or
-0000bc00: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
-0000bc10: 203d 3d20 3129 3a0a 2020 2020 2020 2020   == 1):.        
-0000bc20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000bc30: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-0000bc40: 2020 2020 6966 2075 6e6b 6e6f 776e 5f73      if unknown_s
-0000bc50: 7061 7469 616c 5f6d 6174 6368 6573 2061  patial_matches a
-0000bc60: 6e64 2028 2873 656c 662e 6479 6e5f 7369  nd ((self.dyn_si
-0000bc70: 7a65 2069 7320 4e6f 6e65 2920 6f72 2028  ze is None) or (
-0000bc80: 6f74 6865 722e 6479 6e5f 7369 7a65 2069  other.dyn_size i
-0000bc90: 7320 4e6f 6e65 2929 3a0a 2020 2020 2020  s None)):.      
-0000bca0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000bcb0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000bcc0: 2020 6966 2075 6e64 6566 696e 6564 5f6d    if undefined_m
-0000bcd0: 6174 6368 6573 2061 6e64 2028 7365 6c66  atches and (self
-0000bce0: 2e75 6e64 6566 696e 6564 206f 7220 6f74  .undefined or ot
-0000bcf0: 6865 722e 756e 6465 6669 6e65 6429 3a0a  her.undefined):.
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000bd20: 2020 2020 2320 496e 2070 7269 6e63 6970      # In princip
-0000bd30: 6c65 2c20 7765 2077 6f75 6c64 2077 616e  le, we would wan
-0000bd40: 7420 746f 2063 6865 636b 2066 6f72 2069  t to check for i
-0000bd50: 6465 6e74 6974 7920 2873 656c 6620 6973  dentity (self is
-0000bd60: 206f 7468 6572 292e 0a20 2020 2020 2020   other)..       
-0000bd70: 2023 2057 6520 6375 7272 656e 746c 7920   # We currently 
-0000bd80: 7573 6520 7468 6520 6465 7363 7269 7074  use the descript
-0000bd90: 696f 6e20 6265 6361 7573 6520 7468 6520  ion because the 
-0000bda0: 6964 656e 7469 7479 2077 6f75 6c64 206e  identity would n
-0000bdb0: 6f74 2062 6520 7468 6520 7361 6d65 0a20  ot be the same. 
-0000bdc0: 2020 2020 2020 2023 2069 6e20 6361 7365         # in case
-0000bdd0: 206f 6620 7465 6d70 6c61 7465 2063 6f6e   of template con
-0000bde0: 7374 7275 6374 696f 6e20 7768 6572 6520  struction where 
-0000bdf0: 6120 6469 6d20 7461 6720 6973 206f 6e63  a dim tag is onc
-0000be00: 6520 6372 6561 7465 6420 666f 7220 6120  e created for a 
-0000be10: 7465 6d70 6c61 7465 206c 6179 6572 2c0a  template layer,.
-0000be20: 2020 2020 2020 2020 2320 616e 6420 7468          # and th
-0000be30: 656e 206c 6174 6572 2061 6761 696e 2066  en later again f
-0000be40: 6f72 2074 6865 2072 6561 6c20 6c61 7965  or the real laye
-0000be50: 722e 0a20 2020 2020 2020 2069 6620 7365  r..        if se
-0000be60: 6c66 2e61 7574 6f5f 6765 6e65 7261 7465  lf.auto_generate
-0000be70: 6420 616e 6420 6f74 6865 722e 6175 746f  d and other.auto
-0000be80: 5f67 656e 6572 6174 6564 2061 6e64 2073  _generated and s
-0000be90: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
-0000bea0: 3d3d 206f 7468 6572 2e64 6573 6372 6970  == other.descrip
-0000beb0: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-0000bec0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0000bed0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000bee0: 7365 0a0a 2020 2020 6465 6620 5f5f 6571  se..    def __eq
-0000bef0: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
-0000bf00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000bf10: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
-0000bf20: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-0000bf30: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-0000bf40: 2020 2020 3a72 6574 7572 6e3a 203a 6675      :return: :fu
-0000bf50: 6e63 3a60 6973 5f65 7175 616c 6020 7769  nc:`is_equal` wi
-0000bf60: 7468 2064 6566 6175 6c74 206f 7074 696f  th default optio
-0000bf70: 6e73 0a20 2020 2020 2020 2022 2222 0a20  ns.        """. 
-0000bf80: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-0000bf90: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
-0000bfa0: 5f64 2e44 696d 293a 0a20 2020 2020 2020  _d.Dim):.       
-0000bfb0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-0000bfc0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0000bfd0: 2073 656c 662e 6973 5f65 7175 616c 286f   self.is_equal(o
-0000bfe0: 7468 6572 290a 0a20 2020 2064 6566 205f  ther)..    def _
-0000bff0: 5f6e 655f 5f28 7365 6c66 3a20 4469 6d2c  _ne__(self: Dim,
-0000c000: 206f 7468 6572 3a20 4469 6d29 3a0a 2020   other: Dim):.  
-0000c010: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000c020: 2020 3a70 6172 616d 2044 696d 206f 7468    :param Dim oth
-0000c030: 6572 3a0a 2020 2020 2020 2020 3a72 7479  er:.        :rty
-0000c040: 7065 3a20 626f 6f6c 0a20 2020 2020 2020  pe: bool.       
-0000c050: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-0000c060: 7572 6e20 6e6f 7420 2873 656c 6620 3d3d  urn not (self ==
-0000c070: 206f 7468 6572 290a 0a20 2020 2064 6566   other)..    def
-0000c080: 205f 5f68 6173 685f 5f28 7365 6c66 293a   __hash__(self):
-0000c090: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c0a0: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
-0000c0b0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0000c0c0: 3a20 6861 7368 2c20 6d61 7463 6869 6e67  : hash, matching
-0000c0d0: 2074 6f20 3a66 756e 633a 605f 5f65 715f   to :func:`__eq_
-0000c0e0: 5f60 0a20 2020 2020 2020 2022 2222 0a20  _`.        """. 
-0000c0f0: 2020 2020 2020 2023 2054 6869 7320 6d75         # This mu
-0000c100: 7374 206d 6174 6368 2074 6865 2062 6568  st match the beh
-0000c110: 6176 696f 7220 696e 205f 5f65 715f 5f2c  avior in __eq__,
-0000c120: 2077 6869 6368 2069 7320 6973 5f65 7175   which is is_equ
-0000c130: 616c 2077 6974 6820 6465 6661 756c 7420  al with default 
-0000c140: 6f70 7469 6f6e 732e 0a20 2020 2020 2020  options..       
-0000c150: 2023 2049 2e65 2e20 6469 6666 6572 656e   # I.e. differen
-0000c160: 7420 6861 7368 2069 6d70 6c69 6573 206e  t hash implies n
-0000c170: 6f74 2065 7175 616c 2028 6275 7420 7361  ot equal (but sa
-0000c180: 6d65 2068 6173 6820 6e6f 7420 6e65 6365  me hash not nece
-0000c190: 7373 6172 696c 7920 6571 7561 6c29 2e0a  ssarily equal)..
-0000c1a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c1b0: 7370 6563 6961 6c3a 0a20 2020 2020 2020  special:.       
-0000c1c0: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
-0000c1d0: 2869 6428 7365 6c66 2929 0a20 2020 2020  (id(self)).     
-0000c1e0: 2020 2069 6620 7365 6c66 2e69 735f 6261     if self.is_ba
-0000c1f0: 7463 685f 6469 6d28 293a 0a20 2020 2020  tch_dim():.     
-0000c200: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
-0000c210: 7368 2828 2929 0a20 2020 2020 2020 2077  sh(()).        w
-0000c220: 6974 6820 7574 696c 2e67 7561 7264 5f69  ith util.guard_i
-0000c230: 6e66 696e 6974 655f 7265 6375 7273 696f  nfinite_recursio
-0000c240: 6e28 5f64 2e44 696d 2e5f 5f68 6173 685f  n(_d.Dim.__hash_
-0000c250: 5f2c 2073 656c 6629 3a0a 2020 2020 2020  _, self):.      
-0000c260: 2020 2020 2020 6261 7365 203d 2073 656c        base = sel
-0000c270: 662e 6765 745f 7361 6d65 5f62 6173 6528  f.get_same_base(
-0000c280: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000c290: 2062 6173 6520 6973 206e 6f74 2073 656c   base is not sel
-0000c2a0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-0000c2b0: 2020 2072 6574 7572 6e20 6861 7368 2862     return hash(b
-0000c2c0: 6173 6529 0a20 2020 2020 2020 2020 2020  ase).           
-0000c2d0: 2069 6620 7365 6c66 2e64 6572 6976 6564   if self.derived
-0000c2e0: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
-0000c2f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c300: 2068 6173 6828 7365 6c66 2e64 6572 6976   hash(self.deriv
-0000c310: 6564 5f66 726f 6d5f 6f70 290a 2020 2020  ed_from_op).    
-0000c320: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c330: 6175 746f 5f67 656e 6572 6174 6564 3a0a  auto_generated:.
-0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c350: 7265 7475 726e 2068 6173 6828 2862 6173  return hash((bas
-0000c360: 652e 6b69 6e64 2c20 6261 7365 2e64 696d  e.kind, base.dim
-0000c370: 656e 7369 6f6e 2c20 6261 7365 2e64 6573  ension, base.des
-0000c380: 6372 6970 7469 6f6e 2929 0a20 2020 2020  cription)).     
-0000c390: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
-0000c3a0: 7368 2869 6428 6261 7365 2929 0a0a 2020  sh(id(base))..  
-0000c3b0: 2020 6465 6620 5f5f 6c74 5f5f 2873 656c    def __lt__(sel
-0000c3c0: 663a 2044 696d 2c20 6f74 6865 723a 2044  f: Dim, other: D
-0000c3d0: 696d 293a 0a20 2020 2020 2020 2022 2222  im):.        """
-0000c3e0: 0a20 2020 2020 2020 2044 6566 696e 6520  .        Define 
-0000c3f0: 736f 6d65 206f 7264 6572 2e20 5468 6973  some order. This
-0000c400: 2069 7320 6a75 7374 2073 7563 6820 7468   is just such th
-0000c410: 6174 2060 736f 7274 6564 6020 776f 726b  at `sorted` work
-0000c420: 732c 206f 7220 736f 6d65 2064 6966 6620  s, or some diff 
-0000c430: 7265 706f 7274 696e 672c 206f 7220 736f  reporting, or so
-0000c440: 2e0a 2020 2020 2020 2020 4974 2069 7320  ..        It is 
-0000c450: 6f6e 2073 796d 626f 6c69 6320 6c65 7665  on symbolic leve
-0000c460: 6c2c 2069 2e65 2e20 6974 2064 6f65 7320  l, i.e. it does 
-0000c470: 6e6f 7420 636f 6e73 6964 6572 2074 6865  not consider the
-0000c480: 2061 6374 7561 6c20 6469 6d65 6e73 696f   actual dimensio
-0000c490: 6e20 7661 6c75 652e 0a20 2020 2020 2020  n value..       
-0000c4a0: 2054 6865 2064 6566 696e 6564 206f 7264   The defined ord
-0000c4b0: 6572 2073 6f6d 6577 6861 7420 6172 6269  er somewhat arbi
-0000c4c0: 7472 6172 792c 2073 6f20 646f 206e 6f74  trary, so do not
-0000c4d0: 2072 656c 7920 6f6e 2074 6865 2065 7861   rely on the exa
-0000c4e0: 6374 2062 6568 6176 696f 722c 0a20 2020  ct behavior,.   
-0000c4f0: 2020 2020 2061 7320 7468 6973 206d 6967       as this mig
-0000c500: 6874 2063 6861 6e67 6520 6174 2073 6f6d  ht change at som
-0000c510: 6520 6c61 7465 7220 706f 696e 742e 0a20  e later point.. 
-0000c520: 2020 2020 2020 2043 7572 7265 6e74 6c79         Currently
-0000c530: 2c20 6974 2064 6570 656e 6473 206f 6e20  , it depends on 
-0000c540: 7468 6520 6372 6561 7469 6f6e 2069 6e64  the creation ind
-0000c550: 6578 2e0a 0a20 2020 2020 2020 203a 7061  ex...        :pa
-0000c560: 7261 6d20 4469 6d20 6f74 6865 723a 0a20  ram Dim other:. 
-0000c570: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-0000c580: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
-0000c590: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-0000c5a0: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-0000c5b0: 2028 5f64 2e44 696d 2c20 5f6d 2e4d 6172   (_d.Dim, _m.Mar
-0000c5c0: 6b65 6444 696d 2929 3a0a 2020 2020 2020  kedDim)):.      
-0000c5d0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-0000c5e0: 4572 726f 7228 2263 616e 6e6f 7420 636f  Error("cannot co
-0000c5f0: 6d70 6172 6520 2572 2077 6974 6820 2572  mpare %r with %r
-0000c600: 2220 2520 2873 656c 662c 206f 7468 6572  " % (self, other
-0000c610: 2929 0a20 2020 2020 2020 2069 6620 7365  )).        if se
-0000c620: 6c66 203d 3d20 6f74 6865 723a 0a20 2020  lf == other:.   
-0000c630: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000c640: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
-0000c650: 7475 726e 2064 696d 5f63 6d70 5f76 616c  turn dim_cmp_val
-0000c660: 7565 2873 656c 6629 203c 2064 696d 5f63  ue(self) < dim_c
-0000c670: 6d70 5f76 616c 7565 286f 7468 6572 290a  mp_value(other).
-0000c680: 0a20 2020 2064 6566 205f 5f67 745f 5f28  .    def __gt__(
-0000c690: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
-0000c6a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000c6b0: 2020 5365 6520 3a66 756e 633a 605f 5f6c    See :func:`__l
-0000c6c0: 745f 5f60 2e0a 0a20 2020 2020 2020 203a  t__`...        :
-0000c6d0: 7061 7261 6d20 4469 6d20 6f74 6865 723a  param Dim other:
-0000c6e0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-0000c6f0: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
-0000c700: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0000c710: 206f 7468 6572 203c 2073 656c 660a 0a20   other < self.. 
-0000c720: 2020 2064 6566 205f 5f67 655f 5f28 7365     def __ge__(se
-0000c730: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-0000c740: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
-0000c750: 656c 6620 3c20 6f74 6865 720a 0a20 2020  elf < other..   
-0000c760: 2064 6566 205f 5f6c 655f 5f28 7365 6c66   def __le__(self
-0000c770: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-0000c780: 2020 7265 7475 726e 206e 6f74 2073 656c    return not sel
-0000c790: 6620 3e20 6f74 6865 720a 0a20 2020 2064  f > other..    d
-0000c7a0: 6566 2067 6574 5f73 616d 655f 6261 7365  ef get_same_base
-0000c7b0: 2873 656c 663a 205f 642e 4469 6d29 202d  (self: _d.Dim) -
-0000c7c0: 3e20 5f64 2e44 696d 3a0a 2020 2020 2020  > _d.Dim:.      
-0000c7d0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
-0000c7e0: 6574 7572 6e3a 2073 616d 6520 6261 7365  eturn: same base
-0000c7f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c800: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0000c810: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
-0000c820: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000c830: 0a20 2020 2020 2020 2062 6173 6520 3d20  .        base = 
-0000c840: 7365 6c66 0a20 2020 2020 2020 2077 6869  self.        whi
-0000c850: 6c65 2062 6173 652e 7361 6d65 5f61 733a  le base.same_as:
-0000c860: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
-0000c870: 6520 3d20 6261 7365 2e73 616d 655f 6173  e = base.same_as
-0000c880: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c890: 6261 7365 0a0a 2020 2020 6465 6620 6765  base..    def ge
-0000c8a0: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
-0000c8b0: 6173 6528 7365 6c66 3a20 5f64 2e44 696d  ase(self: _d.Dim
-0000c8c0: 2920 2d3e 205f 642e 4469 6d3a 0a20 2020  ) -> _d.Dim:.   
-0000c8d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c8e0: 203a 7265 7475 726e 3a20 7361 6d65 2062   :return: same b
-0000c8f0: 6173 652c 2062 7574 2061 6c73 6f20 636f  ase, but also co
-0000c900: 6e73 6964 6572 2064 6572 6976 6564 5f66  nsider derived_f
-0000c910: 726f 6d5f 2e2e 2e0a 2020 2020 2020 2020  rom_....        
-0000c920: 2222 220a 2020 2020 2020 2020 6261 7365  """.        base
-0000c930: 203d 2073 656c 660a 2020 2020 2020 2020   = self.        
-0000c940: 7669 7369 7465 6420 3d20 7b7d 0a20 2020  visited = {}.   
-0000c950: 2020 2020 2077 6869 6c65 2062 6173 652e       while base.
-0000c960: 7361 6d65 5f61 7320 6f72 2062 6173 652e  same_as or base.
-0000c970: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
-0000c980: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
-0000c990: 7365 7274 2069 6428 6261 7365 2920 6e6f  sert id(base) no
-0000c9a0: 7420 696e 2076 6973 6974 6564 2020 2320  t in visited  # 
-0000c9b0: 7368 6f75 6c64 206e 6f74 2068 6176 6520  should not have 
-0000c9c0: 6379 636c 6573 2e20 6e6f 726d 616c 6c79  cycles. normally
-0000c9d0: 2074 6869 7320 7368 6f75 6c64 206e 6576   this should nev
-0000c9e0: 6572 2062 6520 7472 6967 6765 7265 640a  er be triggered.
-0000c9f0: 2020 2020 2020 2020 2020 2020 7669 7369              visi
-0000ca00: 7465 645b 6964 2862 6173 6529 5d20 3d20  ted[id(base)] = 
-0000ca10: 6261 7365 0a20 2020 2020 2020 2020 2020  base.           
-0000ca20: 2069 6620 6261 7365 2e73 616d 655f 6173   if base.same_as
-0000ca30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ca40: 2020 6261 7365 203d 2062 6173 652e 7361    base = base.sa
-0000ca50: 6d65 5f61 730a 2020 2020 2020 2020 2020  me_as.          
-0000ca60: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-0000ca70: 2020 2020 2020 2020 2020 2062 6173 6520             base 
-0000ca80: 3d20 6261 7365 2e64 6572 6976 6564 5f66  = base.derived_f
-0000ca90: 726f 6d5f 7461 670a 2020 2020 2020 2020  rom_tag.        
-0000caa0: 2020 2020 6173 7365 7274 2062 6173 650a      assert base.
-0000cab0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-0000cac0: 6173 650a 0a20 2020 2064 6566 2067 6574  ase..    def get
-0000cad0: 5f64 6572 6976 6564 5f62 6173 6573 5f73  _derived_bases_s
-0000cae0: 6574 2873 656c 6629 3a0a 2020 2020 2020  et(self):.      
-0000caf0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
-0000cb00: 7479 7065 3a20 7365 745b 4469 6d5d 0a20  type: set[Dim]. 
-0000cb10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000cb20: 2020 2072 6573 203d 2073 6574 2829 0a20     res = set(). 
-0000cb30: 2020 2020 2020 2071 7565 7565 203d 205b         queue = [
-0000cb40: 7365 6c66 5d0a 2020 2020 2020 2020 7669  self].        vi
-0000cb50: 7369 7465 6420 3d20 7b7d 2020 2320 7479  sited = {}  # ty
-0000cb60: 7065 3a20 4469 6374 5b69 6e74 2c5f 642e  pe: Dict[int,_d.
-0000cb70: 4469 6d5d 2020 2320 6279 2069 640a 2020  Dim]  # by id.  
-0000cb80: 2020 2020 2020 7768 696c 6520 7175 6575        while queu
-0000cb90: 653a 0a20 2020 2020 2020 2020 2020 2062  e:.            b
-0000cba0: 6173 6520 3d20 7175 6575 652e 706f 7028  ase = queue.pop(
-0000cbb0: 2d31 290a 2020 2020 2020 2020 2020 2020  -1).            
-0000cbc0: 6966 2062 6173 652e 7361 6d65 5f61 733a  if base.same_as:
-0000cbd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cbe0: 2062 6173 6520 3d20 6261 7365 2e73 616d   base = base.sam
-0000cbf0: 655f 6173 0a20 2020 2020 2020 2020 2020  e_as.           
-0000cc00: 2069 6620 6964 2862 6173 6529 2069 6e20   if id(base) in 
-0000cc10: 7669 7369 7465 643a 0a20 2020 2020 2020  visited:.       
-0000cc20: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0000cc30: 650a 2020 2020 2020 2020 2020 2020 7669  e.            vi
-0000cc40: 7369 7465 645b 6964 2862 6173 6529 5d20  sited[id(base)] 
-0000cc50: 3d20 6261 7365 0a20 2020 2020 2020 2020  = base.         
-0000cc60: 2020 2072 6573 2e61 6464 2862 6173 6529     res.add(base)
-0000cc70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000cc80: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
-0000cc90: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
-0000cca0: 2020 2020 2020 7175 6575 652e 6578 7465        queue.exte
-0000ccb0: 6e64 2862 6173 652e 6465 7269 7665 645f  nd(base.derived_
-0000ccc0: 6672 6f6d 5f6f 702e 696e 7075 7473 290a  from_op.inputs).
-0000ccd0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000cce0: 2062 6173 652e 6465 7269 7665 645f 6672   base.derived_fr
-0000ccf0: 6f6d 5f74 6167 3a0a 2020 2020 2020 2020  om_tag:.        
-0000cd00: 2020 2020 2020 2020 7175 6575 652e 6170          queue.ap
-0000cd10: 7065 6e64 2862 6173 652e 6465 7269 7665  pend(base.derive
-0000cd20: 645f 6672 6f6d 5f74 6167 290a 2020 2020  d_from_tag).    
-0000cd30: 2020 2020 7265 7475 726e 2072 6573 0a0a      return res..
-0000cd40: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000cd50: 2020 6465 6620 756e 6465 6669 6e65 6428    def undefined(
-0000cd60: 7365 6c66 3a20 5f64 2e44 696d 2920 2d3e  self: _d.Dim) ->
-0000cd70: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-0000cd80: 2222 0a20 2020 2020 2020 203a 7265 7475  "".        :retu
-0000cd90: 726e 3a20 7768 6574 6865 7220 7468 6520  rn: whether the 
-0000cda0: 756e 6465 6669 6e65 6420 666c 6167 2069  undefined flag i
-0000cdb0: 7320 7365 742c 2069 6e20 7365 6c66 2c20  s set, in self, 
-0000cdc0: 6261 7365 732c 206f 7220 616e 7920 6465  bases, or any de
-0000cdd0: 7269 7665 6420 6261 7365 732e 2061 6c73  rived bases. als
-0000cde0: 6f20 7365 6520 3a66 756e 633a 6069 735f  o see :func:`is_
-0000cdf0: 6469 6d5f 6b6e 6f77 6e60 0a20 2020 2020  dim_known`.     
-0000ce00: 2020 2022 2222 0a20 2020 2020 2020 2062     """.        b
-0000ce10: 6173 6520 3d20 7365 6c66 0a20 2020 2020  ase = self.     
-0000ce20: 2020 2076 6973 6974 6564 203d 207b 7d0a     visited = {}.
-0000ce30: 2020 2020 2020 2020 7768 696c 6520 6261          while ba
-0000ce40: 7365 2e73 616d 655f 6173 206f 7220 6261  se.same_as or ba
-0000ce50: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
-0000ce60: 7461 673a 0a20 2020 2020 2020 2020 2020  tag:.           
-0000ce70: 2061 7373 6572 7420 6964 2862 6173 6529   assert id(base)
-0000ce80: 206e 6f74 2069 6e20 7669 7369 7465 6420   not in visited 
-0000ce90: 2023 2073 686f 756c 6420 6e6f 7420 6861   # should not ha
-0000cea0: 7665 2063 7963 6c65 732e 206e 6f72 6d61  ve cycles. norma
-0000ceb0: 6c6c 7920 7468 6973 2073 686f 756c 6420  lly this should 
-0000cec0: 6e65 7665 7220 6265 2074 7269 6767 6572  never be trigger
-0000ced0: 6564 0a20 2020 2020 2020 2020 2020 2076  ed.            v
-0000cee0: 6973 6974 6564 5b69 6428 6261 7365 295d  isited[id(base)]
-0000cef0: 203d 2062 6173 650a 2020 2020 2020 2020   = base.        
-0000cf00: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
-0000cf10: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
-0000cf20: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-0000cf30: 2069 6620 6261 7365 2e5f 6578 7472 6120   if base._extra 
-0000cf40: 616e 6420 6261 7365 2e5f 6578 7472 612e  and base._extra.
-0000cf50: 756e 6465 6669 6e65 643a 0a20 2020 2020  undefined:.     
-0000cf60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000cf70: 6e20 5472 7565 0a20 2020 2020 2020 2020  n True.         
-0000cf80: 2020 2069 6620 6261 7365 2e73 616d 655f     if base.same_
-0000cf90: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
-0000cfa0: 2020 2020 6261 7365 203d 2062 6173 652e      base = base.
-0000cfb0: 7361 6d65 5f61 730a 2020 2020 2020 2020  same_as.        
-0000cfc0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0000cfd0: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
-0000cfe0: 6520 3d20 6261 7365 2e64 6572 6976 6564  e = base.derived
-0000cff0: 5f66 726f 6d5f 7461 670a 2020 2020 2020  _from_tag.      
-0000d000: 2020 2020 2020 6173 7365 7274 2062 6173        assert bas
-0000d010: 650a 2020 2020 2020 2020 2320 6e6f 696e  e.        # noin
-0000d020: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-0000d030: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-0000d040: 2020 2072 6574 7572 6e20 6261 7365 2e5f     return base._
-0000d050: 6578 7472 6120 616e 6420 6261 7365 2e5f  extra and base._
-0000d060: 6578 7472 612e 756e 6465 6669 6e65 640a  extra.undefined.
-0000d070: 0a20 2020 2064 6566 2064 6563 6c61 7265  .    def declare
-0000d080: 5f73 616d 655f 6173 2873 656c 663a 205f  _same_as(self: _
-0000d090: 642e 4469 6d2c 206f 7468 6572 3a20 5f64  d.Dim, other: _d
-0000d0a0: 2e44 696d 293a 0a20 2020 2020 2020 2022  .Dim):.        "
-0000d0b0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-0000d0c0: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
-0000d0d0: 2022 2222 0a20 2020 2020 2020 2061 7373   """.        ass
-0000d0e0: 6572 7420 7365 6c66 2e63 616e 5f62 655f  ert self.can_be_
-0000d0f0: 7573 6564 5f61 735f 6469 6d28 2920 616e  used_as_dim() an
-0000d100: 6420 6f74 6865 722e 6361 6e5f 6265 5f75  d other.can_be_u
-0000d110: 7365 645f 6173 5f64 696d 2829 2020 2320  sed_as_dim()  # 
-0000d120: 6465 636c 6172 655f 7361 6d65 5f61 7320  declare_same_as 
-0000d130: 646f 6573 206e 6f74 206d 616b 6520 7365  does not make se
-0000d140: 6e73 6520 6f74 6865 7277 6973 650a 2020  nse otherwise.  
-0000d150: 2020 2020 2020 2320 4e6f 7465 3a20 4368        # Note: Ch
-0000d160: 6563 6b20 6069 7360 2c20 6e6f 7420 603d  eck `is`, not `=
-0000d170: 3d60 2e20 603d 3d60 2063 616e 2062 6520  =`. `==` can be 
-0000d180: 7472 7565 2065 7665 6e20 7468 6f75 6768  true even though
-0000d190: 2073 616d 655f 6173 2061 7265 206e 6f74   same_as are not
-0000d1a0: 2074 6865 2073 616d 6520 696e 7374 616e   the same instan
-0000d1b0: 6365 2c0a 2020 2020 2020 2020 2320 652e  ce,.        # e.
-0000d1c0: 672e 2076 6961 2061 7574 6f5f 6765 6e65  g. via auto_gene
-0000d1d0: 7261 7465 642e 0a20 2020 2020 2020 2069  rated..        i
-0000d1e0: 6620 7365 6c66 2069 7320 6f74 6865 723a  f self is other:
-0000d1f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000d200: 7572 6e0a 2020 2020 2020 2020 7365 6c66  urn.        self
-0000d210: 2e5f 6d61 7962 655f 7570 6461 7465 2829  ._maybe_update()
-0000d220: 0a20 2020 2020 2020 2073 656c 662e 5f76  .        self._v
-0000d230: 616c 6964 6174 655f 696e 5f63 7572 7265  alidate_in_curre
-0000d240: 6e74 5f67 7261 7068 2829 0a20 2020 2020  nt_graph().     
-0000d250: 2020 206f 7468 6572 2e5f 7661 6c69 6461     other._valida
-0000d260: 7465 5f69 6e5f 6375 7272 656e 745f 6772  te_in_current_gr
-0000d270: 6170 6828 290a 2020 2020 2020 2020 6f74  aph().        ot
-0000d280: 6865 725f 7361 6d65 5f62 6173 6520 3d20  her_same_base = 
-0000d290: 6f74 6865 722e 6765 745f 7361 6d65 5f62  other.get_same_b
-0000d2a0: 6173 6528 290a 2020 2020 2020 2020 6966  ase().        if
-0000d2b0: 2073 656c 6620 6973 206f 7468 6572 5f73   self is other_s
-0000d2c0: 616d 655f 6261 7365 206f 7220 7365 6c66  ame_base or self
-0000d2d0: 2e73 616d 655f 6173 2069 7320 6f74 6865  .same_as is othe
-0000d2e0: 725f 7361 6d65 5f62 6173 653a 0a20 2020  r_same_base:.   
-0000d2f0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000d300: 2020 2020 2020 2020 7365 6c66 5f73 616d          self_sam
-0000d310: 655f 6173 203d 2073 656c 662e 6765 745f  e_as = self.get_
-0000d320: 7361 6d65 5f62 6173 6528 290a 2020 2020  same_base().    
-0000d330: 2020 2020 6966 2073 656c 665f 7361 6d65      if self_same
-0000d340: 5f61 7320 6973 206f 7468 6572 5f73 616d  _as is other_sam
-0000d350: 655f 6261 7365 3a0a 2020 2020 2020 2020  e_base:.        
-0000d360: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000d370: 2020 2069 6620 6f74 6865 725f 7361 6d65     if other_same
-0000d380: 5f62 6173 652e 6765 745f 7361 6d65 5f64  _base.get_same_d
-0000d390: 6572 6976 6564 5f62 6173 6528 2920 6973  erived_base() is
-0000d3a0: 2073 656c 665f 7361 6d65 5f61 733a 0a20   self_same_as:. 
-0000d3b0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
-0000d3c0: 6163 7475 616c 6c79 2077 616e 7420 6974  actually want it
-0000d3d0: 2074 6f20 6265 2074 6865 206f 7468 6572   to be the other
-0000d3e0: 2077 6179 2061 726f 756e 642e 0a20 2020   way around..   
-0000d3f0: 2020 2020 2020 2020 2077 6974 6820 7574           with ut
-0000d400: 696c 2e67 7561 7264 5f69 6e66 696e 6974  il.guard_infinit
-0000d410: 655f 7265 6375 7273 696f 6e28 5f64 2e44  e_recursion(_d.D
-0000d420: 696d 2e64 6563 6c61 7265 5f73 616d 655f  im.declare_same_
-0000d430: 6173 2c20 6f74 6865 722c 2073 656c 6629  as, other, self)
-0000d440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d450: 2020 7265 7475 726e 206f 7468 6572 2e64    return other.d
-0000d460: 6563 6c61 7265 5f73 616d 655f 6173 2873  eclare_same_as(s
-0000d470: 656c 6629 0a20 2020 2020 2020 2069 6620  elf).        if 
-0000d480: 7365 6c66 2e62 6174 6368 3a0a 2020 2020  self.batch:.    
-0000d490: 2020 2020 2020 2020 2320 4966 2073 656c          # If sel
-0000d4a0: 6620 6973 2064 6566 696e 6564 2028 7365  f is defined (se
-0000d4b0: 6c66 2e69 735f 6469 6d5f 6b6e 6f77 6e29  lf.is_dim_known)
-0000d4c0: 2c20 6265 2066 6169 7220 746f 206f 7468  , be fair to oth
-0000d4d0: 6572 2c20 616e 6420 6164 6170 7420 6974  er, and adapt it
-0000d4e0: 2074 6f20 7468 6520 7269 6768 7420 6261   to the right ba
-0000d4f0: 7463 682c 0a20 2020 2020 2020 2020 2020  tch,.           
-0000d500: 2023 2073 7563 6820 7468 6174 206f 7468   # such that oth
-0000d510: 6572 2e69 735f 6469 6d5f 6b6e 6f77 6e20  er.is_dim_known 
-0000d520: 6973 2063 6f72 7265 6374 2c20 6279 2070  is correct, by p
-0000d530: 6f74 656e 7469 616c 6c79 2063 6f6d 706c  otentially compl
-0000d540: 6574 696e 6720 6974 2e0a 2020 2020 2020  eting it..      
-0000d550: 2020 2020 2020 6f74 6865 725f 203d 206f        other_ = o
-0000d560: 7468 6572 2e67 6574 5f66 6f72 5f62 6174  ther.get_for_bat
-0000d570: 6368 5f63 7478 2873 656c 662e 6261 7463  ch_ctx(self.batc
-0000d580: 682c 2063 7478 3d73 656c 662e 636f 6e74  h, ctx=self.cont
-0000d590: 726f 6c5f 666c 6f77 5f63 7478 290a 2020  rol_flow_ctx).  
-0000d5a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000d5b0: 2020 2020 2020 2020 6f74 6865 725f 203d          other_ =
-0000d5c0: 206f 7468 6572 0a20 2020 2020 2020 2069   other.        i
-0000d5d0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-0000d5e0: 2873 656c 662e 6973 5f64 696d 5f6b 6e6f  (self.is_dim_kno
-0000d5f0: 776e 2829 2061 6e64 206e 6f74 206f 7468  wn() and not oth
-0000d600: 6572 5f2e 6973 5f64 696d 5f6b 6e6f 776e  er_.is_dim_known
-0000d610: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-0000d620: 6f72 0a20 2020 2020 2020 2020 2020 2023  or.            #
-0000d630: 204c 696b 6520 6973 5f64 696d 5f6b 6e6f   Like is_dim_kno
-0000d640: 776e 2062 7574 2066 6f72 2073 7461 7469  wn but for stati
-0000d650: 6320 6469 6d73 2c20 7765 206d 6967 6874  c dims, we might
-0000d660: 206b 6e6f 7720 626f 7468 2c0a 2020 2020   know both,.    
-0000d670: 2020 2020 2020 2020 2320 6275 7420 7468          # but th
-0000d680: 6520 6465 7269 7665 645f 6672 6f6d 5f6f  e derived_from_o
-0000d690: 7020 7374 696c 6c20 776f 756c 6420 7072  p still would pr
-0000d6a0: 6f76 6964 6520 6d6f 7265 2069 6e66 6f72  ovide more infor
-0000d6b0: 6d61 7469 6f6e 2e0a 2020 2020 2020 2020  mation..        
-0000d6c0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-0000d6d0: 2020 2020 2020 7365 6c66 5f73 616d 655f        self_same_
-0000d6e0: 6173 2e64 6572 6976 6564 5f66 726f 6d5f  as.derived_from_
-0000d6f0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
-0000d700: 2020 2061 6e64 206e 6f74 206f 7468 6572     and not other
-0000d710: 5f73 616d 655f 6261 7365 2e64 6572 6976  _same_base.deriv
-0000d720: 6564 5f66 726f 6d5f 6f70 0a20 2020 2020  ed_from_op.     
-0000d730: 2020 2020 2020 2020 2020 2061 6e64 206f             and o
-0000d740: 7468 6572 206e 6f74 2069 6e20 7365 6c66  ther not in self
-0000d750: 2e67 6574 5f64 6572 6976 6564 5f62 6173  .get_derived_bas
-0000d760: 6573 5f73 6574 2829 0a20 2020 2020 2020  es_set().       
-0000d770: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000d780: 2020 206f 7220 286e 6f74 2073 656c 662e     or (not self.
-0000d790: 756e 6465 6669 6e65 6420 616e 6420 6f74  undefined and ot
-0000d7a0: 6865 725f 2e75 6e64 6566 696e 6564 290a  her_.undefined).
-0000d7b0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-0000d7c0: 2020 2020 2020 2077 6974 6820 7574 696c         with util
-0000d7d0: 2e67 7561 7264 5f69 6e66 696e 6974 655f  .guard_infinite_
-0000d7e0: 7265 6375 7273 696f 6e28 5f64 2e44 696d  recursion(_d.Dim
-0000d7f0: 2e64 6563 6c61 7265 5f73 616d 655f 6173  .declare_same_as
-0000d800: 2c20 6f74 6865 722c 2073 656c 6629 3a0a  , other, self):.
-0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d820: 7265 7475 726e 206f 7468 6572 2e64 6563  return other.dec
-0000d830: 6c61 7265 5f73 616d 655f 6173 2873 656c  lare_same_as(sel
-0000d840: 6629 0a20 2020 2020 2020 206f 7468 6572  f).        other
-0000d850: 5f64 6572 6976 6564 5f62 6173 6573 203d  _derived_bases =
-0000d860: 206f 7468 6572 2e67 6574 5f64 6572 6976   other.get_deriv
-0000d870: 6564 5f62 6173 6573 5f73 6574 2829 0a20  ed_bases_set(). 
-0000d880: 2020 2020 2020 2073 656c 665f 6465 7269         self_deri
-0000d890: 7665 645f 6261 7365 7320 3d20 7365 6c66  ved_bases = self
-0000d8a0: 2e67 6574 5f64 6572 6976 6564 5f62 6173  .get_derived_bas
-0000d8b0: 6573 5f73 6574 2829 0a20 2020 2020 2020  es_set().       
-0000d8c0: 2069 6620 6f74 6865 725f 6465 7269 7665   if other_derive
-0000d8d0: 645f 6261 7365 7320 213d 2073 656c 665f  d_bases != self_
-0000d8e0: 6465 7269 7665 645f 6261 7365 7320 616e  derived_bases an
-0000d8f0: 6420 7365 6c66 5f64 6572 6976 6564 5f62  d self_derived_b
-0000d900: 6173 6573 2e69 7373 7562 7365 7428 6f74  ases.issubset(ot
-0000d910: 6865 725f 6465 7269 7665 645f 6261 7365  her_derived_base
-0000d920: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000d930: 2320 4176 6f69 6420 6379 636c 6573 206f  # Avoid cycles o
-0000d940: 6e20 6465 7269 7665 645f 6672 6f6d 5f74  n derived_from_t
-0000d950: 6167 2e20 6874 7470 733a 2f2f 6769 7468  ag. https://gith
-0000d960: 7562 2e63 6f6d 2f72 7774 682d 6936 2f72  ub.com/rwth-i6/r
-0000d970: 6574 7572 6e6e 2f69 7373 7565 732f 3130  eturnn/issues/10
-0000d980: 3534 0a20 2020 2020 2020 2020 2020 2077  54.            w
-0000d990: 6974 6820 7574 696c 2e67 7561 7264 5f69  ith util.guard_i
-0000d9a0: 6e66 696e 6974 655f 7265 6375 7273 696f  nfinite_recursio
-0000d9b0: 6e28 5f64 2e44 696d 2e64 6563 6c61 7265  n(_d.Dim.declare
-0000d9c0: 5f73 616d 655f 6173 2c20 6f74 6865 722c  _same_as, other,
-0000d9d0: 2073 656c 6629 3a0a 2020 2020 2020 2020   self):.        
-0000d9e0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0000d9f0: 7468 6572 2e64 6563 6c61 7265 5f73 616d  ther.declare_sam
-0000da00: 655f 6173 2873 656c 6629 0a20 2020 2020  e_as(self).     
-0000da10: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
-0000da20: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
-0000da30: 656c 662e 5f65 7874 7261 2e64 6572 6976  elf._extra.deriv
-0000da40: 6564 5f66 726f 6d5f 6f70 203d 204e 6f6e  ed_from_op = Non
-0000da50: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-0000da60: 6c66 2e5f 6578 7472 612e 6465 7269 7665  lf._extra.derive
-0000da70: 645f 6672 6f6d 5f74 6167 203d 204e 6f6e  d_from_tag = Non
-0000da80: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0000da90: 665f 7361 6d65 5f61 7320 6973 206e 6f74  f_same_as is not
-0000daa0: 2073 656c 663a 0a20 2020 2020 2020 2020   self:.         
-0000dab0: 2020 2061 7373 6572 7420 6e6f 7420 7365     assert not se
-0000dac0: 6c66 5f73 616d 655f 6173 2e73 616d 655f  lf_same_as.same_
-0000dad0: 6173 0a20 2020 2020 2020 2020 2020 2069  as.            i
-0000dae0: 6620 7365 6c66 5f73 616d 655f 6173 2069  f self_same_as i
-0000daf0: 7320 6f74 6865 725f 7361 6d65 5f62 6173  s other_same_bas
-0000db00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000db10: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000db20: 2020 2020 2020 7769 7468 2075 7469 6c2e        with util.
-0000db30: 6775 6172 645f 696e 6669 6e69 7465 5f72  guard_infinite_r
-0000db40: 6563 7572 7369 6f6e 285f 642e 4469 6d2e  ecursion(_d.Dim.
-0000db50: 6465 636c 6172 655f 7361 6d65 5f61 732c  declare_same_as,
-0000db60: 2073 656c 665f 7361 6d65 5f61 732c 206f   self_same_as, o
-0000db70: 7468 6572 5f73 616d 655f 6261 7365 293a  ther_same_base):
-0000db80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000db90: 2073 656c 665f 7361 6d65 5f61 732e 6465   self_same_as.de
-0000dba0: 636c 6172 655f 7361 6d65 5f61 7328 6f74  clare_same_as(ot
-0000dbb0: 6865 725f 7361 6d65 5f62 6173 6529 0a20  her_same_base). 
-0000dbc0: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
-0000dbd0: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-0000dbe0: 2069 7320 4e6f 6e65 206f 7220 6e6f 7420   is None or not 
-0000dbf0: 7365 6c66 2e5f 7661 6c69 6461 7465 5f69  self._validate_i
-0000dc00: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
-0000dc10: 2929 2061 6e64 2073 656c 665f 7361 6d65  )) and self_same
-0000dc20: 5f61 732e 6479 6e5f 7369 7a65 5f65 7874  _as.dyn_size_ext
-0000dc30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000dc40: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
-0000dc50: 6578 7420 3d20 7365 6c66 5f73 616d 655f  ext = self_same_
-0000dc60: 6173 2e67 6574 5f64 796e 5f73 697a 655f  as.get_dyn_size_
-0000dc70: 6578 745f 666f 725f 6261 7463 685f 6374  ext_for_batch_ct
-0000dc80: 7828 0a20 2020 2020 2020 2020 2020 2020  x(.             
-0000dc90: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
-0000dca0: 682c 2073 656c 662e 636f 6e74 726f 6c5f  h, self.control_
-0000dcb0: 666c 6f77 5f63 7478 2c20 7465 6d70 6c61  flow_ctx, templa
-0000dcc0: 7465 5f6f 6e6c 793d 5472 7565 0a20 2020  te_only=True.   
-0000dcd0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000dce0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000dcf0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000dd00: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
-0000dd10: 2020 2020 2020 2020 2066 6f72 2064 696d           for dim
-0000dd20: 5f20 696e 2073 656c 662e 5f65 7874 7261  _ in self._extra
-0000dd30: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-0000dd40: 6374 782e 7661 6c75 6573 2829 3a0a 2020  ctx.values():.  
-0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd60: 2020 2320 6e6f 696e 7370 6563 7469 6f6e    # noinspection
-0000dd70: 2050 7950 726f 7465 6374 6564 4d65 6d62   PyProtectedMemb
-0000dd80: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-0000dd90: 2020 2020 2020 2069 6620 6469 6d5f 2e5f         if dim_._
-0000dda0: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
-0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000ddc0: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
-0000ddd0: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
-0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddf0: 2020 2020 2020 2020 6469 6d5f 2e5f 6578          dim_._ex
-0000de00: 7472 612e 6465 7269 7665 645f 6672 6f6d  tra.derived_from
-0000de10: 5f6f 7020 3d20 4e6f 6e65 0a20 2020 2020  _op = None.     
+0000ba20: 2028 7365 6c66 2e64 696d 656e 7369 6f6e   (self.dimension
+0000ba30: 203d 3d20 3120 616e 6420 7365 6c66 2e61   == 1 and self.a
+0000ba40: 7574 6f5f 6765 6e65 7261 7465 6429 206f  uto_generated) o
+0000ba50: 7220 286f 7468 6572 2e64 696d 656e 7369  r (other.dimensi
+0000ba60: 6f6e 203d 3d20 3120 616e 6420 6f74 6865  on == 1 and othe
+0000ba70: 722e 6175 746f 5f67 656e 6572 6174 6564  r.auto_generated
+0000ba80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ba90: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0000baa0: 2020 2020 2020 2020 2070 6173 7320 2023           pass  #
+0000bab0: 2065 7863 6570 7469 6f6e 2c20 616c 6c6f   exception, allo
+0000bac0: 7720 6272 6f61 6463 6173 7420 6c6f 6769  w broadcast logi
+0000bad0: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
+0000bae0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000baf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000bb00: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0000bb10: 2069 6620 7365 6c66 5f6b 696e 6420 3d3d   if self_kind ==
+0000bb20: 206f 7468 6572 5f6b 696e 6420 3d3d 2044   other_kind == D
+0000bb30: 696d 5479 7065 732e 4665 6174 7572 653a  imTypes.Feature:
+0000bb40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bb50: 616c 6c6f 775f 7361 6d65 5f66 6561 7475  allow_same_featu
+0000bb60: 7265 5f64 696d 3a0a 2020 2020 2020 2020  re_dim:.        
+0000bb70: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0000bb80: 7275 650a 2020 2020 2020 2020 6966 2073  rue.        if s
+0000bb90: 656c 665f 6b69 6e64 203d 3d20 6f74 6865  elf_kind == othe
+0000bba0: 725f 6b69 6e64 203d 3d20 4469 6d54 7970  r_kind == DimTyp
+0000bbb0: 6573 2e53 7061 7469 616c 3a0a 2020 2020  es.Spatial:.    
+0000bbc0: 2020 2020 2020 2020 6966 2061 6c6c 6f77          if allow
+0000bbd0: 5f73 616d 655f 7370 6174 6961 6c5f 6469  _same_spatial_di
+0000bbe0: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
+0000bbf0: 2020 2069 6620 7365 6c66 2e64 696d 656e     if self.dimen
+0000bc00: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
+0000bc10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bc20: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0000bc30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000bc40: 2020 6966 2062 726f 6164 6361 7374 5f6d    if broadcast_m
+0000bc50: 6174 6368 6573 2061 6e64 2028 7365 6c66  atches and (self
+0000bc60: 2e64 696d 656e 7369 6f6e 203d 3d20 3120  .dimension == 1 
+0000bc70: 6f72 206f 7468 6572 2e64 696d 656e 7369  or other.dimensi
+0000bc80: 6f6e 203d 3d20 3129 3a0a 2020 2020 2020  on == 1):.      
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000bca0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+0000bcb0: 2020 2020 2020 6966 2075 6e6b 6e6f 776e        if unknown
+0000bcc0: 5f73 7061 7469 616c 5f6d 6174 6368 6573  _spatial_matches
+0000bcd0: 2061 6e64 2028 2873 656c 662e 6479 6e5f   and ((self.dyn_
+0000bce0: 7369 7a65 2069 7320 4e6f 6e65 2920 6f72  size is None) or
+0000bcf0: 2028 6f74 6865 722e 6479 6e5f 7369 7a65   (other.dyn_size
+0000bd00: 2069 7320 4e6f 6e65 2929 3a0a 2020 2020   is None)):.    
+0000bd10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000bd20: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+0000bd30: 2020 2020 6966 2075 6e64 6566 696e 6564      if undefined
+0000bd40: 5f6d 6174 6368 6573 2061 6e64 2028 7365  _matches and (se
+0000bd50: 6c66 2e75 6e64 6566 696e 6564 206f 7220  lf.undefined or 
+0000bd60: 6f74 6865 722e 756e 6465 6669 6e65 6429  other.undefined)
+0000bd70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bd80: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000bd90: 2020 2020 2020 2320 496e 2070 7269 6e63        # In princ
+0000bda0: 6970 6c65 2c20 7765 2077 6f75 6c64 2077  iple, we would w
+0000bdb0: 616e 7420 746f 2063 6865 636b 2066 6f72  ant to check for
+0000bdc0: 2069 6465 6e74 6974 7920 2873 656c 6620   identity (self 
+0000bdd0: 6973 206f 7468 6572 292e 0a20 2020 2020  is other)..     
+0000bde0: 2020 2023 2057 6520 6375 7272 656e 746c     # We currentl
+0000bdf0: 7920 7573 6520 7468 6520 6465 7363 7269  y use the descri
+0000be00: 7074 696f 6e20 6265 6361 7573 6520 7468  ption because th
+0000be10: 6520 6964 656e 7469 7479 2077 6f75 6c64  e identity would
+0000be20: 206e 6f74 2062 6520 7468 6520 7361 6d65   not be the same
+0000be30: 0a20 2020 2020 2020 2023 2069 6e20 6361  .        # in ca
+0000be40: 7365 206f 6620 7465 6d70 6c61 7465 2063  se of template c
+0000be50: 6f6e 7374 7275 6374 696f 6e20 7768 6572  onstruction wher
+0000be60: 6520 6120 6469 6d20 7461 6720 6973 206f  e a dim tag is o
+0000be70: 6e63 6520 6372 6561 7465 6420 666f 7220  nce created for 
+0000be80: 6120 7465 6d70 6c61 7465 206c 6179 6572  a template layer
+0000be90: 2c0a 2020 2020 2020 2020 2320 616e 6420  ,.        # and 
+0000bea0: 7468 656e 206c 6174 6572 2061 6761 696e  then later again
+0000beb0: 2066 6f72 2074 6865 2072 6561 6c20 6c61   for the real la
+0000bec0: 7965 722e 0a20 2020 2020 2020 2069 6620  yer..        if 
+0000bed0: 7365 6c66 2e61 7574 6f5f 6765 6e65 7261  self.auto_genera
+0000bee0: 7465 6420 616e 6420 6f74 6865 722e 6175  ted and other.au
+0000bef0: 746f 5f67 656e 6572 6174 6564 2061 6e64  to_generated and
+0000bf00: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+0000bf10: 6e20 3d3d 206f 7468 6572 2e64 6573 6372  n == other.descr
+0000bf20: 6970 7469 6f6e 3a0a 2020 2020 2020 2020  iption:.        
+0000bf30: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000bf40: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0000bf50: 616c 7365 0a0a 2020 2020 6465 6620 5f5f  alse..    def __
+0000bf60: 6571 5f5f 2873 656c 662c 206f 7468 6572  eq__(self, other
+0000bf70: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000bf80: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+0000bf90: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
+0000bfa0: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+0000bfb0: 2020 2020 2020 3a72 6574 7572 6e3a 203a        :return: :
+0000bfc0: 6675 6e63 3a60 6973 5f65 7175 616c 6020  func:`is_equal` 
+0000bfd0: 7769 7468 2064 6566 6175 6c74 206f 7074  with default opt
+0000bfe0: 696f 6e73 0a20 2020 2020 2020 2022 2222  ions.        """
+0000bff0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000c000: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+0000c010: 2c20 5f64 2e44 696d 293a 0a20 2020 2020  , _d.Dim):.     
+0000c020: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0000c030: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
+0000c040: 726e 2073 656c 662e 6973 5f65 7175 616c  rn self.is_equal
+0000c050: 286f 7468 6572 290a 0a20 2020 2064 6566  (other)..    def
+0000c060: 205f 5f6e 655f 5f28 7365 6c66 3a20 4469   __ne__(self: Di
+0000c070: 6d2c 206f 7468 6572 3a20 4469 6d29 3a0a  m, other: Dim):.
+0000c080: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c090: 2020 2020 3a70 6172 616d 2044 696d 206f      :param Dim o
+0000c0a0: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
+0000c0b0: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
+0000c0c0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0000c0d0: 6574 7572 6e20 6e6f 7420 2873 656c 6620  eturn not (self 
+0000c0e0: 3d3d 206f 7468 6572 290a 0a20 2020 2064  == other)..    d
+0000c0f0: 6566 205f 5f68 6173 685f 5f28 7365 6c66  ef __hash__(self
+0000c100: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000c110: 2020 2020 2020 203a 7274 7970 653a 2069         :rtype: i
+0000c120: 6e74 0a20 2020 2020 2020 203a 7265 7475  nt.        :retu
+0000c130: 726e 3a20 6861 7368 2c20 6d61 7463 6869  rn: hash, matchi
+0000c140: 6e67 2074 6f20 3a66 756e 633a 605f 5f65  ng to :func:`__e
+0000c150: 715f 5f60 0a20 2020 2020 2020 2022 2222  q__`.        """
+0000c160: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+0000c170: 6d75 7374 206d 6174 6368 2074 6865 2062  must match the b
+0000c180: 6568 6176 696f 7220 696e 205f 5f65 715f  ehavior in __eq_
+0000c190: 5f2c 2077 6869 6368 2069 7320 6973 5f65  _, which is is_e
+0000c1a0: 7175 616c 2077 6974 6820 6465 6661 756c  qual with defaul
+0000c1b0: 7420 6f70 7469 6f6e 732e 0a20 2020 2020  t options..     
+0000c1c0: 2020 2023 2049 2e65 2e20 6469 6666 6572     # I.e. differ
+0000c1d0: 656e 7420 6861 7368 2069 6d70 6c69 6573  ent hash implies
+0000c1e0: 206e 6f74 2065 7175 616c 2028 6275 7420   not equal (but 
+0000c1f0: 7361 6d65 2068 6173 6820 6e6f 7420 6e65  same hash not ne
+0000c200: 6365 7373 6172 696c 7920 6571 7561 6c29  cessarily equal)
+0000c210: 2e0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000c220: 662e 7370 6563 6961 6c3a 0a20 2020 2020  f.special:.     
+0000c230: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
+0000c240: 7368 2869 6428 7365 6c66 2929 0a20 2020  sh(id(self)).   
+0000c250: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
+0000c260: 6261 7463 685f 6469 6d28 293a 0a20 2020  batch_dim():.   
+0000c270: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000c280: 6861 7368 2828 2929 0a20 2020 2020 2020  hash(()).       
+0000c290: 2077 6974 6820 7574 696c 2e67 7561 7264   with util.guard
+0000c2a0: 5f69 6e66 696e 6974 655f 7265 6375 7273  _infinite_recurs
+0000c2b0: 696f 6e28 5f64 2e44 696d 2e5f 5f68 6173  ion(_d.Dim.__has
+0000c2c0: 685f 5f2c 2073 656c 6629 3a0a 2020 2020  h__, self):.    
+0000c2d0: 2020 2020 2020 2020 6261 7365 203d 2073          base = s
+0000c2e0: 656c 662e 6765 745f 7361 6d65 5f62 6173  elf.get_same_bas
+0000c2f0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000c300: 6966 2062 6173 6520 6973 206e 6f74 2073  if base is not s
+0000c310: 656c 663a 0a20 2020 2020 2020 2020 2020  elf:.           
+0000c320: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
+0000c330: 2862 6173 6529 0a20 2020 2020 2020 2020  (base).         
+0000c340: 2020 2069 6620 7365 6c66 2e64 6572 6976     if self.deriv
+0000c350: 6564 5f66 726f 6d5f 6f70 3a0a 2020 2020  ed_from_op:.    
+0000c360: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c370: 726e 2068 6173 6828 7365 6c66 2e64 6572  rn hash(self.der
+0000c380: 6976 6564 5f66 726f 6d5f 6f70 290a 2020  ived_from_op).  
+0000c390: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000c3a0: 662e 6175 746f 5f67 656e 6572 6174 6564  f.auto_generated
+0000c3b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c3c0: 2020 7265 7475 726e 2068 6173 6828 2862    return hash((b
+0000c3d0: 6173 652e 6b69 6e64 2c20 6261 7365 2e64  ase.kind, base.d
+0000c3e0: 696d 656e 7369 6f6e 2c20 6261 7365 2e64  imension, base.d
+0000c3f0: 6573 6372 6970 7469 6f6e 2929 0a20 2020  escription)).   
+0000c400: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000c410: 6861 7368 2869 6428 6261 7365 2929 0a0a  hash(id(base))..
+0000c420: 2020 2020 6465 6620 5f5f 6c74 5f5f 2873      def __lt__(s
+0000c430: 656c 663a 2044 696d 2c20 6f74 6865 723a  elf: Dim, other:
+0000c440: 2044 696d 293a 0a20 2020 2020 2020 2022   Dim):.        "
+0000c450: 2222 0a20 2020 2020 2020 2044 6566 696e  "".        Defin
+0000c460: 6520 736f 6d65 206f 7264 6572 2e20 5468  e some order. Th
+0000c470: 6973 2069 7320 6a75 7374 2073 7563 6820  is is just such 
+0000c480: 7468 6174 2060 736f 7274 6564 6020 776f  that `sorted` wo
+0000c490: 726b 732c 206f 7220 736f 6d65 2064 6966  rks, or some dif
+0000c4a0: 6620 7265 706f 7274 696e 672c 206f 7220  f reporting, or 
+0000c4b0: 736f 2e0a 2020 2020 2020 2020 4974 2069  so..        It i
+0000c4c0: 7320 6f6e 2073 796d 626f 6c69 6320 6c65  s on symbolic le
+0000c4d0: 7665 6c2c 2069 2e65 2e20 6974 2064 6f65  vel, i.e. it doe
+0000c4e0: 7320 6e6f 7420 636f 6e73 6964 6572 2074  s not consider t
+0000c4f0: 6865 2061 6374 7561 6c20 6469 6d65 6e73  he actual dimens
+0000c500: 696f 6e20 7661 6c75 652e 0a20 2020 2020  ion value..     
+0000c510: 2020 2054 6865 2064 6566 696e 6564 206f     The defined o
+0000c520: 7264 6572 2073 6f6d 6577 6861 7420 6172  rder somewhat ar
+0000c530: 6269 7472 6172 792c 2073 6f20 646f 206e  bitrary, so do n
+0000c540: 6f74 2072 656c 7920 6f6e 2074 6865 2065  ot rely on the e
+0000c550: 7861 6374 2062 6568 6176 696f 722c 0a20  xact behavior,. 
+0000c560: 2020 2020 2020 2061 7320 7468 6973 206d         as this m
+0000c570: 6967 6874 2063 6861 6e67 6520 6174 2073  ight change at s
+0000c580: 6f6d 6520 6c61 7465 7220 706f 696e 742e  ome later point.
+0000c590: 0a20 2020 2020 2020 2043 7572 7265 6e74  .        Current
+0000c5a0: 6c79 2c20 6974 2064 6570 656e 6473 206f  ly, it depends o
+0000c5b0: 6e20 7468 6520 6372 6561 7469 6f6e 2069  n the creation i
+0000c5c0: 6e64 6578 2e0a 0a20 2020 2020 2020 203a  ndex...        :
+0000c5d0: 7061 7261 6d20 4469 6d20 6f74 6865 723a  param Dim other:
+0000c5e0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+0000c5f0: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
+0000c600: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+0000c610: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+0000c620: 722c 2028 5f64 2e44 696d 2c20 5f6d 2e4d  r, (_d.Dim, _m.M
+0000c630: 6172 6b65 6444 696d 2929 3a0a 2020 2020  arkedDim)):.    
+0000c640: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+0000c650: 7065 4572 726f 7228 2263 616e 6e6f 7420  peError("cannot 
+0000c660: 636f 6d70 6172 6520 2572 2077 6974 6820  compare %r with 
+0000c670: 2572 2220 2520 2873 656c 662c 206f 7468  %r" % (self, oth
+0000c680: 6572 2929 0a20 2020 2020 2020 2069 6620  er)).        if 
+0000c690: 7365 6c66 203d 3d20 6f74 6865 723a 0a20  self == other:. 
+0000c6a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c6b0: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+0000c6c0: 7265 7475 726e 2064 696d 5f63 6d70 5f76  return dim_cmp_v
+0000c6d0: 616c 7565 2873 656c 6629 203c 2064 696d  alue(self) < dim
+0000c6e0: 5f63 6d70 5f76 616c 7565 286f 7468 6572  _cmp_value(other
+0000c6f0: 290a 0a20 2020 2064 6566 205f 5f67 745f  )..    def __gt_
+0000c700: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+0000c710: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c720: 2020 2020 5365 6520 3a66 756e 633a 605f      See :func:`_
+0000c730: 5f6c 745f 5f60 2e0a 0a20 2020 2020 2020  _lt__`...       
+0000c740: 203a 7061 7261 6d20 4469 6d20 6f74 6865   :param Dim othe
+0000c750: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
+0000c760: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+0000c770: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+0000c780: 726e 206f 7468 6572 203c 2073 656c 660a  rn other < self.
+0000c790: 0a20 2020 2064 6566 205f 5f67 655f 5f28  .    def __ge__(
+0000c7a0: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+0000c7b0: 2020 2020 2020 7265 7475 726e 206e 6f74        return not
+0000c7c0: 2073 656c 6620 3c20 6f74 6865 720a 0a20   self < other.. 
+0000c7d0: 2020 2064 6566 205f 5f6c 655f 5f28 7365     def __le__(se
+0000c7e0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+0000c7f0: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+0000c800: 656c 6620 3e20 6f74 6865 720a 0a20 2020  elf > other..   
+0000c810: 2064 6566 2067 6574 5f73 616d 655f 6261   def get_same_ba
+0000c820: 7365 2873 656c 663a 205f 642e 4469 6d29  se(self: _d.Dim)
+0000c830: 202d 3e20 5f64 2e44 696d 3a0a 2020 2020   -> _d.Dim:.    
+0000c840: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000c850: 3a72 6574 7572 6e3a 2073 616d 6520 6261  :return: same ba
+0000c860: 7365 0a20 2020 2020 2020 2022 2222 0a20  se.        """. 
+0000c870: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000c880: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
+0000c890: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000c8a0: 6c66 0a20 2020 2020 2020 2062 6173 6520  lf.        base 
+0000c8b0: 3d20 7365 6c66 0a20 2020 2020 2020 2077  = self.        w
+0000c8c0: 6869 6c65 2062 6173 652e 7361 6d65 5f61  hile base.same_a
+0000c8d0: 733a 0a20 2020 2020 2020 2020 2020 2062  s:.            b
+0000c8e0: 6173 6520 3d20 6261 7365 2e73 616d 655f  ase = base.same_
+0000c8f0: 6173 0a20 2020 2020 2020 2072 6574 7572  as.        retur
+0000c900: 6e20 6261 7365 0a0a 2020 2020 6465 6620  n base..    def 
+0000c910: 6765 745f 7361 6d65 5f64 6572 6976 6564  get_same_derived
+0000c920: 5f62 6173 6528 7365 6c66 3a20 5f64 2e44  _base(self: _d.D
+0000c930: 696d 2920 2d3e 205f 642e 4469 6d3a 0a20  im) -> _d.Dim:. 
+0000c940: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c950: 2020 203a 7265 7475 726e 3a20 7361 6d65     :return: same
+0000c960: 2062 6173 652c 2062 7574 2061 6c73 6f20   base, but also 
+0000c970: 636f 6e73 6964 6572 2064 6572 6976 6564  consider derived
+0000c980: 5f66 726f 6d5f 2e2e 2e0a 2020 2020 2020  _from_....      
+0000c990: 2020 2222 220a 2020 2020 2020 2020 6261    """.        ba
+0000c9a0: 7365 203d 2073 656c 660a 2020 2020 2020  se = self.      
+0000c9b0: 2020 7669 7369 7465 6420 3d20 7b7d 0a20    visited = {}. 
+0000c9c0: 2020 2020 2020 2077 6869 6c65 2062 6173         while bas
+0000c9d0: 652e 7361 6d65 5f61 7320 6f72 2062 6173  e.same_as or bas
+0000c9e0: 652e 6465 7269 7665 645f 6672 6f6d 5f74  e.derived_from_t
+0000c9f0: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
+0000ca00: 6173 7365 7274 2069 6428 6261 7365 2920  assert id(base) 
+0000ca10: 6e6f 7420 696e 2076 6973 6974 6564 2020  not in visited  
+0000ca20: 2320 7368 6f75 6c64 206e 6f74 2068 6176  # should not hav
+0000ca30: 6520 6379 636c 6573 2e20 6e6f 726d 616c  e cycles. normal
+0000ca40: 6c79 2074 6869 7320 7368 6f75 6c64 206e  ly this should n
+0000ca50: 6576 6572 2062 6520 7472 6967 6765 7265  ever be triggere
+0000ca60: 640a 2020 2020 2020 2020 2020 2020 7669  d.            vi
+0000ca70: 7369 7465 645b 6964 2862 6173 6529 5d20  sited[id(base)] 
+0000ca80: 3d20 6261 7365 0a20 2020 2020 2020 2020  = base.         
+0000ca90: 2020 2069 6620 6261 7365 2e73 616d 655f     if base.same_
+0000caa0: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
+0000cab0: 2020 2020 6261 7365 203d 2062 6173 652e      base = base.
+0000cac0: 7361 6d65 5f61 730a 2020 2020 2020 2020  same_as.        
+0000cad0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000cae0: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+0000caf0: 6520 3d20 6261 7365 2e64 6572 6976 6564  e = base.derived
+0000cb00: 5f66 726f 6d5f 7461 670a 2020 2020 2020  _from_tag.      
+0000cb10: 2020 2020 2020 6173 7365 7274 2062 6173        assert bas
+0000cb20: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+0000cb30: 2062 6173 650a 0a20 2020 2064 6566 2067   base..    def g
+0000cb40: 6574 5f64 6572 6976 6564 5f62 6173 6573  et_derived_bases
+0000cb50: 5f73 6574 2873 656c 6629 3a0a 2020 2020  _set(self):.    
+0000cb60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000cb70: 3a72 7479 7065 3a20 7365 745b 4469 6d5d  :rtype: set[Dim]
+0000cb80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000cb90: 2020 2020 2072 6573 203d 2073 6574 2829       res = set()
+0000cba0: 0a20 2020 2020 2020 2071 7565 7565 203d  .        queue =
+0000cbb0: 205b 7365 6c66 5d0a 2020 2020 2020 2020   [self].        
+0000cbc0: 7669 7369 7465 6420 3d20 7b7d 2020 2320  visited = {}  # 
+0000cbd0: 7479 7065 3a20 4469 6374 5b69 6e74 2c5f  type: Dict[int,_
+0000cbe0: 642e 4469 6d5d 2020 2320 6279 2069 640a  d.Dim]  # by id.
+0000cbf0: 2020 2020 2020 2020 7768 696c 6520 7175          while qu
+0000cc00: 6575 653a 0a20 2020 2020 2020 2020 2020  eue:.           
+0000cc10: 2062 6173 6520 3d20 7175 6575 652e 706f   base = queue.po
+0000cc20: 7028 2d31 290a 2020 2020 2020 2020 2020  p(-1).          
+0000cc30: 2020 6966 2062 6173 652e 7361 6d65 5f61    if base.same_a
+0000cc40: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000cc50: 2020 2062 6173 6520 3d20 6261 7365 2e73     base = base.s
+0000cc60: 616d 655f 6173 0a20 2020 2020 2020 2020  ame_as.         
+0000cc70: 2020 2069 6620 6964 2862 6173 6529 2069     if id(base) i
+0000cc80: 6e20 7669 7369 7465 643a 0a20 2020 2020  n visited:.     
+0000cc90: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0000cca0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+0000ccb0: 7669 7369 7465 645b 6964 2862 6173 6529  visited[id(base)
+0000ccc0: 5d20 3d20 6261 7365 0a20 2020 2020 2020  ] = base.       
+0000ccd0: 2020 2020 2072 6573 2e61 6464 2862 6173       res.add(bas
+0000cce0: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+0000ccf0: 6620 6261 7365 2e64 6572 6976 6564 5f66  f base.derived_f
+0000cd00: 726f 6d5f 6f70 3a0a 2020 2020 2020 2020  rom_op:.        
+0000cd10: 2020 2020 2020 2020 7175 6575 652e 6578          queue.ex
+0000cd20: 7465 6e64 2862 6173 652e 6465 7269 7665  tend(base.derive
+0000cd30: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
+0000cd40: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000cd50: 6966 2062 6173 652e 6465 7269 7665 645f  if base.derived_
+0000cd60: 6672 6f6d 5f74 6167 3a0a 2020 2020 2020  from_tag:.      
+0000cd70: 2020 2020 2020 2020 2020 7175 6575 652e            queue.
+0000cd80: 6170 7065 6e64 2862 6173 652e 6465 7269  append(base.deri
+0000cd90: 7665 645f 6672 6f6d 5f74 6167 290a 2020  ved_from_tag).  
+0000cda0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0000cdb0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000cdc0: 2020 2020 6465 6620 756e 6465 6669 6e65      def undefine
+0000cdd0: 6428 7365 6c66 3a20 5f64 2e44 696d 2920  d(self: _d.Dim) 
+0000cde0: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+0000cdf0: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
+0000ce00: 7475 726e 3a20 7768 6574 6865 7220 7468  turn: whether th
+0000ce10: 6520 756e 6465 6669 6e65 6420 666c 6167  e undefined flag
+0000ce20: 2069 7320 7365 742c 2069 6e20 7365 6c66   is set, in self
+0000ce30: 2c20 6261 7365 732c 206f 7220 616e 7920  , bases, or any 
+0000ce40: 6465 7269 7665 6420 6261 7365 732e 2061  derived bases. a
+0000ce50: 6c73 6f20 7365 6520 3a66 756e 633a 6069  lso see :func:`i
+0000ce60: 735f 6469 6d5f 6b6e 6f77 6e60 0a20 2020  s_dim_known`.   
+0000ce70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ce80: 2062 6173 6520 3d20 7365 6c66 0a20 2020   base = self.   
+0000ce90: 2020 2020 2076 6973 6974 6564 203d 207b       visited = {
+0000cea0: 7d0a 2020 2020 2020 2020 7768 696c 6520  }.        while 
+0000ceb0: 6261 7365 2e73 616d 655f 6173 206f 7220  base.same_as or 
+0000cec0: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000ced0: 6d5f 7461 673a 0a20 2020 2020 2020 2020  m_tag:.         
+0000cee0: 2020 2061 7373 6572 7420 6964 2862 6173     assert id(bas
+0000cef0: 6529 206e 6f74 2069 6e20 7669 7369 7465  e) not in visite
+0000cf00: 6420 2023 2073 686f 756c 6420 6e6f 7420  d  # should not 
+0000cf10: 6861 7665 2063 7963 6c65 732e 206e 6f72  have cycles. nor
+0000cf20: 6d61 6c6c 7920 7468 6973 2073 686f 756c  mally this shoul
+0000cf30: 6420 6e65 7665 7220 6265 2074 7269 6767  d never be trigg
+0000cf40: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
+0000cf50: 2076 6973 6974 6564 5b69 6428 6261 7365   visited[id(base
+0000cf60: 295d 203d 2062 6173 650a 2020 2020 2020  )] = base.      
+0000cf70: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
+0000cf80: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
+0000cf90: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
+0000cfa0: 2020 2069 6620 6261 7365 2e5f 6578 7472     if base._extr
+0000cfb0: 6120 616e 6420 6261 7365 2e5f 6578 7472  a and base._extr
+0000cfc0: 612e 756e 6465 6669 6e65 643a 0a20 2020  a.undefined:.   
+0000cfd0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000cfe0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+0000cff0: 2020 2020 2069 6620 6261 7365 2e73 616d       if base.sam
+0000d000: 655f 6173 3a0a 2020 2020 2020 2020 2020  e_as:.          
+0000d010: 2020 2020 2020 6261 7365 203d 2062 6173        base = bas
+0000d020: 652e 7361 6d65 5f61 730a 2020 2020 2020  e.same_as.      
+0000d030: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+0000d040: 7565 0a20 2020 2020 2020 2020 2020 2062  ue.            b
+0000d050: 6173 6520 3d20 6261 7365 2e64 6572 6976  ase = base.deriv
+0000d060: 6564 5f66 726f 6d5f 7461 670a 2020 2020  ed_from_tag.    
+0000d070: 2020 2020 2020 2020 6173 7365 7274 2062          assert b
+0000d080: 6173 650a 2020 2020 2020 2020 2320 6e6f  ase.        # no
+0000d090: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
+0000d0a0: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
+0000d0b0: 2020 2020 2072 6574 7572 6e20 6261 7365       return base
+0000d0c0: 2e5f 6578 7472 6120 616e 6420 6261 7365  ._extra and base
+0000d0d0: 2e5f 6578 7472 612e 756e 6465 6669 6e65  ._extra.undefine
+0000d0e0: 640a 0a20 2020 2064 6566 2064 6563 6c61  d..    def decla
+0000d0f0: 7265 5f73 616d 655f 6173 2873 656c 663a  re_same_as(self:
+0000d100: 205f 642e 4469 6d2c 206f 7468 6572 3a20   _d.Dim, other: 
+0000d110: 5f64 2e44 696d 293a 0a20 2020 2020 2020  _d.Dim):.       
+0000d120: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+0000d130: 7261 6d20 6f74 6865 723a 0a20 2020 2020  ram other:.     
+0000d140: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+0000d150: 7373 6572 7420 7365 6c66 2e63 616e 5f62  ssert self.can_b
+0000d160: 655f 7573 6564 5f61 735f 6469 6d28 2920  e_used_as_dim() 
+0000d170: 616e 6420 6f74 6865 722e 6361 6e5f 6265  and other.can_be
+0000d180: 5f75 7365 645f 6173 5f64 696d 2829 2020  _used_as_dim()  
+0000d190: 2320 6465 636c 6172 655f 7361 6d65 5f61  # declare_same_a
+0000d1a0: 7320 646f 6573 206e 6f74 206d 616b 6520  s does not make 
+0000d1b0: 7365 6e73 6520 6f74 6865 7277 6973 650a  sense otherwise.
+0000d1c0: 2020 2020 2020 2020 2320 4e6f 7465 3a20          # Note: 
+0000d1d0: 4368 6563 6b20 6069 7360 2c20 6e6f 7420  Check `is`, not 
+0000d1e0: 603d 3d60 2e20 603d 3d60 2063 616e 2062  `==`. `==` can b
+0000d1f0: 6520 7472 7565 2065 7665 6e20 7468 6f75  e true even thou
+0000d200: 6768 2073 616d 655f 6173 2061 7265 206e  gh same_as are n
+0000d210: 6f74 2074 6865 2073 616d 6520 696e 7374  ot the same inst
+0000d220: 616e 6365 2c0a 2020 2020 2020 2020 2320  ance,.        # 
+0000d230: 652e 672e 2076 6961 2061 7574 6f5f 6765  e.g. via auto_ge
+0000d240: 6e65 7261 7465 642e 0a20 2020 2020 2020  nerated..       
+0000d250: 2069 6620 7365 6c66 2069 7320 6f74 6865   if self is othe
+0000d260: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+0000d270: 6574 7572 6e0a 2020 2020 2020 2020 7365  eturn.        se
+0000d280: 6c66 2e5f 6d61 7962 655f 7570 6461 7465  lf._maybe_update
+0000d290: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000d2a0: 5f76 616c 6964 6174 655f 696e 5f63 7572  _validate_in_cur
+0000d2b0: 7265 6e74 5f67 7261 7068 2829 0a20 2020  rent_graph().   
+0000d2c0: 2020 2020 206f 7468 6572 2e5f 7661 6c69       other._vali
+0000d2d0: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
+0000d2e0: 6772 6170 6828 290a 2020 2020 2020 2020  graph().        
+0000d2f0: 6f74 6865 725f 7361 6d65 5f62 6173 6520  other_same_base 
+0000d300: 3d20 6f74 6865 722e 6765 745f 7361 6d65  = other.get_same
+0000d310: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
+0000d320: 6966 2073 656c 6620 6973 206f 7468 6572  if self is other
+0000d330: 5f73 616d 655f 6261 7365 206f 7220 7365  _same_base or se
+0000d340: 6c66 2e73 616d 655f 6173 2069 7320 6f74  lf.same_as is ot
+0000d350: 6865 725f 7361 6d65 5f62 6173 653a 0a20  her_same_base:. 
+0000d360: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000d370: 6e0a 2020 2020 2020 2020 7365 6c66 5f73  n.        self_s
+0000d380: 616d 655f 6173 203d 2073 656c 662e 6765  ame_as = self.ge
+0000d390: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
+0000d3a0: 2020 2020 2020 6966 2073 656c 665f 7361        if self_sa
+0000d3b0: 6d65 5f61 7320 6973 206f 7468 6572 5f73  me_as is other_s
+0000d3c0: 616d 655f 6261 7365 3a0a 2020 2020 2020  ame_base:.      
+0000d3d0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000d3e0: 2020 2020 2069 6620 6f74 6865 725f 7361       if other_sa
+0000d3f0: 6d65 5f62 6173 652e 6765 745f 7361 6d65  me_base.get_same
+0000d400: 5f64 6572 6976 6564 5f62 6173 6528 2920  _derived_base() 
+0000d410: 6973 2073 656c 665f 7361 6d65 5f61 733a  is self_same_as:
+0000d420: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
+0000d430: 6520 6163 7475 616c 6c79 2077 616e 7420  e actually want 
+0000d440: 6974 2074 6f20 6265 2074 6865 206f 7468  it to be the oth
+0000d450: 6572 2077 6179 2061 726f 756e 642e 0a20  er way around.. 
+0000d460: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0000d470: 7574 696c 2e67 7561 7264 5f69 6e66 696e  util.guard_infin
+0000d480: 6974 655f 7265 6375 7273 696f 6e28 5f64  ite_recursion(_d
+0000d490: 2e44 696d 2e64 6563 6c61 7265 5f73 616d  .Dim.declare_sam
+0000d4a0: 655f 6173 2c20 6f74 6865 722c 2073 656c  e_as, other, sel
+0000d4b0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
+0000d4c0: 2020 2020 7265 7475 726e 206f 7468 6572      return other
+0000d4d0: 2e64 6563 6c61 7265 5f73 616d 655f 6173  .declare_same_as
+0000d4e0: 2873 656c 6629 0a20 2020 2020 2020 2069  (self).        i
+0000d4f0: 6620 7365 6c66 2e62 6174 6368 3a0a 2020  f self.batch:.  
+0000d500: 2020 2020 2020 2020 2020 2320 4966 2073            # If s
+0000d510: 656c 6620 6973 2064 6566 696e 6564 2028  elf is defined (
+0000d520: 7365 6c66 2e69 735f 6469 6d5f 6b6e 6f77  self.is_dim_know
+0000d530: 6e29 2c20 6265 2066 6169 7220 746f 206f  n), be fair to o
+0000d540: 7468 6572 2c20 616e 6420 6164 6170 7420  ther, and adapt 
+0000d550: 6974 2074 6f20 7468 6520 7269 6768 7420  it to the right 
+0000d560: 6261 7463 682c 0a20 2020 2020 2020 2020  batch,.         
+0000d570: 2020 2023 2073 7563 6820 7468 6174 206f     # such that o
+0000d580: 7468 6572 2e69 735f 6469 6d5f 6b6e 6f77  ther.is_dim_know
+0000d590: 6e20 6973 2063 6f72 7265 6374 2c20 6279  n is correct, by
+0000d5a0: 2070 6f74 656e 7469 616c 6c79 2063 6f6d   potentially com
+0000d5b0: 706c 6574 696e 6720 6974 2e0a 2020 2020  pleting it..    
+0000d5c0: 2020 2020 2020 2020 6f74 6865 725f 203d          other_ =
+0000d5d0: 206f 7468 6572 2e67 6574 5f66 6f72 5f62   other.get_for_b
+0000d5e0: 6174 6368 5f63 7478 2873 656c 662e 6261  atch_ctx(self.ba
+0000d5f0: 7463 682c 2063 7478 3d73 656c 662e 636f  tch, ctx=self.co
+0000d600: 6e74 726f 6c5f 666c 6f77 5f63 7478 290a  ntrol_flow_ctx).
+0000d610: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000d620: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
+0000d630: 203d 206f 7468 6572 0a20 2020 2020 2020   = other.       
+0000d640: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
+0000d650: 2020 2873 656c 662e 6973 5f64 696d 5f6b    (self.is_dim_k
+0000d660: 6e6f 776e 2829 2061 6e64 206e 6f74 206f  nown() and not o
+0000d670: 7468 6572 5f2e 6973 5f64 696d 5f6b 6e6f  ther_.is_dim_kno
+0000d680: 776e 2829 290a 2020 2020 2020 2020 2020  wn()).          
+0000d690: 2020 6f72 0a20 2020 2020 2020 2020 2020    or.           
+0000d6a0: 2023 204c 696b 6520 6973 5f64 696d 5f6b   # Like is_dim_k
+0000d6b0: 6e6f 776e 2062 7574 2066 6f72 2073 7461  nown but for sta
+0000d6c0: 7469 6320 6469 6d73 2c20 7765 206d 6967  tic dims, we mig
+0000d6d0: 6874 206b 6e6f 7720 626f 7468 2c0a 2020  ht know both,.  
+0000d6e0: 2020 2020 2020 2020 2020 2320 6275 7420            # but 
+0000d6f0: 7468 6520 6465 7269 7665 645f 6672 6f6d  the derived_from
+0000d700: 5f6f 7020 7374 696c 6c20 776f 756c 6420  _op still would 
+0000d710: 7072 6f76 6964 6520 6d6f 7265 2069 6e66  provide more inf
+0000d720: 6f72 6d61 7469 6f6e 2e0a 2020 2020 2020  ormation..      
+0000d730: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+0000d740: 2020 2020 2020 2020 7365 6c66 5f73 616d          self_sam
+0000d750: 655f 6173 2e64 6572 6976 6564 5f66 726f  e_as.derived_fro
+0000d760: 6d5f 6f70 0a20 2020 2020 2020 2020 2020  m_op.           
+0000d770: 2020 2020 2061 6e64 206e 6f74 206f 7468       and not oth
+0000d780: 6572 5f73 616d 655f 6261 7365 2e64 6572  er_same_base.der
+0000d790: 6976 6564 5f66 726f 6d5f 6f70 0a20 2020  ived_from_op.   
+0000d7a0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+0000d7b0: 206f 7468 6572 206e 6f74 2069 6e20 7365   other not in se
+0000d7c0: 6c66 2e67 6574 5f64 6572 6976 6564 5f62  lf.get_derived_b
+0000d7d0: 6173 6573 5f73 6574 2829 0a20 2020 2020  ases_set().     
+0000d7e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000d7f0: 2020 2020 206f 7220 286e 6f74 2073 656c       or (not sel
+0000d800: 662e 756e 6465 6669 6e65 6420 616e 6420  f.undefined and 
+0000d810: 6f74 6865 725f 2e75 6e64 6566 696e 6564  other_.undefined
+0000d820: 290a 2020 2020 2020 2020 293a 0a20 2020  ).        ):.   
+0000d830: 2020 2020 2020 2020 2077 6974 6820 7574           with ut
+0000d840: 696c 2e67 7561 7264 5f69 6e66 696e 6974  il.guard_infinit
+0000d850: 655f 7265 6375 7273 696f 6e28 5f64 2e44  e_recursion(_d.D
+0000d860: 696d 2e64 6563 6c61 7265 5f73 616d 655f  im.declare_same_
+0000d870: 6173 2c20 6f74 6865 722c 2073 656c 6629  as, other, self)
+0000d880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d890: 2020 7265 7475 726e 206f 7468 6572 2e64    return other.d
+0000d8a0: 6563 6c61 7265 5f73 616d 655f 6173 2873  eclare_same_as(s
+0000d8b0: 656c 6629 0a20 2020 2020 2020 206f 7468  elf).        oth
+0000d8c0: 6572 5f64 6572 6976 6564 5f62 6173 6573  er_derived_bases
+0000d8d0: 203d 206f 7468 6572 2e67 6574 5f64 6572   = other.get_der
+0000d8e0: 6976 6564 5f62 6173 6573 5f73 6574 2829  ived_bases_set()
+0000d8f0: 0a20 2020 2020 2020 2073 656c 665f 6465  .        self_de
+0000d900: 7269 7665 645f 6261 7365 7320 3d20 7365  rived_bases = se
+0000d910: 6c66 2e67 6574 5f64 6572 6976 6564 5f62  lf.get_derived_b
+0000d920: 6173 6573 5f73 6574 2829 0a20 2020 2020  ases_set().     
+0000d930: 2020 2069 6620 6f74 6865 725f 6465 7269     if other_deri
+0000d940: 7665 645f 6261 7365 7320 213d 2073 656c  ved_bases != sel
+0000d950: 665f 6465 7269 7665 645f 6261 7365 7320  f_derived_bases 
+0000d960: 616e 6420 7365 6c66 5f64 6572 6976 6564  and self_derived
+0000d970: 5f62 6173 6573 2e69 7373 7562 7365 7428  _bases.issubset(
+0000d980: 6f74 6865 725f 6465 7269 7665 645f 6261  other_derived_ba
+0000d990: 7365 7329 3a0a 2020 2020 2020 2020 2020  ses):.          
+0000d9a0: 2020 2320 4176 6f69 6420 6379 636c 6573    # Avoid cycles
+0000d9b0: 206f 6e20 6465 7269 7665 645f 6672 6f6d   on derived_from
+0000d9c0: 5f74 6167 2e20 6874 7470 733a 2f2f 6769  _tag. https://gi
+0000d9d0: 7468 7562 2e63 6f6d 2f72 7774 682d 6936  thub.com/rwth-i6
+0000d9e0: 2f72 6574 7572 6e6e 2f69 7373 7565 732f  /returnn/issues/
+0000d9f0: 3130 3534 0a20 2020 2020 2020 2020 2020  1054.           
+0000da00: 2077 6974 6820 7574 696c 2e67 7561 7264   with util.guard
+0000da10: 5f69 6e66 696e 6974 655f 7265 6375 7273  _infinite_recurs
+0000da20: 696f 6e28 5f64 2e44 696d 2e64 6563 6c61  ion(_d.Dim.decla
+0000da30: 7265 5f73 616d 655f 6173 2c20 6f74 6865  re_same_as, othe
+0000da40: 722c 2073 656c 6629 3a0a 2020 2020 2020  r, self):.      
+0000da50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000da60: 206f 7468 6572 2e64 6563 6c61 7265 5f73   other.declare_s
+0000da70: 616d 655f 6173 2873 656c 6629 0a20 2020  ame_as(self).   
+0000da80: 2020 2020 2069 6620 7365 6c66 2e5f 6578       if self._ex
+0000da90: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
+0000daa0: 2073 656c 662e 5f65 7874 7261 2e64 6572   self._extra.der
+0000dab0: 6976 6564 5f66 726f 6d5f 6f70 203d 204e  ived_from_op = N
+0000dac0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000dad0: 7365 6c66 2e5f 6578 7472 612e 6465 7269  self._extra.deri
+0000dae0: 7665 645f 6672 6f6d 5f74 6167 203d 204e  ved_from_tag = N
+0000daf0: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
+0000db00: 656c 665f 7361 6d65 5f61 7320 6973 206e  elf_same_as is n
+0000db10: 6f74 2073 656c 663a 0a20 2020 2020 2020  ot self:.       
+0000db20: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
+0000db30: 7365 6c66 5f73 616d 655f 6173 2e73 616d  self_same_as.sam
+0000db40: 655f 6173 0a20 2020 2020 2020 2020 2020  e_as.           
+0000db50: 2069 6620 7365 6c66 5f73 616d 655f 6173   if self_same_as
+0000db60: 2069 7320 6f74 6865 725f 7361 6d65 5f62   is other_same_b
+0000db70: 6173 653a 0a20 2020 2020 2020 2020 2020  ase:.           
+0000db80: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000db90: 2020 2020 2020 2020 7769 7468 2075 7469          with uti
+0000dba0: 6c2e 6775 6172 645f 696e 6669 6e69 7465  l.guard_infinite
+0000dbb0: 5f72 6563 7572 7369 6f6e 285f 642e 4469  _recursion(_d.Di
+0000dbc0: 6d2e 6465 636c 6172 655f 7361 6d65 5f61  m.declare_same_a
+0000dbd0: 732c 2073 656c 665f 7361 6d65 5f61 732c  s, self_same_as,
+0000dbe0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000dbf0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000dc00: 2020 2073 656c 665f 7361 6d65 5f61 732e     self_same_as.
+0000dc10: 6465 636c 6172 655f 7361 6d65 5f61 7328  declare_same_as(
+0000dc20: 6f74 6865 725f 7361 6d65 5f62 6173 6529  other_same_base)
+0000dc30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000dc40: 2873 656c 662e 6479 6e5f 7369 7a65 5f65  (self.dyn_size_e
+0000dc50: 7874 2069 7320 4e6f 6e65 206f 7220 6e6f  xt is None or no
+0000dc60: 7420 7365 6c66 2e5f 7661 6c69 6461 7465  t self._validate
+0000dc70: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
+0000dc80: 6828 2929 2061 6e64 2073 656c 665f 7361  h()) and self_sa
+0000dc90: 6d65 5f61 732e 6479 6e5f 7369 7a65 5f65  me_as.dyn_size_e
+0000dca0: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+0000dcb0: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
+0000dcc0: 655f 6578 7420 3d20 7365 6c66 5f73 616d  e_ext = self_sam
+0000dcd0: 655f 6173 2e67 6574 5f64 796e 5f73 697a  e_as.get_dyn_siz
+0000dce0: 655f 6578 745f 666f 725f 6261 7463 685f  e_ext_for_batch_
+0000dcf0: 6374 7828 0a20 2020 2020 2020 2020 2020  ctx(.           
+0000dd00: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
+0000dd10: 7463 682c 2073 656c 662e 636f 6e74 726f  tch, self.contro
+0000dd20: 6c5f 666c 6f77 5f63 7478 2c20 7465 6d70  l_flow_ctx, temp
+0000dd30: 6c61 7465 5f6f 6e6c 793d 5472 7565 0a20  late_only=True. 
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000dd50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000dd60: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000dd70: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
+0000dd80: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
+0000dd90: 696d 5f20 696e 2073 656c 662e 5f65 7874  im_ in self._ext
+0000dda0: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
+0000ddb0: 685f 6374 782e 7661 6c75 6573 2829 3a0a  h_ctx.values():.
+0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddd0: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+0000dde0: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+0000ddf0: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+0000de00: 2020 2020 2020 2020 2069 6620 6469 6d5f           if dim_
+0000de10: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
 0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de30: 2020 2023 206e 6f69 6e73 7065 6374 696f     # noinspectio
-0000de40: 6e20 5079 5072 6f74 6563 7465 644d 656d  n PyProtectedMem
-0000de50: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
-0000de60: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
-0000de70: 2e5f 6578 7472 612e 6465 7269 7665 645f  ._extra.derived_
-0000de80: 6672 6f6d 5f74 6167 203d 204e 6f6e 650a  from_tag = None.
-0000de90: 2020 2020 2020 2020 2320 4e6f 7720 6d65          # Now me
-0000dea0: 7267 6520 6578 6973 7469 6e67 2076 6172  rge existing var
-0000deb0: 6961 6e74 732e 2042 7574 206f 6e6c 7920  iants. But only 
-0000dec0: 6966 206e 6f74 2064 6572 6976 6564 2076  if not derived v
-0000ded0: 6961 206f 702c 2062 6563 6175 7365 2069  ia op, because i
-0000dee0: 6e20 7468 6174 2063 6173 652c 2077 6520  n that case, we 
-0000def0: 6361 6e20 2861 6e64 2073 686f 756c 6421  can (and should!
-0000df00: 290a 2020 2020 2020 2020 2320 6175 746f  ).        # auto
-0000df10: 6d61 7469 6361 6c6c 7920 696e 6665 7220  matically infer 
-0000df20: 6974 2e20 4e6f 7465 2074 6861 7420 7765  it. Note that we
-0000df30: 206f 6e6c 7920 676f 7420 6865 7265 2077   only got here w
-0000df40: 6865 6e20 7468 6520 6f74 6865 7220 6973  hen the other is
-0000df50: 206e 6f74 2074 6865 2073 616d 6520 6469   not the same di
-0000df60: 6d2c 2073 6f20 6974 206d 6561 6e73 2074  m, so it means t
-0000df70: 6861 740a 2020 2020 2020 2020 2320 7468  hat.        # th
-0000df80: 6520 6f74 6865 7220 6973 2072 6561 6c6c  e other is reall
-0000df90: 7920 6469 6666 6572 656e 742c 2074 6865  y different, the
-0000dfa0: 2073 697a 6573 2061 7265 2070 6f74 656e   sizes are poten
-0000dfb0: 7469 616c 6c79 2064 6966 6665 7265 6e74  tially different
-0000dfc0: 2c20 6275 7420 7765 2077 616e 7420 746f  , but we want to
-0000dfd0: 206f 7665 7274 616b 6520 7468 6520 6f74   overtake the ot
-0000dfe0: 6865 722e 0a20 2020 2020 2020 2069 6620  her..        if 
-0000dff0: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
-0000e000: 6465 7269 7665 645f 6672 6f6d 5f6f 703a  derived_from_op:
-0000e010: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-0000e020: 6c65 616e 7570 2065 7665 7279 7468 696e  leanup everythin
-0000e030: 672c 2065 7370 2070 6f74 656e 7469 616c  g, esp potential
-0000e040: 2061 6c72 6561 6479 2063 6f6d 7075 7465   already compute
-0000e050: 6420 7369 7a65 732c 2061 7320 7468 6573  d sizes, as thes
-0000e060: 6520 6d69 6768 7420 6265 2069 6e76 616c  e might be inval
-0000e070: 6964 2e0a 2020 2020 2020 2020 2020 2020  id..            
-0000e080: 666f 7220 6469 6d5f 2069 6e20 5b73 656c  for dim_ in [sel
-0000e090: 665f 7361 6d65 5f61 732c 2073 656c 665d  f_same_as, self]
-0000e0a0: 202b 2028 6c69 7374 2873 656c 662e 5f65   + (list(self._e
-0000e0b0: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
-0000e0c0: 7463 685f 6374 782e 7661 6c75 6573 2829  tch_ctx.values()
-0000e0d0: 2920 6966 2073 656c 662e 5f65 7874 7261  ) if self._extra
-0000e0e0: 2065 6c73 6520 5b5d 293a 0a20 2020 2020   else []):.     
-0000e0f0: 2020 2020 2020 2020 2020 2069 6620 6469             if di
-0000e100: 6d5f 2e64 796e 5f73 697a 655f 6578 743a  m_.dyn_size_ext:
-0000e110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e120: 2020 2020 2064 696d 5f2e 6479 6e5f 7369       dim_.dyn_si
-0000e130: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
-0000e140: 6572 203d 204e 6f6e 650a 2020 2020 2020  er = None.      
-0000e150: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
-0000e160: 652e 5f6d 6572 6765 5f73 616d 655f 666f  e._merge_same_fo
-0000e170: 725f 6261 7463 685f 6374 785f 6469 6374  r_batch_ctx_dict
-0000e180: 2873 656c 6629 0a20 2020 2020 2020 206f  (self).        o
-0000e190: 7468 6572 2e5f 6d61 7962 655f 7570 6461  ther._maybe_upda
-0000e1a0: 7465 2829 0a20 2020 2020 2020 2073 656c  te().        sel
-0000e1b0: 662e 7361 6d65 5f61 7320 3d20 6f74 6865  f.same_as = othe
-0000e1c0: 725f 7361 6d65 5f62 6173 650a 2020 2020  r_same_base.    
-0000e1d0: 2020 2020 7365 6c66 2e5f 6d61 7962 655f      self._maybe_
-0000e1e0: 7570 6461 7465 2829 0a20 2020 2020 2020  update().       
-0000e1f0: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
-0000e200: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
-0000e210: 6420 6f74 6865 725f 7361 6d65 5f62 6173  d other_same_bas
-0000e220: 652e 6479 6e5f 7369 7a65 2069 7320 6e6f  e.dyn_size is no
-0000e230: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000e240: 2020 2020 6966 2073 656c 662e 6479 6e5f      if self.dyn_
-0000e250: 7369 7a65 2069 7320 6e6f 7420 6f74 6865  size is not othe
-0000e260: 725f 7361 6d65 5f62 6173 652e 6479 6e5f  r_same_base.dyn_
-0000e270: 7369 7a65 3a0a 2020 2020 2020 2020 2020  size:.          
-0000e280: 2020 2020 2020 6966 2073 656c 662e 6261        if self.ba
-0000e290: 7463 6820 3d3d 206f 7468 6572 5f73 616d  tch == other_sam
-0000e2a0: 655f 6261 7365 2e62 6174 6368 2061 6e64  e_base.batch and
-0000e2b0: 2073 656c 662e 636f 6e74 726f 6c5f 666c   self.control_fl
-0000e2c0: 6f77 5f63 7478 203d 3d20 6f74 6865 725f  ow_ctx == other_
-0000e2d0: 7361 6d65 5f62 6173 652e 636f 6e74 726f  same_base.contro
-0000e2e0: 6c5f 666c 6f77 5f63 7478 3a0a 2020 2020  l_flow_ctx:.    
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e300: 2320 4e6f 7465 3a20 496e 7374 6561 6420  # Note: Instead 
-0000e310: 6f66 206d 616b 696e 6720 7468 6973 2061  of making this a
-0000e320: 2077 6172 6e69 6e67 2c20 7765 2063 6f75   warning, we cou
-0000e330: 6c64 2061 6c73 6f20 656e 666f 7263 6520  ld also enforce 
-0000e340: 7468 6973 2061 7420 736f 6d65 2070 6f69  this at some poi
-0000e350: 6e74 2e0a 2020 2020 2020 2020 2020 2020  nt..            
-0000e360: 2020 2020 2020 2020 2320 2020 5468 6520          #   The 
-0000e370: 7573 6572 2073 686f 756c 6420 6265 2061  user should be a
-0000e380: 626c 6520 746f 2066 6978 2060 6578 7465  ble to fix `exte
-0000e390: 726e 5f64 6174 6160 2069 6e20 7468 6520  rn_data` in the 
-0000e3a0: 636f 6e66 6967 0a20 2020 2020 2020 2020  config.         
-0000e3b0: 2020 2020 2020 2020 2020 2023 2020 2073             #   s
-0000e3c0: 7563 6820 7468 6174 2074 6869 7320 6973  uch that this is
-0000e3d0: 2063 6f72 7265 6374 2069 6e20 7468 6520   correct in the 
-0000e3e0: 6669 7273 7420 706c 6163 652e 0a20 2020  first place..   
-0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e400: 2023 2020 2041 6c73 6f2c 2069 6e20 6164   #   Also, in ad
-0000e410: 6469 7469 6f6e 2074 6f20 7468 6973 2077  dition to this w
-0000e420: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
-0000e430: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0000e440: 7765 206d 6967 6874 2077 616e 7420 746f  we might want to
-0000e450: 2061 6464 2073 6f6d 6520 7275 6e74 696d   add some runtim
-0000e460: 6520 6368 6563 6b20 6f6e 2074 6865 2065  e check on the e
-0000e470: 7120 6f66 2074 6865 2064 796e 2073 697a  q of the dyn siz
-0000e480: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-0000e490: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
-0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4b0: 2020 2020 2020 2022 5761 726e 696e 673a         "Warning:
-0000e4c0: 2061 7373 756d 696e 6720 6469 6d20 7461   assuming dim ta
-0000e4d0: 6773 2061 7265 2073 616d 6520 7769 7468  gs are same with
-0000e4e0: 2064 6966 6665 7265 6e74 2073 697a 6520   different size 
-0000e4f0: 706c 6163 6568 6f6c 6465 7273 3a20 2572  placeholders: %r
-0000e500: 2076 7320 2572 220a 2020 2020 2020 2020   vs %r".        
-0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e520: 2520 2873 656c 662e 6479 6e5f 7369 7a65  % (self.dyn_size
-0000e530: 2c20 6f74 6865 725f 7361 6d65 5f62 6173  , other_same_bas
-0000e540: 652e 6479 6e5f 7369 7a65 290a 2020 2020  e.dyn_size).    
-0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e560: 290a 2020 2020 2020 2020 2320 4966 2077  ).        # If w
-0000e570: 6520 6861 7665 2061 2064 6566 696e 6564  e have a defined
-0000e580: 2073 6f75 7263 652c 2061 6e64 2074 6869   source, and thi
-0000e590: 7320 6973 2061 2064 796e 616d 6963 2073  s is a dynamic s
-0000e5a0: 7061 7469 616c 2061 7869 732c 2061 6e64  patial axis, and
-0000e5b0: 2069 7420 7761 7320 756e 6465 6669 6e65   it was undefine
-0000e5c0: 6420 6265 666f 7265 2c0a 2020 2020 2020  d before,.      
-0000e5d0: 2020 2320 6d61 7962 6520 7765 2063 616e    # maybe we can
-0000e5e0: 206f 7665 7274 616b 6520 7468 6520 7369   overtake the si
-0000e5f0: 7a65 5f70 6c61 6365 686f 6c64 6572 206e  ze_placeholder n
-0000e600: 6f77 2e0a 2020 2020 2020 2020 6966 206f  ow..        if o
-0000e610: 7468 6572 5f73 616d 655f 6261 7365 2e64  ther_same_base.d
-0000e620: 796e 5f73 697a 6520 6973 206e 6f74 204e  yn_size is not N
-0000e630: 6f6e 6520 616e 6420 7365 6c66 2e5f 6578  one and self._ex
-0000e640: 7472 6120 616e 6420 7365 6c66 2e5f 6578  tra and self._ex
-0000e650: 7472 612e 7372 635f 6461 7461 3a0a 2020  tra.src_data:.  
-0000e660: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000e670: 2069 7369 6e73 7461 6e63 6528 7365 6c66   isinstance(self
-0000e680: 2e5f 6578 7472 612e 7372 635f 6178 6973  ._extra.src_axis
-0000e690: 2c20 696e 7429 0a20 2020 2020 2020 2020  , int).         
-0000e6a0: 2020 2023 204d 6179 6265 2069 7420 6368     # Maybe it ch
-0000e6b0: 616e 6765 6420 696e 2074 6865 206d 6561  anged in the mea
-0000e6c0: 6e77 6869 6c65 2c20 736f 2063 6865 636b  nwhile, so check
-0000e6d0: 2e0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
-0000e6e0: 6720 3d20 7365 6c66 2e5f 6578 7472 612e  g = self._extra.
-0000e6f0: 7372 635f 6461 7461 2e67 6574 5f64 696d  src_data.get_dim
-0000e700: 5f74 6167 2873 656c 662e 5f65 7874 7261  _tag(self._extra
-0000e710: 2e73 7263 5f61 7869 7329 0a20 2020 2020  .src_axis).     
-0000e720: 2020 2020 2020 2069 6620 7461 672e 6465         if tag.de
-0000e730: 7363 7269 7074 696f 6e20 3d3d 2073 656c  scription == sel
-0000e740: 662e 6465 7363 7269 7074 696f 6e20 616e  f.description an
-0000e750: 6420 286e 6f74 2074 6167 2e64 796e 5f73  d (not tag.dyn_s
-0000e760: 697a 655f 6578 7420 6f72 206e 6f74 2074  ize_ext or not t
-0000e770: 6167 2e5f 7661 6c69 6461 7465 5f69 6e5f  ag._validate_in_
-0000e780: 6375 7272 656e 745f 6772 6170 6828 2929  current_graph())
-0000e790: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e7a0: 2020 7461 672e 6479 6e5f 7369 7a65 5f65    tag.dyn_size_e
-0000e7b0: 7874 203d 2073 656c 662e 6765 745f 6479  xt = self.get_dy
-0000e7c0: 6e5f 7369 7a65 5f65 7874 5f66 6f72 5f62  n_size_ext_for_b
-0000e7d0: 6174 6368 5f63 7478 280a 2020 2020 2020  atch_ctx(.      
-0000e7e0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0000e7f0: 672e 6261 7463 682c 2074 6167 2e63 6f6e  g.batch, tag.con
-0000e800: 7472 6f6c 5f66 6c6f 775f 6374 782c 2074  trol_flow_ctx, t
-0000e810: 656d 706c 6174 655f 6f6e 6c79 3d54 7275  emplate_only=Tru
-0000e820: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000e830: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000e840: 2020 2020 7461 672e 5f6d 6179 6265 5f75      tag._maybe_u
-0000e850: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
-0000e860: 2320 4966 206f 7468 6572 7320 6479 6e5f  # If others dyn_
-0000e870: 7369 7a65 2069 7320 4e6f 6e65 2062 7574  size is None but
-0000e880: 2077 6520 6861 7665 2061 2064 796e 5f73   we have a dyn_s
-0000e890: 697a 652c 206d 6179 6265 2075 7064 6174  ize, maybe updat
-0000e8a0: 6520 6f74 6865 7273 2064 796e 5f73 697a  e others dyn_siz
-0000e8b0: 652e 0a20 2020 2020 2020 2069 6620 7365  e..        if se
-0000e8c0: 6c66 2e64 796e 5f73 697a 6520 6973 206e  lf.dyn_size is n
-0000e8d0: 6f74 204e 6f6e 6520 616e 6420 6f74 6865  ot None and othe
-0000e8e0: 725f 7361 6d65 5f62 6173 652e 6479 6e5f  r_same_base.dyn_
-0000e8f0: 7369 7a65 2069 7320 6e6f 7420 7365 6c66  size is not self
-0000e900: 2e64 796e 5f73 697a 653a 0a20 2020 2020  .dyn_size:.     
-0000e910: 2020 2020 2020 2023 2043 6f75 6c64 2062         # Could b
-0000e920: 6520 756e 7365 7420 6966 2069 7420 636f  e unset if it co
-0000e930: 6d65 7320 6672 6f6d 2074 6865 2063 6f6e  mes from the con
-0000e940: 6669 672c 206f 7220 6672 6f6d 2070 7265  fig, or from pre
-0000e950: 7620 6772 6170 6820 6372 6561 7469 6f6e  v graph creation
-0000e960: 2e0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000e970: 5468 6973 2069 7320 696d 706f 7274 616e  This is importan
-0000e980: 7420 7375 6368 2074 6861 7420 7365 6c66  t such that self
-0000e990: 2e63 616e 5f63 6f6d 7061 7265 2829 2069  .can_compare() i
-0000e9a0: 7320 7361 6e65 2e0a 2020 2020 2020 2020  s sane..        
-0000e9b0: 2020 2020 6966 206f 7468 6572 5f73 616d      if other_sam
-0000e9c0: 655f 6261 7365 2e64 796e 5f73 697a 6520  e_base.dyn_size 
-0000e9d0: 6973 204e 6f6e 6520 6f72 206e 6f74 206f  is None or not o
-0000e9e0: 7468 6572 5f73 616d 655f 6261 7365 2e5f  ther_same_base._
-0000e9f0: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-0000ea00: 656e 745f 6772 6170 6828 293a 0a20 2020  ent_graph():.   
-0000ea10: 2020 2020 2020 2020 2020 2020 206f 7468               oth
-0000ea20: 6572 5f73 616d 655f 6261 7365 2e64 796e  er_same_base.dyn
-0000ea30: 5f73 697a 655f 6578 7420 3d20 7365 6c66  _size_ext = self
-0000ea40: 2e67 6574 5f64 796e 5f73 697a 655f 6578  .get_dyn_size_ex
-0000ea50: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
-0000ea60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea70: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
-0000ea80: 6261 7365 2e62 6174 6368 2c20 6f74 6865  base.batch, othe
-0000ea90: 725f 7361 6d65 5f62 6173 652e 636f 6e74  r_same_base.cont
-0000eaa0: 726f 6c5f 666c 6f77 5f63 7478 2c20 7465  rol_flow_ctx, te
-0000eab0: 6d70 6c61 7465 5f6f 6e6c 793d 5472 7565  mplate_only=True
-0000eac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ead0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000eae0: 2020 206f 7468 6572 5f73 616d 655f 6261     other_same_ba
-0000eaf0: 7365 2e5f 6d61 7962 655f 7570 6461 7465  se._maybe_update
-0000eb00: 2829 0a20 2020 2020 2020 2069 6620 6e6f  ().        if no
-0000eb10: 7420 7365 6c66 2e64 796e 5f73 697a 655f  t self.dyn_size_
-0000eb20: 6578 7420 6f72 206e 6f74 2073 656c 662e  ext or not self.
-0000eb30: 5f76 616c 6964 6174 655f 696e 5f63 7572  _validate_in_cur
-0000eb40: 7265 6e74 5f67 7261 7068 2829 3a0a 2020  rent_graph():.  
-0000eb50: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0000eb60: 796e 5f73 697a 655f 6578 7420 3d20 6f74  yn_size_ext = ot
-0000eb70: 6865 725f 7361 6d65 5f62 6173 652e 6765  her_same_base.ge
-0000eb80: 745f 6479 6e5f 7369 7a65 5f65 7874 5f66  t_dyn_size_ext_f
-0000eb90: 6f72 5f62 6174 6368 5f63 7478 280a 2020  or_batch_ctx(.  
-0000eba0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ebb0: 6c66 2e62 6174 6368 2c20 7365 6c66 2e63  lf.batch, self.c
-0000ebc0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 782c  ontrol_flow_ctx,
-0000ebd0: 2074 656d 706c 6174 655f 6f6e 6c79 3d54   template_only=T
-0000ebe0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0000ebf0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0000ec00: 6c66 2e5f 6d61 7962 655f 7570 6461 7465  lf._maybe_update
-0000ec10: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
-0000ec20: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
-0000ec30: 6479 6e5f 7369 7a65 5f65 7874 2069 7320  dyn_size_ext is 
-0000ec40: 4e6f 6e65 206f 7220 6e6f 7420 6f74 6865  None or not othe
-0000ec50: 725f 7361 6d65 5f62 6173 652e 5f76 616c  r_same_base._val
-0000ec60: 6964 6174 655f 696e 5f63 7572 7265 6e74  idate_in_current
-0000ec70: 5f67 7261 7068 2829 3a0a 2020 2020 2020  _graph():.      
-0000ec80: 2020 2020 2020 6f74 6865 725f 7361 6d65        other_same
-0000ec90: 5f62 6173 652e 6479 6e5f 7369 7a65 5f65  _base.dyn_size_e
-0000eca0: 7874 203d 2073 656c 662e 6765 745f 6479  xt = self.get_dy
-0000ecb0: 6e5f 7369 7a65 5f65 7874 5f66 6f72 5f62  n_size_ext_for_b
-0000ecc0: 6174 6368 5f63 7478 280a 2020 2020 2020  atch_ctx(.      
-0000ecd0: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
-0000ece0: 7361 6d65 5f62 6173 652e 6261 7463 682c  same_base.batch,
-0000ecf0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000ed00: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-0000ed10: 782c 2074 656d 706c 6174 655f 6f6e 6c79  x, template_only
-0000ed20: 3d54 7275 650a 2020 2020 2020 2020 2020  =True.          
-0000ed30: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000ed40: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
-0000ed50: 5f6d 6179 6265 5f75 7064 6174 6528 290a  _maybe_update().
-0000ed60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ed70: 6973 5f64 696d 5f6b 6e6f 776e 2829 2061  is_dim_known() a
-0000ed80: 6e64 206f 7468 6572 2e69 735f 6469 6d5f  nd other.is_dim_
-0000ed90: 6b6e 6f77 6e28 293a 0a20 2020 2020 2020  known():.       
-0000eda0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-0000edb0: 2e64 696d 656e 7369 6f6e 203d 3d20 6f74  .dimension == ot
-0000edc0: 6865 722e 6469 6d65 6e73 696f 6e0a 2020  her.dimension.  
-0000edd0: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-0000ede0: 6973 5f64 696d 5f6b 6e6f 776e 2829 2061  is_dim_known() a
-0000edf0: 6e64 206e 6f74 206f 7468 6572 2e69 735f  nd not other.is_
-0000ee00: 6469 6d5f 6b6e 6f77 6e28 293a 0a20 2020  dim_known():.   
-0000ee10: 2020 2020 2020 2020 206f 7468 6572 2e63           other.c
-0000ee20: 6170 6163 6974 7920 3d20 7365 6c66 2e63  apacity = self.c
-0000ee30: 6170 6163 6974 790a 2020 2020 2020 2020  apacity.        
-0000ee40: 2020 2020 6f74 6865 722e 7369 7a65 203d      other.size =
-0000ee50: 2073 656c 662e 7369 7a65 0a20 2020 2020   self.size.     
-0000ee60: 2020 2065 6c69 6620 6e6f 7420 7365 6c66     elif not self
-0000ee70: 2e69 735f 6469 6d5f 6b6e 6f77 6e28 2920  .is_dim_known() 
-0000ee80: 616e 6420 6f74 6865 722e 6973 5f64 696d  and other.is_dim
-0000ee90: 5f6b 6e6f 776e 2829 3a0a 2020 2020 2020  _known():.      
-0000eea0: 2020 2020 2020 7365 6c66 2e63 6170 6163        self.capac
-0000eeb0: 6974 7920 3d20 6f74 6865 722e 6361 7061  ity = other.capa
-0000eec0: 6369 7479 0a20 2020 2020 2020 2020 2020  city.           
-0000eed0: 2073 656c 662e 7369 7a65 203d 206f 7468   self.size = oth
-0000eee0: 6572 2e73 697a 650a 2020 2020 2020 2020  er.size.        
-0000eef0: 6966 2073 656c 662e 766f 6361 6220 616e  if self.vocab an
-0000ef00: 6420 6e6f 7420 6f74 6865 725f 7361 6d65  d not other_same
-0000ef10: 5f62 6173 652e 766f 6361 623a 0a20 2020  _base.vocab:.   
-0000ef20: 2020 2020 2020 2020 206f 7468 6572 5f73           other_s
-0000ef30: 616d 655f 6261 7365 2e76 6f63 6162 203d  ame_base.vocab =
-0000ef40: 2073 656c 662e 766f 6361 620a 2020 2020   self.vocab.    
-0000ef50: 2020 2020 656c 6966 206f 7468 6572 5f73      elif other_s
-0000ef60: 616d 655f 6261 7365 2e76 6f63 6162 2061  ame_base.vocab a
-0000ef70: 6e64 206e 6f74 2073 656c 662e 766f 6361  nd not self.voca
-0000ef80: 623a 0a20 2020 2020 2020 2020 2020 2073  b:.            s
-0000ef90: 656c 662e 766f 6361 6220 3d20 6f74 6865  elf.vocab = othe
-0000efa0: 725f 7361 6d65 5f62 6173 652e 766f 6361  r_same_base.voca
-0000efb0: 620a 2020 2020 2020 2020 7365 6c66 2e5f  b.        self._
-0000efc0: 6d61 6b65 5f65 7874 7261 2829 0a20 2020  make_extra().   
-0000efd0: 2020 2020 2073 656c 665f 7361 6d65 5f61       self_same_a
-0000efe0: 732e 5f6d 616b 655f 6578 7472 6128 290a  s._make_extra().
-0000eff0: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
-0000f000: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
-0000f010: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
-0000f020: 2073 656c 662e 5f65 7874 7261 2e61 7574   self._extra.aut
-0000f030: 6f5f 6765 6e65 7261 7465 6420 3d20 7365  o_generated = se
-0000f040: 6c66 5f73 616d 655f 6173 2e5f 6578 7472  lf_same_as._extr
-0000f050: 612e 6175 746f 5f67 656e 6572 6174 6564  a.auto_generated
-0000f060: 203d 206f 7468 6572 5f73 616d 655f 6261   = other_same_ba
-0000f070: 7365 2e61 7574 6f5f 6765 6e65 7261 7465  se.auto_generate
-0000f080: 640a 2020 2020 2020 2020 2320 5461 6b65  d.        # Take
-0000f090: 206f 7665 7220 6465 7269 7665 645f 6672   over derived_fr
-0000f0a0: 6f6d 5f6f 702e 2048 6f77 6576 6572 2c20  om_op. However, 
-0000f0b0: 6f6e 6c79 2069 6620 7468 6973 2077 6f75  only if this wou
-0000f0c0: 6c64 206e 6f74 2069 6e74 726f 6475 6365  ld not introduce
-0000f0d0: 2063 7963 6c65 7321 0a20 2020 2020 2020   cycles!.       
-0000f0e0: 2069 6620 6e6f 7420 7365 6c66 5f64 6572   if not self_der
-0000f0f0: 6976 6564 5f62 6173 6573 2e69 7373 7570  ived_bases.issup
-0000f100: 6572 7365 7428 6f74 6865 725f 6465 7269  erset(other_deri
-0000f110: 7665 645f 6261 7365 7329 3a0a 2020 2020  ved_bases):.    
-0000f120: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f130: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-0000f140: 616e 6420 6e6f 7420 6f74 6865 725f 7361  and not other_sa
-0000f150: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
-0000f160: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
-0000f170: 2020 2020 2020 2020 2023 206e 6f69 6e73           # noins
-0000f180: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
-0000f190: 7465 644d 656d 6265 720a 2020 2020 2020  tedMember.      
-0000f1a0: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
-0000f1b0: 7361 6d65 5f62 6173 652e 5f6d 616b 655f  same_base._make_
-0000f1c0: 6578 7472 6128 292e 6465 7269 7665 645f  extra().derived_
-0000f1d0: 6672 6f6d 5f6f 7020 3d20 7365 6c66 2e64  from_op = self.d
-0000f1e0: 6572 6976 6564 5f66 726f 6d5f 6f70 0a20  erived_from_op. 
-0000f1f0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000f200: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
-0000f210: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-0000f220: 616e 6420 6e6f 7420 7365 6c66 2e64 6572  and not self.der
-0000f230: 6976 6564 5f66 726f 6d5f 6f70 3a0a 2020  ived_from_op:.  
-0000f240: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f250: 6c66 2e5f 6d61 6b65 5f65 7874 7261 2829  lf._make_extra()
-0000f260: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-0000f270: 203d 206f 7468 6572 5f73 616d 655f 6261   = other_same_ba
-0000f280: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
-0000f290: 6f70 0a20 2020 2020 2020 2069 6620 7365  op.        if se
-0000f2a0: 6c66 2e5f 6578 7472 6120 616e 6420 6e6f  lf._extra and no
-0000f2b0: 7420 6f74 6865 725f 7361 6d65 5f62 6173  t other_same_bas
-0000f2c0: 652e 6973 5f64 796e 616d 6963 2829 3a0a  e.is_dynamic():.
-0000f2d0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-0000f2e0: 6f73 6520 6d69 6768 7420 6265 2073 6574  ose might be set
-0000f2f0: 2076 6961 2067 6574 5f62 6174 6368 5f66   via get_batch_f
-0000f300: 6f72 5f63 7478 2066 6f72 2061 6e20 756e  or_ctx for an un
-0000f310: 6465 6669 6e65 6420 6469 6d2c 0a20 2020  defined dim,.   
-0000f320: 2020 2020 2020 2020 2023 2077 6869 6368           # which
-0000f330: 206e 6f77 2062 6563 6f6d 6573 2073 7461   now becomes sta
-0000f340: 7469 6320 6475 6520 746f 2060 6f74 6865  tic due to `othe
-0000f350: 7260 2e0a 2020 2020 2020 2020 2020 2020  r`..            
-0000f360: 7365 6c66 2e5f 6578 7472 612e 6261 7463  self._extra.batc
-0000f370: 6820 3d20 4e6f 6e65 0a20 2020 2020 2020  h = None.       
-0000f380: 2020 2020 2073 656c 662e 5f65 7874 7261       self._extra
-0000f390: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
-0000f3a0: 7820 3d20 4e6f 6e65 0a20 2020 2020 2020  x = None.       
-0000f3b0: 2020 2020 2066 6f72 206b 6579 2c20 6469       for key, di
-0000f3c0: 6d5f 2069 6e20 7365 6c66 2e5f 6578 7472  m_ in self._extr
-0000f3d0: 612e 7361 6d65 5f66 6f72 5f62 6174 6368  a.same_for_batch
-0000f3e0: 5f63 7478 2e69 7465 6d73 2829 3a0a 2020  _ctx.items():.  
-0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000f400: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
-0000f410: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
-0000f420: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000f430: 696d 5f65 7874 7261 203d 2064 696d 5f2e  im_extra = dim_.
-0000f440: 5f65 7874 7261 0a20 2020 2020 2020 2020  _extra.         
-0000f450: 2020 2020 2020 2069 6620 6469 6d5f 6578         if dim_ex
-0000f460: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
-0000f470: 2020 2020 2020 2020 2064 696d 5f65 7874           dim_ext
-0000f480: 7261 2e62 6174 6368 203d 204e 6f6e 650a  ra.batch = None.
-0000f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4a0: 2020 2020 6469 6d5f 6578 7472 612e 636f      dim_extra.co
-0000f4b0: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
-0000f4c0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-0000f4d0: 2073 656c 662e 6261 7463 683a 0a20 2020   self.batch:.   
-0000f4e0: 2020 2020 2020 2020 2073 656c 665f 203d           self_ =
-0000f4f0: 2073 656c 662e 6765 745f 666f 725f 6261   self.get_for_ba
-0000f500: 7463 685f 6374 7828 6261 7463 683d 7365  tch_ctx(batch=se
-0000f510: 6c66 2e62 6174 6368 2c20 6374 783d 7365  lf.batch, ctx=se
-0000f520: 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  lf.control_flow_
-0000f530: 6374 7829 0a20 2020 2020 2020 2020 2020  ctx).           
-0000f540: 2069 6620 7365 6c66 5f20 6973 206e 6f74   if self_ is not
-0000f550: 2073 656c 663a 0a20 2020 2020 2020 2020   self:.         
-0000f560: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-0000f570: 726f 6c5f 666c 6f77 5f63 7478 203d 2073  rol_flow_ctx = s
-0000f580: 656c 665f 2e63 6f6e 7472 6f6c 5f66 6c6f  elf_.control_flo
-0000f590: 775f 6374 7820 2023 206d 6967 6874 2062  w_ctx  # might b
-0000f5a0: 6520 6469 6666 6572 656e 740a 2020 2020  e different.    
-0000f5b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f5c0: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
-0000f5d0: 7365 6c66 5f2e 6479 6e5f 7369 7a65 5f65  self_.dyn_size_e
-0000f5e0: 7874 2020 2320 6d69 6768 7420 6265 2075  xt  # might be u
-0000f5f0: 6e73 6574 0a0a 2020 2020 6465 6620 5f6d  nset..    def _m
-0000f600: 6572 6765 5f73 616d 655f 666f 725f 6261  erge_same_for_ba
-0000f610: 7463 685f 6374 785f 6469 6374 2873 656c  tch_ctx_dict(sel
-0000f620: 663a 205f 642e 4469 6d2c 206f 7468 6572  f: _d.Dim, other
-0000f630: 3a20 5f64 2e44 696d 293a 0a20 2020 2020  : _d.Dim):.     
-0000f640: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-0000f650: 7061 7261 6d20 6f74 6865 723a 0a20 2020  param other:.   
-0000f660: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000f670: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
-0000f680: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
-0000f690: 720a 2020 2020 2020 2020 6966 206e 6f74  r.        if not
-0000f6a0: 2073 656c 662e 5f65 7874 7261 2061 6e64   self._extra and
-0000f6b0: 206e 6f74 206f 7468 6572 2e5f 6578 7472   not other._extr
-0000f6c0: 613a 0a20 2020 2020 2020 2020 2020 2072  a:.            r
-0000f6d0: 6574 7572 6e0a 2020 2020 2020 2020 7365  eturn.        se
-0000f6e0: 6c66 2e5f 7661 6c69 6461 7465 5f69 6e5f  lf._validate_in_
-0000f6f0: 6375 7272 656e 745f 6772 6170 6828 290a  current_graph().
-0000f700: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f710: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
-0000f720: 2020 2020 666f 7220 5f2c 2064 696d 2069      for _, dim i
-0000f730: 6e20 6c69 7374 2873 656c 662e 5f65 7874  n list(self._ext
-0000f740: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
-0000f750: 685f 6374 782e 6974 656d 7328 2929 3a0a  h_ctx.items()):.
-0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f770: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
-0000f780: 6528 6469 6d2c 205f 642e 4469 6d29 0a20  e(dim, _d.Dim). 
-0000f790: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000f7a0: 696d 2e5f 7661 6c69 6461 7465 5f69 6e5f  im._validate_in_
-0000f7b0: 6375 7272 656e 745f 6772 6170 6828 290a  current_graph().
-0000f7c0: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
-0000f7d0: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
-0000f7e0: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
-0000f7f0: 2069 6620 6f74 6865 722e 5f65 7874 7261   if other._extra
-0000f800: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000f810: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
-0000f820: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
-0000f830: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-0000f840: 6579 2c20 6469 6d20 696e 206f 7468 6572  ey, dim in other
-0000f850: 2e5f 6578 7472 612e 7361 6d65 5f66 6f72  ._extra.same_for
-0000f860: 5f62 6174 6368 5f63 7478 2e69 7465 6d73  _batch_ctx.items
-0000f870: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000f880: 2020 2020 6966 206e 6f74 2064 696d 2e5f      if not dim._
-0000f890: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-0000f8a0: 656e 745f 6772 6170 6828 293a 0a20 2020  ent_graph():.   
-0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8c0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-0000f8d0: 2020 2020 2020 2020 2020 7365 6c66 5f64            self_d
-0000f8e0: 696d 203d 2073 656c 662e 5f6d 616b 655f  im = self._make_
-0000f8f0: 6578 7472 6128 292e 7361 6d65 5f66 6f72  extra().same_for
-0000f900: 5f62 6174 6368 5f63 7478 2e67 6574 286b  _batch_ctx.get(k
-0000f910: 6579 2c20 4e6f 6e65 290a 2020 2020 2020  ey, None).      
-0000f920: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000f930: 665f 6469 6d20 616e 6420 2873 656c 665f  f_dim and (self_
-0000f940: 6469 6d2e 6479 6e5f 7369 7a65 5f65 7874  dim.dyn_size_ext
-0000f950: 206f 7220 6e6f 7420 6469 6d2e 6479 6e5f   or not dim.dyn_
-0000f960: 7369 7a65 5f65 7874 293a 0a20 2020 2020  size_ext):.     
-0000f970: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000f980: 6f6e 7469 6e75 6520 2023 206b 6565 7020  ontinue  # keep 
-0000f990: 6f75 7273 0a20 2020 2020 2020 2020 2020  ours.           
-0000f9a0: 2020 2020 2069 6620 6e6f 7420 6469 6d2e       if not dim.
-0000f9b0: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
-0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9d0: 2020 636f 6e74 696e 7565 2020 2320 756e    continue  # un
-0000f9e0: 6465 6669 6e65 642c 2064 6f20 6e6f 7420  defined, do not 
-0000f9f0: 6f76 6572 7461 6b65 0a20 2020 2020 2020  overtake.       
-0000fa00: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
-0000fa10: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
-0000fa20: 7463 685f 6374 785b 6b65 795d 203d 2064  tch_ctx[key] = d
-0000fa30: 696d 0a20 2020 2020 2020 2020 2020 2023  im.            #
-0000fa40: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
-0000fa50: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
-0000fa60: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-0000fa70: 722e 5f65 7874 7261 2e73 616d 655f 666f  r._extra.same_fo
-0000fa80: 725f 6261 7463 685f 6374 782e 636c 6561  r_batch_ctx.clea
-0000fa90: 7228 2920 2023 2077 6520 6f6e 6c79 2077  r()  # we only w
-0000faa0: 616e 7420 746f 2068 6176 6520 6974 206f  ant to have it o
-0000fab0: 6e63 650a 0a20 2020 2023 206e 6f69 6e73  nce..    # noins
-0000fac0: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
-0000fad0: 7465 644d 656d 6265 720a 2020 2020 6465  tedMember.    de
-0000fae0: 6620 6465 7269 7665 5f66 726f 6d28 7365  f derive_from(se
-0000faf0: 6c66 3a20 5f64 2e44 696d 2c20 6261 7365  lf: _d.Dim, base
-0000fb00: 3a20 5f64 2e44 696d 2c20 7365 745f 6465  : _d.Dim, set_de
-0000fb10: 7269 7665 645f 6672 6f6d 5f66 6c61 673a  rived_from_flag:
-0000fb20: 2062 6f6f 6c20 3d20 5472 7565 293a 0a20   bool = True):. 
-0000fb30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000fb40: 2020 203a 7061 7261 6d20 6261 7365 3a20     :param base: 
-0000fb50: 6469 6d0a 2020 2020 2020 2020 3a70 6172  dim.        :par
-0000fb60: 616d 2073 6574 5f64 6572 6976 6564 5f66  am set_derived_f
-0000fb70: 726f 6d5f 666c 6167 3a0a 2020 2020 2020  rom_flag:.      
-0000fb80: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-0000fb90: 6c66 5f62 6173 6520 3d20 7365 6c66 2e67  lf_base = self.g
-0000fba0: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
-0000fbb0: 2020 2020 2020 2073 656c 665f 6261 7365         self_base
-0000fbc0: 5f65 7874 7261 203d 2073 656c 665f 6261  _extra = self_ba
-0000fbd0: 7365 2e5f 6d61 6b65 5f65 7874 7261 2829  se._make_extra()
-0000fbe0: 0a20 2020 2020 2020 2069 6620 7365 745f  .        if set_
-0000fbf0: 6465 7269 7665 645f 6672 6f6d 5f66 6c61  derived_from_fla
-0000fc00: 673a 0a20 2020 2020 2020 2020 2020 2069  g:.            i
-0000fc10: 6620 7365 6c66 5f62 6173 655f 6578 7472  f self_base_extr
-0000fc20: 612e 6465 7269 7665 645f 6672 6f6d 5f74  a.derived_from_t
-0000fc30: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
-0000fc40: 2020 2020 6173 7365 7274 2073 656c 665f      assert self_
-0000fc50: 6261 7365 5f65 7874 7261 2e64 6572 6976  base_extra.deriv
-0000fc60: 6564 5f66 726f 6d5f 7461 6720 3d3d 2062  ed_from_tag == b
-0000fc70: 6173 650a 2020 2020 2020 2020 2020 2020  ase.            
-0000fc80: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000fc90: 2020 2020 2020 7365 6c66 5f62 6173 655f        self_base_
-0000fca0: 6578 7472 612e 6465 7269 7665 645f 6672  extra.derived_fr
-0000fcb0: 6f6d 5f74 6167 203d 2062 6173 650a 2020  om_tag = base.  
-0000fcc0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-0000fcd0: 662e 6261 7463 6820 616e 6420 6261 7365  f.batch and base
-0000fce0: 2e62 6174 6368 3a0a 2020 2020 2020 2020  .batch:.        
-0000fcf0: 2020 2020 7365 6c66 2e62 6174 6368 203d      self.batch =
-0000fd00: 2062 6173 652e 6261 7463 680a 2020 2020   base.batch.    
-0000fd10: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000fd20: 7472 6f6c 5f66 6c6f 775f 6374 7820 3d20  trol_flow_ctx = 
-0000fd30: 6261 7365 2e63 6f6e 7472 6f6c 5f66 6c6f  base.control_flo
-0000fd40: 775f 6374 780a 2020 2020 2020 2020 2020  w_ctx.          
-0000fd50: 2020 6b65 7920 3d20 6261 7365 2e62 6174    key = base.bat
-0000fd60: 6368 2c20 6261 7365 2e63 6f6e 7472 6f6c  ch, base.control
-0000fd70: 5f66 6c6f 775f 6374 780a 2020 2020 2020  _flow_ctx.      
-0000fd80: 2020 2020 2020 6173 7365 7274 206b 6579        assert key
-0000fd90: 206e 6f74 2069 6e20 7365 6c66 5f62 6173   not in self_bas
-0000fda0: 655f 6578 7472 612e 7361 6d65 5f66 6f72  e_extra.same_for
-0000fdb0: 5f62 6174 6368 5f63 7478 0a20 2020 2020  _batch_ctx.     
-0000fdc0: 2020 2020 2020 2073 656c 665f 6261 7365         self_base
-0000fdd0: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
-0000fde0: 6261 7463 685f 6374 785b 6b65 795d 203d  batch_ctx[key] =
-0000fdf0: 2073 656c 660a 2020 2020 2020 2020 6966   self.        if
-0000fe00: 2073 656c 662e 6973 5f64 796e 616d 6963   self.is_dynamic
-0000fe10: 2829 206f 7220 6e6f 7420 7365 6c66 2e69  () or not self.i
-0000fe20: 735f 6469 6d5f 6b6e 6f77 6e28 293a 0a20  s_dim_known():. 
-0000fe30: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000fe40: 7420 7365 6c66 2e64 796e 5f73 697a 655f  t self.dyn_size_
-0000fe50: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-0000fe60: 2020 2020 2069 6620 6261 7365 2e64 796e       if base.dyn
-0000fe70: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-0000fe80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000fe90: 6620 6261 7365 2e62 6174 6368 2061 6e64  f base.batch and
-0000fea0: 2062 6173 652e 6261 7463 6820 3d3d 2073   base.batch == s
-0000feb0: 656c 662e 6261 7463 6820 616e 6420 6261  elf.batch and ba
-0000fec0: 7365 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  se.control_flow_
-0000fed0: 6374 7820 3d3d 2073 656c 662e 636f 6e74  ctx == self.cont
-0000fee0: 726f 6c5f 666c 6f77 5f63 7478 3a0a 2020  rol_flow_ctx:.  
-0000fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff00: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
-0000ff10: 697a 655f 6578 7420 3d20 6261 7365 2e64  ize_ext = base.d
-0000ff20: 796e 5f73 697a 655f 6578 742e 636f 7079  yn_size_ext.copy
-0000ff30: 5f74 656d 706c 6174 6528 6e61 6d65 3d22  _template(name="
-0000ff40: 2573 3a73 697a 6522 2025 2073 656c 665f  %s:size" % self_
-0000ff50: 6261 7365 2e64 6573 6372 6970 7469 6f6e  base.description
-0000ff60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ff70: 2020 656c 6966 2062 6173 652e 6973 5f62    elif base.is_b
-0000ff80: 6174 6368 5f64 696d 2829 3a0a 2020 2020  atch_dim():.    
-0000ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffa0: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-0000ffb0: 7420 3d20 5f74 2e54 656e 736f 7228 0a20  t = _t.Tensor(. 
-0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffd0: 2020 2020 2020 206e 616d 653d 2225 733a         name="%s:
-0000ffe0: 6261 7463 6822 2025 2073 656c 665f 6261  batch" % self_ba
-0000fff0: 7365 2e64 6573 6372 6970 7469 6f6e 2c20  se.description, 
-00010000: 7368 6170 653d 2829 2c20 6474 7970 653d  shape=(), dtype=
-00010010: 2269 6e74 3332 222c 2062 6174 6368 5f64  "int32", batch_d
-00010020: 696d 5f61 7869 733d 4e6f 6e65 0a20 2020  im_axis=None.   
-00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010040: 2029 0a0a 2020 2020 6465 6620 636f 7079   )..    def copy
-00010050: 5f66 726f 6d28 7365 6c66 3a20 4469 6d2c  _from(self: Dim,
-00010060: 206f 7468 6572 3a20 4469 6d29 3a0a 2020   other: Dim):.  
-00010070: 2020 2020 2020 2222 2264 6566 696e 6522        """define"
-00010080: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00010090: 7369 7a65 203d 206f 7468 6572 2e73 697a  size = other.siz
-000100a0: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
-000100b0: 6170 6163 6974 7920 3d20 6f74 6865 722e  apacity = other.
-000100c0: 6361 7061 6369 7479 0a20 2020 2020 2020  capacity.       
-000100d0: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-000100e0: 7874 203d 206f 7468 6572 2e64 796e 5f73  xt = other.dyn_s
-000100f0: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
-00010100: 7365 6c66 2e64 6572 6976 655f 6672 6f6d  self.derive_from
-00010110: 286f 7468 6572 290a 0a20 2020 2040 636c  (other)..    @cl
-00010120: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00010130: 6620 6765 745f 6578 6973 7469 6e67 5f74  f get_existing_t
-00010140: 6167 5f66 726f 6d5f 636f 6c6c 6563 7469  ag_from_collecti
-00010150: 6f6e 2863 6c73 2c20 6f74 6865 722c 2074  on(cls, other, t
-00010160: 6167 732c 2069 735f 6571 7561 6c5f 6f70  ags, is_equal_op
-00010170: 7473 3d4e 6f6e 6529 3a0a 2020 2020 2020  ts=None):.      
-00010180: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00010190: 6172 616d 2044 696d 206f 7468 6572 3a0a  aram Dim other:.
-000101a0: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
-000101b0: 6973 745b 4469 6d5d 7c74 7570 6c65 5b44  ist[Dim]|tuple[D
-000101c0: 696d 5d7c 7365 745b 4469 6d5d 2074 6167  im]|set[Dim] tag
-000101d0: 733a 0a20 2020 2020 2020 203a 7061 7261  s:.        :para
-000101e0: 6d20 6469 6374 5b73 7472 5d7c 4e6f 6e65  m dict[str]|None
-000101f0: 2069 735f 6571 7561 6c5f 6f70 7473 3a20   is_equal_opts: 
-00010200: 7061 7373 6564 2074 6f20 4469 6d2e 6973  passed to Dim.is
-00010210: 5f65 7175 616c 0a20 2020 2020 2020 203a  _equal.        :
-00010220: 7274 7970 653a 2044 696d 7c4e 6f6e 650a  rtype: Dim|None.
-00010230: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010240: 2020 2020 6966 2069 735f 6571 7561 6c5f      if is_equal_
-00010250: 6f70 7473 2069 7320 4e6f 6e65 3a0a 2020  opts is None:.  
-00010260: 2020 2020 2020 2020 2020 6973 5f65 7175            is_equ
-00010270: 616c 5f6f 7074 7320 3d20 7b7d 0a20 2020  al_opts = {}.   
-00010280: 2020 2020 2023 2057 6520 646f 2070 6f74       # We do pot
-00010290: 656e 7469 616c 206d 756c 7469 706c 6520  ential multiple 
-000102a0: 726f 756e 6473 2c20 7375 6368 2074 6861  rounds, such tha
-000102b0: 7420 7765 2070 7265 6665 7220 226d 6f72  t we prefer "mor
-000102c0: 6520 6571 7561 6c22 2028 7573 696e 6720  e equal" (using 
-000102d0: 6c65 7373 2069 735f 6571 7561 6c5f 6f70  less is_equal_op
-000102e0: 7473 292e 0a20 2020 2020 2020 2072 6f75  ts)..        rou
-000102f0: 6e64 7320 3d20 5b7b 7d5d 0a20 2020 2020  nds = [{}].     
-00010300: 2020 2069 6620 6973 5f65 7175 616c 5f6f     if is_equal_o
-00010310: 7074 733a 0a20 2020 2020 2020 2020 2020  pts:.           
-00010320: 2069 6620 2262 726f 6164 6361 7374 5f6d   if "broadcast_m
-00010330: 6174 6368 6573 2220 696e 2069 735f 6571  atches" in is_eq
-00010340: 7561 6c5f 6f70 7473 3a0a 2020 2020 2020  ual_opts:.      
-00010350: 2020 2020 2020 2020 2020 726f 756e 6473            rounds
-00010360: 2e61 7070 656e 6428 7b6b 3a20 7620 666f  .append({k: v fo
-00010370: 7220 286b 2c20 7629 2069 6e20 6973 5f65  r (k, v) in is_e
-00010380: 7175 616c 5f6f 7074 732e 6974 656d 7328  qual_opts.items(
-00010390: 2920 6966 206b 2021 3d20 2262 726f 6164  ) if k != "broad
-000103a0: 6361 7374 5f6d 6174 6368 6573 227d 290a  cast_matches"}).
-000103b0: 2020 2020 2020 2020 2020 2020 726f 756e              roun
-000103c0: 6473 2e61 7070 656e 6428 6973 5f65 7175  ds.append(is_equ
-000103d0: 616c 5f6f 7074 7329 0a20 2020 2020 2020  al_opts).       
-000103e0: 2066 6f72 205f 6973 5f65 7175 616c 5f6f   for _is_equal_o
-000103f0: 7074 7320 696e 2072 6f75 6e64 733a 0a20  pts in rounds:. 
-00010400: 2020 2020 2020 2020 2020 2066 6f72 205f             for _
-00010410: 7461 6720 696e 2074 6167 733a 0a20 2020  tag in tags:.   
-00010420: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010430: 5f74 6167 2e69 735f 6571 7561 6c28 6f74  _tag.is_equal(ot
-00010440: 6865 722c 202a 2a5f 6973 5f65 7175 616c  her, **_is_equal
-00010450: 5f6f 7074 7329 3a0a 2020 2020 2020 2020  _opts):.        
-00010460: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00010470: 726e 205f 7461 670a 2020 2020 2020 2020  rn _tag.        
-00010480: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00010490: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-000104a0: 2020 6465 6620 6765 745f 616c 6c5f 6469    def get_all_di
-000104b0: 6d65 6e73 696f 6e5f 7461 6773 2863 6c73  mension_tags(cls
-000104c0: 2c20 6461 7461 5f6c 6973 742c 2069 735f  , data_list, is_
-000104d0: 6571 7561 6c5f 6f70 7473 3d4e 6f6e 652c  equal_opts=None,
-000104e0: 2075 6e69 7175 655f 7365 7061 7261 7465   unique_separate
-000104f0: 5f61 7865 733d 5472 7565 293a 0a20 2020  _axes=True):.   
-00010500: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00010510: 203a 7061 7261 6d20 6c69 7374 5b5f 742e   :param list[_t.
-00010520: 5465 6e73 6f72 5d20 6461 7461 5f6c 6973  Tensor] data_lis
-00010530: 743a 0a20 2020 2020 2020 203a 7061 7261  t:.        :para
-00010540: 6d20 6469 6374 5b73 7472 5d7c 4e6f 6e65  m dict[str]|None
-00010550: 2069 735f 6571 7561 6c5f 6f70 7473 3a20   is_equal_opts: 
-00010560: 7061 7373 6564 2074 6f20 4469 6d2e 6973  passed to Dim.is
-00010570: 5f65 7175 616c 0a20 2020 2020 2020 203a  _equal.        :
-00010580: 7061 7261 6d20 626f 6f6c 2075 6e69 7175  param bool uniqu
-00010590: 655f 7365 7061 7261 7465 5f61 7865 733a  e_separate_axes:
-000105a0: 2065 2e67 2e20 6461 7461 5f6c 6973 743d   e.g. data_list=
-000105b0: 5b44 6174 6120 7769 7468 2073 6861 7065  [Data with shape
-000105c0: 2028 422c 352c 352c 3130 295d 2072 6573   (B,5,5,10)] res
-000105d0: 756c 7473 2069 6e20 3420 6469 6d20 7461  ults in 4 dim ta
-000105e0: 6773 2c20 6e6f 7420 332e 0a20 2020 2020  gs, not 3..     
-000105f0: 2020 203a 7265 7475 726e 3a20 6c69 7374     :return: list
-00010600: 206f 6620 6469 6d65 6e73 696f 6e20 7461   of dimension ta
-00010610: 6773 2c20 6469 6374 2066 6f72 2064 6174  gs, dict for dat
-00010620: 6120 2d3e 206c 6973 7420 6f66 2064 696d  a -> list of dim
-00010630: 656e 7369 6f6e 2074 6167 7320 2866 6f72  ension tags (for
-00010640: 2065 6163 6820 6178 6973 290a 2020 2020   each axis).    
-00010650: 2020 2020 3a72 7479 7065 3a20 286c 6973      :rtype: (lis
-00010660: 745b 4469 6d5d 2c20 7574 696c 2e44 6963  t[Dim], util.Dic
-00010670: 7452 6566 4b65 7973 5b5f 742e 5465 6e73  tRefKeys[_t.Tens
-00010680: 6f72 2c20 6c69 7374 5b44 696d 5d5d 290a  or, list[Dim]]).
-00010690: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000106a0: 2020 2020 7461 6773 203d 205b 5d0a 2020      tags = [].  
-000106b0: 2020 2020 2020 6461 7461 5f61 7865 735f        data_axes_
-000106c0: 6469 6374 203d 2075 7469 6c2e 4469 6374  dict = util.Dict
-000106d0: 5265 664b 6579 7328 2920 2023 2074 7970  RefKeys()  # typ
-000106e0: 653a 2075 7469 6c2e 4469 6374 5265 664b  e: util.DictRefK
-000106f0: 6579 735b 5f74 2e54 656e 736f 722c 204c  eys[_t.Tensor, L
-00010700: 6973 745b 4469 6d5d 5d0a 2020 2020 2020  ist[Dim]].      
-00010710: 2020 666f 7220 6461 7461 2069 6e20 6461    for data in da
-00010720: 7461 5f6c 6973 743a 0a20 2020 2020 2020  ta_list:.       
-00010730: 2020 2020 2064 6174 615f 6178 6573 5f64       data_axes_d
-00010740: 6963 745b 6461 7461 5d20 3d20 5b5d 0a20  ict[data] = []. 
-00010750: 2020 2020 2020 2020 2020 2065 7869 7374             exist
-00010760: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
-00010770: 6f6e 5f66 6f72 5f64 6174 6120 3d20 6c69  on_for_data = li
-00010780: 7374 2874 6167 7329 2069 6620 756e 6971  st(tags) if uniq
-00010790: 7565 5f73 6570 6172 6174 655f 6178 6573  ue_separate_axes
-000107a0: 2065 6c73 6520 7461 6773 0a20 2020 2020   else tags.     
-000107b0: 2020 2020 2020 2066 6f72 2061 7869 7320         for axis 
-000107c0: 696e 2072 616e 6765 2864 6174 612e 6261  in range(data.ba
-000107d0: 7463 685f 6e64 696d 293a 0a20 2020 2020  tch_ndim):.     
-000107e0: 2020 2020 2020 2020 2020 2074 6167 203d             tag =
-000107f0: 2064 6174 612e 6765 745f 6469 6d5f 7461   data.get_dim_ta
-00010800: 6728 6178 6973 290a 2020 2020 2020 2020  g(axis).        
-00010810: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
-00010820: 5f74 6167 203d 2063 6c73 2e67 6574 5f65  _tag = cls.get_e
-00010830: 7869 7374 696e 675f 7461 675f 6672 6f6d  xisting_tag_from
-00010840: 5f63 6f6c 6c65 6374 696f 6e28 0a20 2020  _collection(.   
-00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010860: 2074 6167 2c20 7461 6773 3d65 7869 7374   tag, tags=exist
-00010870: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
-00010880: 6f6e 5f66 6f72 5f64 6174 612c 2069 735f  on_for_data, is_
-00010890: 6571 7561 6c5f 6f70 7473 3d69 735f 6571  equal_opts=is_eq
-000108a0: 7561 6c5f 6f70 7473 0a20 2020 2020 2020  ual_opts.       
-000108b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000108c0: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
-000108d0: 6973 7469 6e67 5f74 6167 3a0a 2020 2020  isting_tag:.    
-000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108f0: 6966 2075 6e69 7175 655f 7365 7061 7261  if unique_separa
-00010900: 7465 5f61 7865 733a 0a20 2020 2020 2020  te_axes:.       
-00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010920: 2065 7869 7374 696e 675f 7461 675f 636f   existing_tag_co
-00010930: 6c6c 6563 7469 6f6e 5f66 6f72 5f64 6174  llection_for_dat
-00010940: 612e 7265 6d6f 7665 2865 7869 7374 696e  a.remove(existin
-00010950: 675f 7461 6729 2020 2320 646f 6e27 7420  g_tag)  # don't 
-00010960: 7461 6b65 2069 7420 6167 6169 6e20 666f  take it again fo
-00010970: 7220 7468 6973 2064 6174 610a 2020 2020  r this data.    
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 7265 706c 6163 655f 6578 6973 7469 6e67  replace_existing
-000109a0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-000109b0: 2020 2020 2020 2020 2020 2020 2065 7869               exi
-000109c0: 7374 696e 675f 7461 672e 756e 6465 6669  sting_tag.undefi
-000109d0: 6e65 6420 616e 6420 6e6f 7420 7461 672e  ned and not tag.
-000109e0: 756e 6465 6669 6e65 6420 616e 6420 7461  undefined and ta
-000109f0: 672e 6469 6d65 6e73 696f 6e20 3d3d 2065  g.dimension == e
-00010a00: 7869 7374 696e 675f 7461 672e 6469 6d65  xisting_tag.dime
-00010a10: 6e73 696f 6e0a 2020 2020 2020 2020 2020  nsion.          
-00010a20: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000de30: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
+0000de40: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
+0000de50: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000de60: 2020 2020 2020 2020 2020 6469 6d5f 2e5f            dim_._
+0000de70: 6578 7472 612e 6465 7269 7665 645f 6672  extra.derived_fr
+0000de80: 6f6d 5f6f 7020 3d20 4e6f 6e65 0a20 2020  om_op = None.   
+0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dea0: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
+0000deb0: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
+0000dec0: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
+0000ded0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+0000dee0: 6d5f 2e5f 6578 7472 612e 6465 7269 7665  m_._extra.derive
+0000def0: 645f 6672 6f6d 5f74 6167 203d 204e 6f6e  d_from_tag = Non
+0000df00: 650a 2020 2020 2020 2020 2320 4e6f 7720  e.        # Now 
+0000df10: 6d65 7267 6520 6578 6973 7469 6e67 2076  merge existing v
+0000df20: 6172 6961 6e74 732e 2042 7574 206f 6e6c  ariants. But onl
+0000df30: 7920 6966 206e 6f74 2064 6572 6976 6564  y if not derived
+0000df40: 2076 6961 206f 702c 2062 6563 6175 7365   via op, because
+0000df50: 2069 6e20 7468 6174 2063 6173 652c 2077   in that case, w
+0000df60: 6520 6361 6e20 2861 6e64 2073 686f 756c  e can (and shoul
+0000df70: 6421 290a 2020 2020 2020 2020 2320 6175  d!).        # au
+0000df80: 746f 6d61 7469 6361 6c6c 7920 696e 6665  tomatically infe
+0000df90: 7220 6974 2e20 4e6f 7465 2074 6861 7420  r it. Note that 
+0000dfa0: 7765 206f 6e6c 7920 676f 7420 6865 7265  we only got here
+0000dfb0: 2077 6865 6e20 7468 6520 6f74 6865 7220   when the other 
+0000dfc0: 6973 206e 6f74 2074 6865 2073 616d 6520  is not the same 
+0000dfd0: 6469 6d2c 2073 6f20 6974 206d 6561 6e73  dim, so it means
+0000dfe0: 2074 6861 740a 2020 2020 2020 2020 2320   that.        # 
+0000dff0: 7468 6520 6f74 6865 7220 6973 2072 6561  the other is rea
+0000e000: 6c6c 7920 6469 6666 6572 656e 742c 2074  lly different, t
+0000e010: 6865 2073 697a 6573 2061 7265 2070 6f74  he sizes are pot
+0000e020: 656e 7469 616c 6c79 2064 6966 6665 7265  entially differe
+0000e030: 6e74 2c20 6275 7420 7765 2077 616e 7420  nt, but we want 
+0000e040: 746f 206f 7665 7274 616b 6520 7468 6520  to overtake the 
+0000e050: 6f74 6865 722e 0a20 2020 2020 2020 2069  other..        i
+0000e060: 6620 6f74 6865 725f 7361 6d65 5f62 6173  f other_same_bas
+0000e070: 652e 6465 7269 7665 645f 6672 6f6d 5f6f  e.derived_from_o
+0000e080: 703a 0a20 2020 2020 2020 2020 2020 2023  p:.            #
+0000e090: 2043 6c65 616e 7570 2065 7665 7279 7468   Cleanup everyth
+0000e0a0: 696e 672c 2065 7370 2070 6f74 656e 7469  ing, esp potenti
+0000e0b0: 616c 2061 6c72 6561 6479 2063 6f6d 7075  al already compu
+0000e0c0: 7465 6420 7369 7a65 732c 2061 7320 7468  ted sizes, as th
+0000e0d0: 6573 6520 6d69 6768 7420 6265 2069 6e76  ese might be inv
+0000e0e0: 616c 6964 2e0a 2020 2020 2020 2020 2020  alid..          
+0000e0f0: 2020 666f 7220 6469 6d5f 2069 6e20 5b73    for dim_ in [s
+0000e100: 656c 665f 7361 6d65 5f61 732c 2073 656c  elf_same_as, sel
+0000e110: 665d 202b 2028 6c69 7374 2873 656c 662e  f] + (list(self.
+0000e120: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000e130: 6261 7463 685f 6374 782e 7661 6c75 6573  batch_ctx.values
+0000e140: 2829 2920 6966 2073 656c 662e 5f65 7874  ()) if self._ext
+0000e150: 7261 2065 6c73 6520 5b5d 293a 0a20 2020  ra else []):.   
+0000e160: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000e170: 6469 6d5f 2e64 796e 5f73 697a 655f 6578  dim_.dyn_size_ex
+0000e180: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000e190: 2020 2020 2020 2064 696d 5f2e 6479 6e5f         dim_.dyn_
+0000e1a0: 7369 7a65 5f65 7874 2e70 6c61 6365 686f  size_ext.placeho
+0000e1b0: 6c64 6572 203d 204e 6f6e 650a 2020 2020  lder = None.    
+0000e1c0: 2020 2020 6f74 6865 725f 7361 6d65 5f62      other_same_b
+0000e1d0: 6173 652e 5f6d 6572 6765 5f73 616d 655f  ase._merge_same_
+0000e1e0: 666f 725f 6261 7463 685f 6374 785f 6469  for_batch_ctx_di
+0000e1f0: 6374 2873 656c 6629 0a20 2020 2020 2020  ct(self).       
+0000e200: 206f 7468 6572 2e5f 6d61 7962 655f 7570   other._maybe_up
+0000e210: 6461 7465 2829 0a20 2020 2020 2020 2073  date().        s
+0000e220: 656c 662e 7361 6d65 5f61 7320 3d20 6f74  elf.same_as = ot
+0000e230: 6865 725f 7361 6d65 5f62 6173 650a 2020  her_same_base.  
+0000e240: 2020 2020 2020 7365 6c66 2e5f 6d61 7962        self._mayb
+0000e250: 655f 7570 6461 7465 2829 0a20 2020 2020  e_update().     
+0000e260: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
+0000e270: 697a 6520 6973 206e 6f74 204e 6f6e 6520  ize is not None 
+0000e280: 616e 6420 6f74 6865 725f 7361 6d65 5f62  and other_same_b
+0000e290: 6173 652e 6479 6e5f 7369 7a65 2069 7320  ase.dyn_size is 
+0000e2a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000e2b0: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
+0000e2c0: 6e5f 7369 7a65 2069 7320 6e6f 7420 6f74  n_size is not ot
+0000e2d0: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
+0000e2e0: 6e5f 7369 7a65 3a0a 2020 2020 2020 2020  n_size:.        
+0000e2f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000e300: 6261 7463 6820 3d3d 206f 7468 6572 5f73  batch == other_s
+0000e310: 616d 655f 6261 7365 2e62 6174 6368 2061  ame_base.batch a
+0000e320: 6e64 2073 656c 662e 636f 6e74 726f 6c5f  nd self.control_
+0000e330: 666c 6f77 5f63 7478 203d 3d20 6f74 6865  flow_ctx == othe
+0000e340: 725f 7361 6d65 5f62 6173 652e 636f 6e74  r_same_base.cont
+0000e350: 726f 6c5f 666c 6f77 5f63 7478 3a0a 2020  rol_flow_ctx:.  
+0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e370: 2020 2320 4e6f 7465 3a20 496e 7374 6561    # Note: Instea
+0000e380: 6420 6f66 206d 616b 696e 6720 7468 6973  d of making this
+0000e390: 2061 2077 6172 6e69 6e67 2c20 7765 2063   a warning, we c
+0000e3a0: 6f75 6c64 2061 6c73 6f20 656e 666f 7263  ould also enforc
+0000e3b0: 6520 7468 6973 2061 7420 736f 6d65 2070  e this at some p
+0000e3c0: 6f69 6e74 2e0a 2020 2020 2020 2020 2020  oint..          
+0000e3d0: 2020 2020 2020 2020 2020 2320 2020 5468            #   Th
+0000e3e0: 6520 7573 6572 2073 686f 756c 6420 6265  e user should be
+0000e3f0: 2061 626c 6520 746f 2066 6978 2060 6578   able to fix `ex
+0000e400: 7465 726e 5f64 6174 6160 2069 6e20 7468  tern_data` in th
+0000e410: 6520 636f 6e66 6967 0a20 2020 2020 2020  e config.       
+0000e420: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+0000e430: 2073 7563 6820 7468 6174 2074 6869 7320   such that this 
+0000e440: 6973 2063 6f72 7265 6374 2069 6e20 7468  is correct in th
+0000e450: 6520 6669 7273 7420 706c 6163 652e 0a20  e first place.. 
+0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e470: 2020 2023 2020 2041 6c73 6f2c 2069 6e20     #   Also, in 
+0000e480: 6164 6469 7469 6f6e 2074 6f20 7468 6973  addition to this
+0000e490: 2077 6172 6e69 6e67 2c0a 2020 2020 2020   warning,.      
+0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000e4b0: 2020 7765 206d 6967 6874 2077 616e 7420    we might want 
+0000e4c0: 746f 2061 6464 2073 6f6d 6520 7275 6e74  to add some runt
+0000e4d0: 696d 6520 6368 6563 6b20 6f6e 2074 6865  ime check on the
+0000e4e0: 2065 7120 6f66 2074 6865 2064 796e 2073   eq of the dyn s
+0000e4f0: 697a 6573 2e0a 2020 2020 2020 2020 2020  izes..          
+0000e500: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000e510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e520: 2020 2020 2020 2020 2022 5761 726e 696e           "Warnin
+0000e530: 673a 2061 7373 756d 696e 6720 6469 6d20  g: assuming dim 
+0000e540: 7461 6773 2061 7265 2073 616d 6520 7769  tags are same wi
+0000e550: 7468 2064 6966 6665 7265 6e74 2073 697a  th different siz
+0000e560: 6520 706c 6163 6568 6f6c 6465 7273 3a20  e placeholders: 
+0000e570: 2572 2076 7320 2572 220a 2020 2020 2020  %r vs %r".      
+0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e590: 2020 2520 2873 656c 662e 6479 6e5f 7369    % (self.dyn_si
+0000e5a0: 7a65 2c20 6f74 6865 725f 7361 6d65 5f62  ze, other_same_b
+0000e5b0: 6173 652e 6479 6e5f 7369 7a65 290a 2020  ase.dyn_size).  
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5d0: 2020 290a 2020 2020 2020 2020 2320 4966    ).        # If
+0000e5e0: 2077 6520 6861 7665 2061 2064 6566 696e   we have a defin
+0000e5f0: 6564 2073 6f75 7263 652c 2061 6e64 2074  ed source, and t
+0000e600: 6869 7320 6973 2061 2064 796e 616d 6963  his is a dynamic
+0000e610: 2073 7061 7469 616c 2061 7869 732c 2061   spatial axis, a
+0000e620: 6e64 2069 7420 7761 7320 756e 6465 6669  nd it was undefi
+0000e630: 6e65 6420 6265 666f 7265 2c0a 2020 2020  ned before,.    
+0000e640: 2020 2020 2320 6d61 7962 6520 7765 2063      # maybe we c
+0000e650: 616e 206f 7665 7274 616b 6520 7468 6520  an overtake the 
+0000e660: 7369 7a65 5f70 6c61 6365 686f 6c64 6572  size_placeholder
+0000e670: 206e 6f77 2e0a 2020 2020 2020 2020 6966   now..        if
+0000e680: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000e690: 2e64 796e 5f73 697a 6520 6973 206e 6f74  .dyn_size is not
+0000e6a0: 204e 6f6e 6520 616e 6420 7365 6c66 2e5f   None and self._
+0000e6b0: 6578 7472 6120 616e 6420 7365 6c66 2e5f  extra and self._
+0000e6c0: 6578 7472 612e 7372 635f 6461 7461 3a0a  extra.src_data:.
+0000e6d0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000e6e0: 7274 2069 7369 6e73 7461 6e63 6528 7365  rt isinstance(se
+0000e6f0: 6c66 2e5f 6578 7472 612e 7372 635f 6178  lf._extra.src_ax
+0000e700: 6973 2c20 696e 7429 0a20 2020 2020 2020  is, int).       
+0000e710: 2020 2020 2023 204d 6179 6265 2069 7420       # Maybe it 
+0000e720: 6368 616e 6765 6420 696e 2074 6865 206d  changed in the m
+0000e730: 6561 6e77 6869 6c65 2c20 736f 2063 6865  eanwhile, so che
+0000e740: 636b 2e0a 2020 2020 2020 2020 2020 2020  ck..            
+0000e750: 7461 6720 3d20 7365 6c66 2e5f 6578 7472  tag = self._extr
+0000e760: 612e 7372 635f 6461 7461 2e67 6574 5f64  a.src_data.get_d
+0000e770: 696d 5f74 6167 2873 656c 662e 5f65 7874  im_tag(self._ext
+0000e780: 7261 2e73 7263 5f61 7869 7329 0a20 2020  ra.src_axis).   
+0000e790: 2020 2020 2020 2020 2069 6620 7461 672e           if tag.
+0000e7a0: 6465 7363 7269 7074 696f 6e20 3d3d 2073  description == s
+0000e7b0: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
+0000e7c0: 616e 6420 286e 6f74 2074 6167 2e64 796e  and (not tag.dyn
+0000e7d0: 5f73 697a 655f 6578 7420 6f72 206e 6f74  _size_ext or not
+0000e7e0: 2074 6167 2e5f 7661 6c69 6461 7465 5f69   tag._validate_i
+0000e7f0: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+0000e800: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000e810: 2020 2020 7461 672e 6479 6e5f 7369 7a65      tag.dyn_size
+0000e820: 5f65 7874 203d 2073 656c 662e 6765 745f  _ext = self.get_
+0000e830: 6479 6e5f 7369 7a65 5f65 7874 5f66 6f72  dyn_size_ext_for
+0000e840: 5f62 6174 6368 5f63 7478 280a 2020 2020  _batch_ctx(.    
+0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e860: 7461 672e 6261 7463 682c 2074 6167 2e63  tag.batch, tag.c
+0000e870: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 782c  ontrol_flow_ctx,
+0000e880: 2074 656d 706c 6174 655f 6f6e 6c79 3d54   template_only=T
+0000e890: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000e8a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000e8b0: 2020 2020 2020 7461 672e 5f6d 6179 6265        tag._maybe
+0000e8c0: 5f75 7064 6174 6528 290a 2020 2020 2020  _update().      
+0000e8d0: 2020 2320 4966 206f 7468 6572 7320 6479    # If others dy
+0000e8e0: 6e5f 7369 7a65 2069 7320 4e6f 6e65 2062  n_size is None b
+0000e8f0: 7574 2077 6520 6861 7665 2061 2064 796e  ut we have a dyn
+0000e900: 5f73 697a 652c 206d 6179 6265 2075 7064  _size, maybe upd
+0000e910: 6174 6520 6f74 6865 7273 2064 796e 5f73  ate others dyn_s
+0000e920: 697a 652e 0a20 2020 2020 2020 2069 6620  ize..        if 
+0000e930: 7365 6c66 2e64 796e 5f73 697a 6520 6973  self.dyn_size is
+0000e940: 206e 6f74 204e 6f6e 6520 616e 6420 6f74   not None and ot
+0000e950: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
+0000e960: 6e5f 7369 7a65 2069 7320 6e6f 7420 7365  n_size is not se
+0000e970: 6c66 2e64 796e 5f73 697a 653a 0a20 2020  lf.dyn_size:.   
+0000e980: 2020 2020 2020 2020 2023 2043 6f75 6c64           # Could
+0000e990: 2062 6520 756e 7365 7420 6966 2069 7420   be unset if it 
+0000e9a0: 636f 6d65 7320 6672 6f6d 2074 6865 2063  comes from the c
+0000e9b0: 6f6e 6669 672c 206f 7220 6672 6f6d 2070  onfig, or from p
+0000e9c0: 7265 7620 6772 6170 6820 6372 6561 7469  rev graph creati
+0000e9d0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+0000e9e0: 2320 5468 6973 2069 7320 696d 706f 7274  # This is import
+0000e9f0: 616e 7420 7375 6368 2074 6861 7420 7365  ant such that se
+0000ea00: 6c66 2e63 616e 5f63 6f6d 7061 7265 2829  lf.can_compare()
+0000ea10: 2069 7320 7361 6e65 2e0a 2020 2020 2020   is sane..      
+0000ea20: 2020 2020 2020 6966 206f 7468 6572 5f73        if other_s
+0000ea30: 616d 655f 6261 7365 2e64 796e 5f73 697a  ame_base.dyn_siz
+0000ea40: 6520 6973 204e 6f6e 6520 6f72 206e 6f74  e is None or not
+0000ea50: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000ea60: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+0000ea70: 7272 656e 745f 6772 6170 6828 293a 0a20  rrent_graph():. 
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000ea90: 7468 6572 5f73 616d 655f 6261 7365 2e64  ther_same_base.d
+0000eaa0: 796e 5f73 697a 655f 6578 7420 3d20 7365  yn_size_ext = se
+0000eab0: 6c66 2e67 6574 5f64 796e 5f73 697a 655f  lf.get_dyn_size_
+0000eac0: 6578 745f 666f 725f 6261 7463 685f 6374  ext_for_batch_ct
+0000ead0: 7828 0a20 2020 2020 2020 2020 2020 2020  x(.             
+0000eae0: 2020 2020 2020 206f 7468 6572 5f73 616d         other_sam
+0000eaf0: 655f 6261 7365 2e62 6174 6368 2c20 6f74  e_base.batch, ot
+0000eb00: 6865 725f 7361 6d65 5f62 6173 652e 636f  her_same_base.co
+0000eb10: 6e74 726f 6c5f 666c 6f77 5f63 7478 2c20  ntrol_flow_ctx, 
+0000eb20: 7465 6d70 6c61 7465 5f6f 6e6c 793d 5472  template_only=Tr
+0000eb30: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+0000eb40: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000eb50: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
+0000eb60: 6261 7365 2e5f 6d61 7962 655f 7570 6461  base._maybe_upda
+0000eb70: 7465 2829 0a20 2020 2020 2020 2069 6620  te().        if 
+0000eb80: 6e6f 7420 7365 6c66 2e64 796e 5f73 697a  not self.dyn_siz
+0000eb90: 655f 6578 7420 6f72 206e 6f74 2073 656c  e_ext or not sel
+0000eba0: 662e 5f76 616c 6964 6174 655f 696e 5f63  f._validate_in_c
+0000ebb0: 7572 7265 6e74 5f67 7261 7068 2829 3a0a  urrent_graph():.
+0000ebc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ebd0: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
+0000ebe0: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000ebf0: 6765 745f 6479 6e5f 7369 7a65 5f65 7874  get_dyn_size_ext
+0000ec00: 5f66 6f72 5f62 6174 6368 5f63 7478 280a  _for_batch_ctx(.
+0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec20: 7365 6c66 2e62 6174 6368 2c20 7365 6c66  self.batch, self
+0000ec30: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+0000ec40: 782c 2074 656d 706c 6174 655f 6f6e 6c79  x, template_only
+0000ec50: 3d54 7275 650a 2020 2020 2020 2020 2020  =True.          
+0000ec60: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000ec70: 7365 6c66 2e5f 6d61 7962 655f 7570 6461  self._maybe_upda
+0000ec80: 7465 2829 0a20 2020 2020 2020 2065 6c69  te().        eli
+0000ec90: 6620 6f74 6865 725f 7361 6d65 5f62 6173  f other_same_bas
+0000eca0: 652e 6479 6e5f 7369 7a65 5f65 7874 2069  e.dyn_size_ext i
+0000ecb0: 7320 4e6f 6e65 206f 7220 6e6f 7420 6f74  s None or not ot
+0000ecc0: 6865 725f 7361 6d65 5f62 6173 652e 5f76  her_same_base._v
+0000ecd0: 616c 6964 6174 655f 696e 5f63 7572 7265  alidate_in_curre
+0000ece0: 6e74 5f67 7261 7068 2829 3a0a 2020 2020  nt_graph():.    
+0000ecf0: 2020 2020 2020 2020 6f74 6865 725f 7361          other_sa
+0000ed00: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
+0000ed10: 5f65 7874 203d 2073 656c 662e 6765 745f  _ext = self.get_
+0000ed20: 6479 6e5f 7369 7a65 5f65 7874 5f66 6f72  dyn_size_ext_for
+0000ed30: 5f62 6174 6368 5f63 7478 280a 2020 2020  _batch_ctx(.    
+0000ed40: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
+0000ed50: 725f 7361 6d65 5f62 6173 652e 6261 7463  r_same_base.batc
+0000ed60: 682c 206f 7468 6572 5f73 616d 655f 6261  h, other_same_ba
+0000ed70: 7365 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  se.control_flow_
+0000ed80: 6374 782c 2074 656d 706c 6174 655f 6f6e  ctx, template_on
+0000ed90: 6c79 3d54 7275 650a 2020 2020 2020 2020  ly=True.        
+0000eda0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000edb0: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
+0000edc0: 652e 5f6d 6179 6265 5f75 7064 6174 6528  e._maybe_update(
+0000edd0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000ede0: 662e 6973 5f64 696d 5f6b 6e6f 776e 2829  f.is_dim_known()
+0000edf0: 2061 6e64 206f 7468 6572 2e69 735f 6469   and other.is_di
+0000ee00: 6d5f 6b6e 6f77 6e28 293a 0a20 2020 2020  m_known():.     
+0000ee10: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+0000ee20: 6c66 2e64 696d 656e 7369 6f6e 203d 3d20  lf.dimension == 
+0000ee30: 6f74 6865 722e 6469 6d65 6e73 696f 6e0a  other.dimension.
+0000ee40: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+0000ee50: 662e 6973 5f64 696d 5f6b 6e6f 776e 2829  f.is_dim_known()
+0000ee60: 2061 6e64 206e 6f74 206f 7468 6572 2e69   and not other.i
+0000ee70: 735f 6469 6d5f 6b6e 6f77 6e28 293a 0a20  s_dim_known():. 
+0000ee80: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000ee90: 2e63 6170 6163 6974 7920 3d20 7365 6c66  .capacity = self
+0000eea0: 2e63 6170 6163 6974 790a 2020 2020 2020  .capacity.      
+0000eeb0: 2020 2020 2020 6f74 6865 722e 7369 7a65        other.size
+0000eec0: 203d 2073 656c 662e 7369 7a65 0a20 2020   = self.size.   
+0000eed0: 2020 2020 2065 6c69 6620 6e6f 7420 7365       elif not se
+0000eee0: 6c66 2e69 735f 6469 6d5f 6b6e 6f77 6e28  lf.is_dim_known(
+0000eef0: 2920 616e 6420 6f74 6865 722e 6973 5f64  ) and other.is_d
+0000ef00: 696d 5f6b 6e6f 776e 2829 3a0a 2020 2020  im_known():.    
+0000ef10: 2020 2020 2020 2020 7365 6c66 2e63 6170          self.cap
+0000ef20: 6163 6974 7920 3d20 6f74 6865 722e 6361  acity = other.ca
+0000ef30: 7061 6369 7479 0a20 2020 2020 2020 2020  pacity.         
+0000ef40: 2020 2073 656c 662e 7369 7a65 203d 206f     self.size = o
+0000ef50: 7468 6572 2e73 697a 650a 2020 2020 2020  ther.size.      
+0000ef60: 2020 6966 2073 656c 662e 766f 6361 6220    if self.vocab 
+0000ef70: 616e 6420 6e6f 7420 6f74 6865 725f 7361  and not other_sa
+0000ef80: 6d65 5f62 6173 652e 766f 6361 623a 0a20  me_base.vocab:. 
+0000ef90: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000efa0: 5f73 616d 655f 6261 7365 2e76 6f63 6162  _same_base.vocab
+0000efb0: 203d 2073 656c 662e 766f 6361 620a 2020   = self.vocab.  
+0000efc0: 2020 2020 2020 656c 6966 206f 7468 6572        elif other
+0000efd0: 5f73 616d 655f 6261 7365 2e76 6f63 6162  _same_base.vocab
+0000efe0: 2061 6e64 206e 6f74 2073 656c 662e 766f   and not self.vo
+0000eff0: 6361 623a 0a20 2020 2020 2020 2020 2020  cab:.           
+0000f000: 2073 656c 662e 766f 6361 6220 3d20 6f74   self.vocab = ot
+0000f010: 6865 725f 7361 6d65 5f62 6173 652e 766f  her_same_base.vo
+0000f020: 6361 620a 2020 2020 2020 2020 7365 6c66  cab.        self
+0000f030: 2e5f 6d61 6b65 5f65 7874 7261 2829 0a20  ._make_extra(). 
+0000f040: 2020 2020 2020 2073 656c 665f 7361 6d65         self_same
+0000f050: 5f61 732e 5f6d 616b 655f 6578 7472 6128  _as._make_extra(
+0000f060: 290a 2020 2020 2020 2020 2320 6e6f 696e  ).        # noin
+0000f070: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+0000f080: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+0000f090: 2020 2073 656c 662e 5f65 7874 7261 2e61     self._extra.a
+0000f0a0: 7574 6f5f 6765 6e65 7261 7465 6420 3d20  uto_generated = 
+0000f0b0: 7365 6c66 5f73 616d 655f 6173 2e5f 6578  self_same_as._ex
+0000f0c0: 7472 612e 6175 746f 5f67 656e 6572 6174  tra.auto_generat
+0000f0d0: 6564 203d 206f 7468 6572 5f73 616d 655f  ed = other_same_
+0000f0e0: 6261 7365 2e61 7574 6f5f 6765 6e65 7261  base.auto_genera
+0000f0f0: 7465 640a 2020 2020 2020 2020 2320 5461  ted.        # Ta
+0000f100: 6b65 206f 7665 7220 6465 7269 7665 645f  ke over derived_
+0000f110: 6672 6f6d 5f6f 702e 2048 6f77 6576 6572  from_op. However
+0000f120: 2c20 6f6e 6c79 2069 6620 7468 6973 2077  , only if this w
+0000f130: 6f75 6c64 206e 6f74 2069 6e74 726f 6475  ould not introdu
+0000f140: 6365 2063 7963 6c65 7321 0a20 2020 2020  ce cycles!.     
+0000f150: 2020 2069 6620 6e6f 7420 7365 6c66 5f64     if not self_d
+0000f160: 6572 6976 6564 5f62 6173 6573 2e69 7373  erived_bases.iss
+0000f170: 7570 6572 7365 7428 6f74 6865 725f 6465  uperset(other_de
+0000f180: 7269 7665 645f 6261 7365 7329 3a0a 2020  rived_bases):.  
+0000f190: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000f1a0: 662e 6465 7269 7665 645f 6672 6f6d 5f6f  f.derived_from_o
+0000f1b0: 7020 616e 6420 6e6f 7420 6f74 6865 725f  p and not other_
+0000f1c0: 7361 6d65 5f62 6173 652e 6465 7269 7665  same_base.derive
+0000f1d0: 645f 6672 6f6d 5f6f 703a 0a20 2020 2020  d_from_op:.     
+0000f1e0: 2020 2020 2020 2020 2020 2023 206e 6f69             # noi
+0000f1f0: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
+0000f200: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
+0000f210: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
+0000f220: 725f 7361 6d65 5f62 6173 652e 5f6d 616b  r_same_base._mak
+0000f230: 655f 6578 7472 6128 292e 6465 7269 7665  e_extra().derive
+0000f240: 645f 6672 6f6d 5f6f 7020 3d20 7365 6c66  d_from_op = self
+0000f250: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+0000f260: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000f270: 6620 6f74 6865 725f 7361 6d65 5f62 6173  f other_same_bas
+0000f280: 652e 6465 7269 7665 645f 6672 6f6d 5f6f  e.derived_from_o
+0000f290: 7020 616e 6420 6e6f 7420 7365 6c66 2e64  p and not self.d
+0000f2a0: 6572 6976 6564 5f66 726f 6d5f 6f70 3a0a  erived_from_op:.
+0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2c0: 7365 6c66 2e5f 6d61 6b65 5f65 7874 7261  self._make_extra
+0000f2d0: 2829 2e64 6572 6976 6564 5f66 726f 6d5f  ().derived_from_
+0000f2e0: 6f70 203d 206f 7468 6572 5f73 616d 655f  op = other_same_
+0000f2f0: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000f300: 6d5f 6f70 0a20 2020 2020 2020 2069 6620  m_op.        if 
+0000f310: 7365 6c66 2e5f 6578 7472 6120 616e 6420  self._extra and 
+0000f320: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
+0000f330: 6173 652e 6973 5f64 796e 616d 6963 2829  ase.is_dynamic()
+0000f340: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000f350: 5468 6f73 6520 6d69 6768 7420 6265 2073  Those might be s
+0000f360: 6574 2076 6961 2067 6574 5f62 6174 6368  et via get_batch
+0000f370: 5f66 6f72 5f63 7478 2066 6f72 2061 6e20  _for_ctx for an 
+0000f380: 756e 6465 6669 6e65 6420 6469 6d2c 0a20  undefined dim,. 
+0000f390: 2020 2020 2020 2020 2020 2023 2077 6869             # whi
+0000f3a0: 6368 206e 6f77 2062 6563 6f6d 6573 2073  ch now becomes s
+0000f3b0: 7461 7469 6320 6475 6520 746f 2060 6f74  tatic due to `ot
+0000f3c0: 6865 7260 2e0a 2020 2020 2020 2020 2020  her`..          
+0000f3d0: 2020 7365 6c66 2e5f 6578 7472 612e 6261    self._extra.ba
+0000f3e0: 7463 6820 3d20 4e6f 6e65 0a20 2020 2020  tch = None.     
+0000f3f0: 2020 2020 2020 2073 656c 662e 5f65 7874         self._ext
+0000f400: 7261 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  ra.control_flow_
+0000f410: 6374 7820 3d20 4e6f 6e65 0a20 2020 2020  ctx = None.     
+0000f420: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
+0000f430: 6469 6d5f 2069 6e20 7365 6c66 2e5f 6578  dim_ in self._ex
+0000f440: 7472 612e 7361 6d65 5f66 6f72 5f62 6174  tra.same_for_bat
+0000f450: 6368 5f63 7478 2e69 7465 6d73 2829 3a0a  ch_ctx.items():.
+0000f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f470: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+0000f480: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+0000f490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f4a0: 2064 696d 5f65 7874 7261 203d 2064 696d   dim_extra = dim
+0000f4b0: 5f2e 5f65 7874 7261 0a20 2020 2020 2020  _._extra.       
+0000f4c0: 2020 2020 2020 2020 2069 6620 6469 6d5f           if dim_
+0000f4d0: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
+0000f4e0: 2020 2020 2020 2020 2020 2064 696d 5f65             dim_e
+0000f4f0: 7874 7261 2e62 6174 6368 203d 204e 6f6e  xtra.batch = Non
+0000f500: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000f510: 2020 2020 2020 6469 6d5f 6578 7472 612e        dim_extra.
+0000f520: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+0000f530: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000f540: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
+0000f550: 2020 2020 2020 2020 2020 2073 656c 665f             self_
+0000f560: 203d 2073 656c 662e 6765 745f 666f 725f   = self.get_for_
+0000f570: 6261 7463 685f 6374 7828 6261 7463 683d  batch_ctx(batch=
+0000f580: 7365 6c66 2e62 6174 6368 2c20 6374 783d  self.batch, ctx=
+0000f590: 7365 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f  self.control_flo
+0000f5a0: 775f 6374 7829 0a20 2020 2020 2020 2020  w_ctx).         
+0000f5b0: 2020 2069 6620 7365 6c66 5f20 6973 206e     if self_ is n
+0000f5c0: 6f74 2073 656c 663a 0a20 2020 2020 2020  ot self:.       
+0000f5d0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000f5e0: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
+0000f5f0: 2073 656c 665f 2e63 6f6e 7472 6f6c 5f66   self_.control_f
+0000f600: 6c6f 775f 6374 7820 2023 206d 6967 6874  low_ctx  # might
+0000f610: 2062 6520 6469 6666 6572 656e 740a 2020   be different.  
+0000f620: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f630: 6c66 2e64 796e 5f73 697a 655f 6578 7420  lf.dyn_size_ext 
+0000f640: 3d20 7365 6c66 5f2e 6479 6e5f 7369 7a65  = self_.dyn_size
+0000f650: 5f65 7874 2020 2320 6d69 6768 7420 6265  _ext  # might be
+0000f660: 2075 6e73 6574 0a0a 2020 2020 6465 6620   unset..    def 
+0000f670: 5f6d 6572 6765 5f73 616d 655f 666f 725f  _merge_same_for_
+0000f680: 6261 7463 685f 6374 785f 6469 6374 2873  batch_ctx_dict(s
+0000f690: 656c 663a 205f 642e 4469 6d2c 206f 7468  elf: _d.Dim, oth
+0000f6a0: 6572 3a20 5f64 2e44 696d 293a 0a20 2020  er: _d.Dim):.   
+0000f6b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f6c0: 203a 7061 7261 6d20 6f74 6865 723a 0a20   :param other:. 
+0000f6d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000f6e0: 2020 2023 206e 6f69 6e73 7065 6374 696f     # noinspectio
+0000f6f0: 6e20 5079 5072 6f74 6563 7465 644d 656d  n PyProtectedMem
+0000f700: 6265 720a 2020 2020 2020 2020 6966 206e  ber.        if n
+0000f710: 6f74 2073 656c 662e 5f65 7874 7261 2061  ot self._extra a
+0000f720: 6e64 206e 6f74 206f 7468 6572 2e5f 6578  nd not other._ex
+0000f730: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
+0000f740: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000f750: 7365 6c66 2e5f 7661 6c69 6461 7465 5f69  self._validate_i
+0000f760: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+0000f770: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000f780: 662e 5f65 7874 7261 3a0a 2020 2020 2020  f._extra:.      
+0000f790: 2020 2020 2020 666f 7220 5f2c 2064 696d        for _, dim
+0000f7a0: 2069 6e20 6c69 7374 2873 656c 662e 5f65   in list(self._e
+0000f7b0: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
+0000f7c0: 7463 685f 6374 782e 6974 656d 7328 2929  tch_ctx.items())
+0000f7d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f7e0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+0000f7f0: 6e63 6528 6469 6d2c 205f 642e 4469 6d29  nce(dim, _d.Dim)
+0000f800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f810: 2064 696d 2e5f 7661 6c69 6461 7465 5f69   dim._validate_i
+0000f820: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+0000f830: 290a 2020 2020 2020 2020 2320 6e6f 696e  ).        # noin
+0000f840: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+0000f850: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+0000f860: 2020 2069 6620 6f74 6865 722e 5f65 7874     if other._ext
+0000f870: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
+0000f880: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+0000f890: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+0000f8a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000f8b0: 206b 6579 2c20 6469 6d20 696e 206f 7468   key, dim in oth
+0000f8c0: 6572 2e5f 6578 7472 612e 7361 6d65 5f66  er._extra.same_f
+0000f8d0: 6f72 5f62 6174 6368 5f63 7478 2e69 7465  or_batch_ctx.ite
+0000f8e0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+0000f8f0: 2020 2020 2020 6966 206e 6f74 2064 696d        if not dim
+0000f900: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+0000f910: 7272 656e 745f 6772 6170 6828 293a 0a20  rrent_graph():. 
+0000f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f930: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+0000f940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f950: 5f64 696d 203d 2073 656c 662e 5f6d 616b  _dim = self._mak
+0000f960: 655f 6578 7472 6128 292e 7361 6d65 5f66  e_extra().same_f
+0000f970: 6f72 5f62 6174 6368 5f63 7478 2e67 6574  or_batch_ctx.get
+0000f980: 286b 6579 2c20 4e6f 6e65 290a 2020 2020  (key, None).    
+0000f990: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000f9a0: 656c 665f 6469 6d20 616e 6420 2873 656c  elf_dim and (sel
+0000f9b0: 665f 6469 6d2e 6479 6e5f 7369 7a65 5f65  f_dim.dyn_size_e
+0000f9c0: 7874 206f 7220 6e6f 7420 6469 6d2e 6479  xt or not dim.dy
+0000f9d0: 6e5f 7369 7a65 5f65 7874 293a 0a20 2020  n_size_ext):.   
+0000f9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9f0: 2063 6f6e 7469 6e75 6520 2023 206b 6565   continue  # kee
+0000fa00: 7020 6f75 7273 0a20 2020 2020 2020 2020  p ours.         
+0000fa10: 2020 2020 2020 2069 6620 6e6f 7420 6469         if not di
+0000fa20: 6d2e 6479 6e5f 7369 7a65 5f65 7874 3a0a  m.dyn_size_ext:.
+0000fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa40: 2020 2020 636f 6e74 696e 7565 2020 2320      continue  # 
+0000fa50: 756e 6465 6669 6e65 642c 2064 6f20 6e6f  undefined, do no
+0000fa60: 7420 6f76 6572 7461 6b65 0a20 2020 2020  t overtake.     
+0000fa70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fa80: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000fa90: 6261 7463 685f 6374 785b 6b65 795d 203d  batch_ctx[key] =
+0000faa0: 2064 696d 0a20 2020 2020 2020 2020 2020   dim.           
+0000fab0: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
+0000fac0: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
+0000fad0: 720a 2020 2020 2020 2020 2020 2020 6f74  r.            ot
+0000fae0: 6865 722e 5f65 7874 7261 2e73 616d 655f  her._extra.same_
+0000faf0: 666f 725f 6261 7463 685f 6374 782e 636c  for_batch_ctx.cl
+0000fb00: 6561 7228 2920 2023 2077 6520 6f6e 6c79  ear()  # we only
+0000fb10: 2077 616e 7420 746f 2068 6176 6520 6974   want to have it
+0000fb20: 206f 6e63 650a 0a20 2020 2023 206e 6f69   once..    # noi
+0000fb30: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
+0000fb40: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
+0000fb50: 6465 6620 6465 7269 7665 5f66 726f 6d28  def derive_from(
+0000fb60: 7365 6c66 3a20 5f64 2e44 696d 2c20 6261  self: _d.Dim, ba
+0000fb70: 7365 3a20 5f64 2e44 696d 2c20 7365 745f  se: _d.Dim, set_
+0000fb80: 6465 7269 7665 645f 6672 6f6d 5f66 6c61  derived_from_fla
+0000fb90: 673a 2062 6f6f 6c20 3d20 5472 7565 293a  g: bool = True):
+0000fba0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000fbb0: 2020 2020 203a 7061 7261 6d20 6261 7365       :param base
+0000fbc0: 3a20 6469 6d0a 2020 2020 2020 2020 3a70  : dim.        :p
+0000fbd0: 6172 616d 2073 6574 5f64 6572 6976 6564  aram set_derived
+0000fbe0: 5f66 726f 6d5f 666c 6167 3a0a 2020 2020  _from_flag:.    
+0000fbf0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000fc00: 7365 6c66 5f62 6173 6520 3d20 7365 6c66  self_base = self
+0000fc10: 2e67 6574 5f73 616d 655f 6261 7365 2829  .get_same_base()
+0000fc20: 0a20 2020 2020 2020 2073 656c 665f 6261  .        self_ba
+0000fc30: 7365 5f65 7874 7261 203d 2073 656c 665f  se_extra = self_
+0000fc40: 6261 7365 2e5f 6d61 6b65 5f65 7874 7261  base._make_extra
+0000fc50: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0000fc60: 745f 6465 7269 7665 645f 6672 6f6d 5f66  t_derived_from_f
+0000fc70: 6c61 673a 0a20 2020 2020 2020 2020 2020  lag:.           
+0000fc80: 2069 6620 7365 6c66 5f62 6173 655f 6578   if self_base_ex
+0000fc90: 7472 612e 6465 7269 7665 645f 6672 6f6d  tra.derived_from
+0000fca0: 5f74 6167 3a0a 2020 2020 2020 2020 2020  _tag:.          
+0000fcb0: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+0000fcc0: 665f 6261 7365 5f65 7874 7261 2e64 6572  f_base_extra.der
+0000fcd0: 6976 6564 5f66 726f 6d5f 7461 6720 3d3d  ived_from_tag ==
+0000fce0: 2062 6173 650a 2020 2020 2020 2020 2020   base.          
+0000fcf0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000fd00: 2020 2020 2020 2020 7365 6c66 5f62 6173          self_bas
+0000fd10: 655f 6578 7472 612e 6465 7269 7665 645f  e_extra.derived_
+0000fd20: 6672 6f6d 5f74 6167 203d 2062 6173 650a  from_tag = base.
+0000fd30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000fd40: 6973 5f64 796e 616d 6963 2829 206f 7220  is_dynamic() or 
+0000fd50: 6e6f 7420 7365 6c66 2e69 735f 6469 6d5f  not self.is_dim_
+0000fd60: 6b6e 6f77 6e28 293a 0a20 2020 2020 2020  known():.       
+0000fd70: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0000fd80: 2e62 6174 6368 2061 6e64 2062 6173 652e  .batch and base.
+0000fd90: 6261 7463 683a 0a20 2020 2020 2020 2020  batch:.         
+0000fda0: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
+0000fdb0: 6820 3d20 6261 7365 2e62 6174 6368 0a20  h = base.batch. 
+0000fdc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fdd0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
+0000fde0: 5f63 7478 203d 2062 6173 652e 636f 6e74  _ctx = base.cont
+0000fdf0: 726f 6c5f 666c 6f77 5f63 7478 0a20 2020  rol_flow_ctx.   
+0000fe00: 2020 2020 2020 2020 2020 2020 206b 6579               key
+0000fe10: 203d 2062 6173 652e 6261 7463 682c 2062   = base.batch, b
+0000fe20: 6173 652e 636f 6e74 726f 6c5f 666c 6f77  ase.control_flow
+0000fe30: 5f63 7478 0a20 2020 2020 2020 2020 2020  _ctx.           
+0000fe40: 2020 2020 2061 7373 6572 7420 6b65 7920       assert key 
+0000fe50: 6e6f 7420 696e 2073 656c 665f 6261 7365  not in self_base
+0000fe60: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000fe70: 6261 7463 685f 6374 780a 2020 2020 2020  batch_ctx.      
+0000fe80: 2020 2020 2020 2020 2020 7365 6c66 5f62            self_b
+0000fe90: 6173 655f 6578 7472 612e 7361 6d65 5f66  ase_extra.same_f
+0000fea0: 6f72 5f62 6174 6368 5f63 7478 5b6b 6579  or_batch_ctx[key
+0000feb0: 5d20 3d20 7365 6c66 0a20 2020 2020 2020  ] = self.       
+0000fec0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0000fed0: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
+0000fee0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000fef0: 6620 6261 7365 2e64 796e 5f73 697a 655f  f base.dyn_size_
+0000ff00: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
+0000ff10: 2020 2020 2020 2020 2069 6620 6261 7365           if base
+0000ff20: 2e62 6174 6368 2061 6e64 2062 6173 652e  .batch and base.
+0000ff30: 6261 7463 6820 3d3d 2073 656c 662e 6261  batch == self.ba
+0000ff40: 7463 6820 616e 6420 6261 7365 2e63 6f6e  tch and base.con
+0000ff50: 7472 6f6c 5f66 6c6f 775f 6374 7820 3d3d  trol_flow_ctx ==
+0000ff60: 2073 656c 662e 636f 6e74 726f 6c5f 666c   self.control_fl
+0000ff70: 6f77 5f63 7478 3a0a 2020 2020 2020 2020  ow_ctx:.        
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+0000ffa0: 7420 3d20 6261 7365 2e64 796e 5f73 697a  t = base.dyn_siz
+0000ffb0: 655f 6578 742e 636f 7079 5f74 656d 706c  e_ext.copy_templ
+0000ffc0: 6174 6528 6e61 6d65 3d22 2573 3a73 697a  ate(name="%s:siz
+0000ffd0: 6522 2025 2073 656c 665f 6261 7365 2e64  e" % self_base.d
+0000ffe0: 6573 6372 6970 7469 6f6e 290a 2020 2020  escription).    
+0000fff0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00010000: 2062 6173 652e 6973 5f62 6174 6368 5f64   base.is_batch_d
+00010010: 696d 2829 3a0a 2020 2020 2020 2020 2020  im():.          
+00010020: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00010030: 796e 5f73 697a 655f 6578 7420 3d20 5f74  yn_size_ext = _t
+00010040: 2e54 656e 736f 7228 0a20 2020 2020 2020  .Tensor(.       
+00010050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010060: 206e 616d 653d 2225 733a 6261 7463 6822   name="%s:batch"
+00010070: 2025 2073 656c 665f 6261 7365 2e64 6573   % self_base.des
+00010080: 6372 6970 7469 6f6e 2c20 7368 6170 653d  cription, shape=
+00010090: 2829 2c20 6474 7970 653d 2269 6e74 3332  (), dtype="int32
+000100a0: 222c 2062 6174 6368 5f64 696d 5f61 7869  ", batch_dim_axi
+000100b0: 733d 4e6f 6e65 0a20 2020 2020 2020 2020  s=None.         
+000100c0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+000100d0: 2020 6465 6620 636f 7079 5f66 726f 6d28    def copy_from(
+000100e0: 7365 6c66 3a20 4469 6d2c 206f 7468 6572  self: Dim, other
+000100f0: 3a20 4469 6d29 3a0a 2020 2020 2020 2020  : Dim):.        
+00010100: 2222 2264 6566 696e 6522 2222 0a20 2020  """define""".   
+00010110: 2020 2020 2073 656c 662e 7369 7a65 203d       self.size =
+00010120: 206f 7468 6572 2e73 697a 650a 2020 2020   other.size.    
+00010130: 2020 2020 7365 6c66 2e63 6170 6163 6974      self.capacit
+00010140: 7920 3d20 6f74 6865 722e 6361 7061 6369  y = other.capaci
+00010150: 7479 0a20 2020 2020 2020 2073 656c 662e  ty.        self.
+00010160: 6479 6e5f 7369 7a65 5f65 7874 203d 206f  dyn_size_ext = o
+00010170: 7468 6572 2e64 796e 5f73 697a 655f 6578  ther.dyn_size_ex
+00010180: 740a 2020 2020 2020 2020 7365 6c66 2e64  t.        self.d
+00010190: 6572 6976 655f 6672 6f6d 286f 7468 6572  erive_from(other
+000101a0: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
+000101b0: 686f 640a 2020 2020 6465 6620 6765 745f  hod.    def get_
+000101c0: 6578 6973 7469 6e67 5f74 6167 5f66 726f  existing_tag_fro
+000101d0: 6d5f 636f 6c6c 6563 7469 6f6e 2863 6c73  m_collection(cls
+000101e0: 2c20 6f74 6865 722c 2074 6167 732c 2069  , other, tags, i
+000101f0: 735f 6571 7561 6c5f 6f70 7473 3d4e 6f6e  s_equal_opts=Non
+00010200: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+00010210: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
+00010220: 696d 206f 7468 6572 3a0a 2020 2020 2020  im other:.      
+00010230: 2020 3a70 6172 616d 206c 6973 745b 4469    :param list[Di
+00010240: 6d5d 7c74 7570 6c65 5b44 696d 5d7c 7365  m]|tuple[Dim]|se
+00010250: 745b 4469 6d5d 2074 6167 733a 0a20 2020  t[Dim] tags:.   
+00010260: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
+00010270: 5b73 7472 5d7c 4e6f 6e65 2069 735f 6571  [str]|None is_eq
+00010280: 7561 6c5f 6f70 7473 3a20 7061 7373 6564  ual_opts: passed
+00010290: 2074 6f20 4469 6d2e 6973 5f65 7175 616c   to Dim.is_equal
+000102a0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000102b0: 2044 696d 7c4e 6f6e 650a 2020 2020 2020   Dim|None.      
+000102c0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+000102d0: 2069 735f 6571 7561 6c5f 6f70 7473 2069   is_equal_opts i
+000102e0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000102f0: 2020 2020 6973 5f65 7175 616c 5f6f 7074      is_equal_opt
+00010300: 7320 3d20 7b7d 0a20 2020 2020 2020 2023  s = {}.        #
+00010310: 2057 6520 646f 2070 6f74 656e 7469 616c   We do potential
+00010320: 206d 756c 7469 706c 6520 726f 756e 6473   multiple rounds
+00010330: 2c20 7375 6368 2074 6861 7420 7765 2070  , such that we p
+00010340: 7265 6665 7220 226d 6f72 6520 6571 7561  refer "more equa
+00010350: 6c22 2028 7573 696e 6720 6c65 7373 2069  l" (using less i
+00010360: 735f 6571 7561 6c5f 6f70 7473 292e 0a20  s_equal_opts).. 
+00010370: 2020 2020 2020 2072 6f75 6e64 7320 3d20         rounds = 
+00010380: 5b7b 7d5d 0a20 2020 2020 2020 2069 6620  [{}].        if 
+00010390: 6973 5f65 7175 616c 5f6f 7074 733a 0a20  is_equal_opts:. 
+000103a0: 2020 2020 2020 2020 2020 2069 6620 2262             if "b
+000103b0: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
+000103c0: 2220 696e 2069 735f 6571 7561 6c5f 6f70  " in is_equal_op
+000103d0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+000103e0: 2020 2020 726f 756e 6473 2e61 7070 656e      rounds.appen
+000103f0: 6428 7b6b 3a20 7620 666f 7220 286b 2c20  d({k: v for (k, 
+00010400: 7629 2069 6e20 6973 5f65 7175 616c 5f6f  v) in is_equal_o
+00010410: 7074 732e 6974 656d 7328 2920 6966 206b  pts.items() if k
+00010420: 2021 3d20 2262 726f 6164 6361 7374 5f6d   != "broadcast_m
+00010430: 6174 6368 6573 227d 290a 2020 2020 2020  atches"}).      
+00010440: 2020 2020 2020 726f 756e 6473 2e61 7070        rounds.app
+00010450: 656e 6428 6973 5f65 7175 616c 5f6f 7074  end(is_equal_opt
+00010460: 7329 0a20 2020 2020 2020 2066 6f72 205f  s).        for _
+00010470: 6973 5f65 7175 616c 5f6f 7074 7320 696e  is_equal_opts in
+00010480: 2072 6f75 6e64 733a 0a20 2020 2020 2020   rounds:.       
+00010490: 2020 2020 2066 6f72 205f 7461 6720 696e       for _tag in
+000104a0: 2074 6167 733a 0a20 2020 2020 2020 2020   tags:.         
+000104b0: 2020 2020 2020 2069 6620 5f74 6167 2e69         if _tag.i
+000104c0: 735f 6571 7561 6c28 6f74 6865 722c 202a  s_equal(other, *
+000104d0: 2a5f 6973 5f65 7175 616c 5f6f 7074 7329  *_is_equal_opts)
+000104e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000104f0: 2020 2020 2020 7265 7475 726e 205f 7461        return _ta
+00010500: 670a 2020 2020 2020 2020 7265 7475 726e  g.        return
+00010510: 204e 6f6e 650a 0a20 2020 2040 636c 6173   None..    @clas
+00010520: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00010530: 6765 745f 616c 6c5f 6469 6d65 6e73 696f  get_all_dimensio
+00010540: 6e5f 7461 6773 2863 6c73 2c20 6461 7461  n_tags(cls, data
+00010550: 5f6c 6973 742c 2069 735f 6571 7561 6c5f  _list, is_equal_
+00010560: 6f70 7473 3d4e 6f6e 652c 2075 6e69 7175  opts=None, uniqu
+00010570: 655f 7365 7061 7261 7465 5f61 7865 733d  e_separate_axes=
+00010580: 5472 7565 293a 0a20 2020 2020 2020 2022  True):.        "
+00010590: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+000105a0: 6d20 6c69 7374 5b5f 742e 5465 6e73 6f72  m list[_t.Tensor
+000105b0: 5d20 6461 7461 5f6c 6973 743a 0a20 2020  ] data_list:.   
+000105c0: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
+000105d0: 5b73 7472 5d7c 4e6f 6e65 2069 735f 6571  [str]|None is_eq
+000105e0: 7561 6c5f 6f70 7473 3a20 7061 7373 6564  ual_opts: passed
+000105f0: 2074 6f20 4469 6d2e 6973 5f65 7175 616c   to Dim.is_equal
+00010600: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00010610: 626f 6f6c 2075 6e69 7175 655f 7365 7061  bool unique_sepa
+00010620: 7261 7465 5f61 7865 733a 2065 2e67 2e20  rate_axes: e.g. 
+00010630: 6461 7461 5f6c 6973 743d 5b44 6174 6120  data_list=[Data 
+00010640: 7769 7468 2073 6861 7065 2028 422c 352c  with shape (B,5,
+00010650: 352c 3130 295d 2072 6573 756c 7473 2069  5,10)] results i
+00010660: 6e20 3420 6469 6d20 7461 6773 2c20 6e6f  n 4 dim tags, no
+00010670: 7420 332e 0a20 2020 2020 2020 203a 7265  t 3..        :re
+00010680: 7475 726e 3a20 6c69 7374 206f 6620 6469  turn: list of di
+00010690: 6d65 6e73 696f 6e20 7461 6773 2c20 6469  mension tags, di
+000106a0: 6374 2066 6f72 2064 6174 6120 2d3e 206c  ct for data -> l
+000106b0: 6973 7420 6f66 2064 696d 656e 7369 6f6e  ist of dimension
+000106c0: 2074 6167 7320 2866 6f72 2065 6163 6820   tags (for each 
+000106d0: 6178 6973 290a 2020 2020 2020 2020 3a72  axis).        :r
+000106e0: 7479 7065 3a20 286c 6973 745b 4469 6d5d  type: (list[Dim]
+000106f0: 2c20 7574 696c 2e44 6963 7452 6566 4b65  , util.DictRefKe
+00010700: 7973 5b5f 742e 5465 6e73 6f72 2c20 6c69  ys[_t.Tensor, li
+00010710: 7374 5b44 696d 5d5d 290a 2020 2020 2020  st[Dim]]).      
+00010720: 2020 2222 220a 2020 2020 2020 2020 7461    """.        ta
+00010730: 6773 203d 205b 5d0a 2020 2020 2020 2020  gs = [].        
+00010740: 6461 7461 5f61 7865 735f 6469 6374 203d  data_axes_dict =
+00010750: 2075 7469 6c2e 4469 6374 5265 664b 6579   util.DictRefKey
+00010760: 7328 2920 2023 2074 7970 653a 2075 7469  s()  # type: uti
+00010770: 6c2e 4469 6374 5265 664b 6579 735b 5f74  l.DictRefKeys[_t
+00010780: 2e54 656e 736f 722c 204c 6973 745b 4469  .Tensor, List[Di
+00010790: 6d5d 5d0a 2020 2020 2020 2020 666f 7220  m]].        for 
+000107a0: 6461 7461 2069 6e20 6461 7461 5f6c 6973  data in data_lis
+000107b0: 743a 0a20 2020 2020 2020 2020 2020 2064  t:.            d
+000107c0: 6174 615f 6178 6573 5f64 6963 745b 6461  ata_axes_dict[da
+000107d0: 7461 5d20 3d20 5b5d 0a20 2020 2020 2020  ta] = [].       
+000107e0: 2020 2020 2065 7869 7374 696e 675f 7461       existing_ta
+000107f0: 675f 636f 6c6c 6563 7469 6f6e 5f66 6f72  g_collection_for
+00010800: 5f64 6174 6120 3d20 6c69 7374 2874 6167  _data = list(tag
+00010810: 7329 2069 6620 756e 6971 7565 5f73 6570  s) if unique_sep
+00010820: 6172 6174 655f 6178 6573 2065 6c73 6520  arate_axes else 
+00010830: 7461 6773 0a20 2020 2020 2020 2020 2020  tags.           
+00010840: 2066 6f72 2061 7869 7320 696e 2072 616e   for axis in ran
+00010850: 6765 2864 6174 612e 6261 7463 685f 6e64  ge(data.batch_nd
+00010860: 696d 293a 0a20 2020 2020 2020 2020 2020  im):.           
+00010870: 2020 2020 2074 6167 203d 2064 6174 612e       tag = data.
+00010880: 6765 745f 6469 6d5f 7461 6728 6178 6973  get_dim_tag(axis
+00010890: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000108a0: 2020 6578 6973 7469 6e67 5f74 6167 203d    existing_tag =
+000108b0: 2063 6c73 2e67 6574 5f65 7869 7374 696e   cls.get_existin
+000108c0: 675f 7461 675f 6672 6f6d 5f63 6f6c 6c65  g_tag_from_colle
+000108d0: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
+000108e0: 2020 2020 2020 2020 2020 2074 6167 2c20             tag, 
+000108f0: 7461 6773 3d65 7869 7374 696e 675f 7461  tags=existing_ta
+00010900: 675f 636f 6c6c 6563 7469 6f6e 5f66 6f72  g_collection_for
+00010910: 5f64 6174 612c 2069 735f 6571 7561 6c5f  _data, is_equal_
+00010920: 6f70 7473 3d69 735f 6571 7561 6c5f 6f70  opts=is_equal_op
+00010930: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+00010940: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00010950: 2020 2020 2069 6620 6578 6973 7469 6e67       if existing
+00010960: 5f74 6167 3a0a 2020 2020 2020 2020 2020  _tag:.          
+00010970: 2020 2020 2020 2020 2020 6966 2075 6e69            if uni
+00010980: 7175 655f 7365 7061 7261 7465 5f61 7865  que_separate_axe
+00010990: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000109a0: 2020 2020 2020 2020 2020 2065 7869 7374             exist
+000109b0: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
+000109c0: 6f6e 5f66 6f72 5f64 6174 612e 7265 6d6f  on_for_data.remo
+000109d0: 7665 2865 7869 7374 696e 675f 7461 6729  ve(existing_tag)
+000109e0: 2020 2320 646f 6e27 7420 7461 6b65 2069    # don't take i
+000109f0: 7420 6167 6169 6e20 666f 7220 7468 6973  t again for this
+00010a00: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
+00010a10: 2020 2020 2020 2020 2020 7265 706c 6163            replac
+00010a20: 655f 6578 6973 7469 6e67 203d 2028 0a20  e_existing = (. 
 00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a40: 6966 2072 6570 6c61 6365 5f65 7869 7374  if replace_exist
-00010a50: 696e 673a 2020 2320 5265 706c 6163 6520  ing:  # Replace 
-00010a60: 7468 6520 6578 6973 7469 6e67 2062 7920  the existing by 
-00010a70: 7468 6520 6e65 7720 7461 672e 0a20 2020  the new tag..   
-00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a90: 2020 2020 2074 6167 735b 7461 6773 2e69       tags[tags.i
-00010aa0: 6e64 6578 2865 7869 7374 696e 675f 7461  ndex(existing_ta
-00010ab0: 6729 5d20 3d20 7461 670a 2020 2020 2020  g)] = tag.      
-00010ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ad0: 2020 666f 7220 5f2c 2064 696d 735f 2069    for _, dims_ i
-00010ae0: 6e20 6461 7461 5f61 7865 735f 6469 6374  n data_axes_dict
-00010af0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b10: 2020 2020 2020 6469 6d73 5f5b 3a5d 203d        dims_[:] =
-00010b20: 205b 7461 6720 6966 2064 203d 3d20 6578   [tag if d == ex
-00010b30: 6973 7469 6e67 5f74 6167 2065 6c73 6520  isting_tag else 
-00010b40: 6420 666f 7220 6420 696e 2064 696d 735f  d for d in dims_
-00010b50: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00010b60: 2020 2020 2020 2020 2020 6578 6973 7469            existi
-00010b70: 6e67 5f74 6167 203d 2074 6167 0a20 2020  ng_tag = tag.   
-00010b80: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00010b90: 653a 2020 2320 6e6f 2065 7869 7374 696e  e:  # no existin
-00010ba0: 6720 7461 670a 2020 2020 2020 2020 2020  g tag.          
-00010bb0: 2020 2020 2020 2020 2020 7461 6773 2e61            tags.a
-00010bc0: 7070 656e 6428 7461 6729 0a20 2020 2020  ppend(tag).     
-00010bd0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00010be0: 6178 6573 5f64 6963 745b 6461 7461 5d2e  axes_dict[data].
-00010bf0: 6170 7065 6e64 2865 7869 7374 696e 675f  append(existing_
-00010c00: 7461 6720 6f72 2074 6167 290a 2020 2020  tag or tag).    
-00010c10: 2020 2020 7265 7475 726e 2074 6167 732c      return tags,
-00010c20: 2064 6174 615f 6178 6573 5f64 6963 740a   data_axes_dict.
-00010c30: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00010c40: 640a 2020 2020 6465 6620 6765 745f 756e  d.    def get_un
-00010c50: 6971 5f63 6f6c 6c65 6374 696f 6e28 636c  iq_collection(cl
-00010c60: 732c 2074 6167 732c 2069 735f 6571 7561  s, tags, is_equa
-00010c70: 6c5f 6f70 7473 3d4e 6f6e 6529 3a0a 2020  l_opts=None):.  
-00010c80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010c90: 2020 3a70 6172 616d 206c 6973 745b 4469    :param list[Di
-00010ca0: 6d5d 7c74 7570 6c65 5b44 696d 5d7c 7365  m]|tuple[Dim]|se
-00010cb0: 745b 4469 6d5d 2074 6167 733a 0a20 2020  t[Dim] tags:.   
-00010cc0: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
-00010cd0: 5b73 7472 5d7c 4e6f 6e65 2069 735f 6571  [str]|None is_eq
-00010ce0: 7561 6c5f 6f70 7473 3a20 7061 7373 6564  ual_opts: passed
-00010cf0: 2074 6f20 4469 6d2e 6973 5f65 7175 616c   to Dim.is_equal
-00010d00: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00010d10: 206c 6973 745b 4469 6d5d 0a20 2020 2020   list[Dim].     
-00010d20: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00010d30: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
-00010d40: 666f 7220 7461 6720 696e 2074 6167 733a  for tag in tags:
-00010d50: 0a20 2020 2020 2020 2020 2020 2065 7820  .            ex 
-00010d60: 3d20 636c 732e 6765 745f 6578 6973 7469  = cls.get_existi
-00010d70: 6e67 5f74 6167 5f66 726f 6d5f 636f 6c6c  ng_tag_from_coll
-00010d80: 6563 7469 6f6e 2874 6167 2c20 7265 732c  ection(tag, res,
-00010d90: 2069 735f 6571 7561 6c5f 6f70 7473 3d69   is_equal_opts=i
-00010da0: 735f 6571 7561 6c5f 6f70 7473 290a 2020  s_equal_opts).  
-00010db0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00010dc0: 2065 783a 0a20 2020 2020 2020 2020 2020   ex:.           
-00010dd0: 2020 2020 2072 6573 2e61 7070 656e 6428       res.append(
-00010de0: 7461 6729 0a20 2020 2020 2020 2072 6574  tag).        ret
-00010df0: 7572 6e20 7265 730a 0a20 2020 2064 6566  urn res..    def
-00010e00: 2067 6574 5f73 697a 655f 7465 6e73 6f72   get_size_tensor
-00010e10: 2873 656c 6629 202d 3e20 5f74 2e54 656e  (self) -> _t.Ten
-00010e20: 736f 723a 0a20 2020 2020 2020 2022 2222  sor:.        """
-00010e30: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00010e40: 3a20 7369 7a65 2074 656e 736f 722c 206f  : size tensor, o
-00010e50: 7220 6479 6e5f 7369 7a65 5f65 7874 2069  r dyn_size_ext i
-00010e60: 6620 6465 6669 6e65 640a 2020 2020 2020  f defined.      
-00010e70: 2020 3a72 7479 7065 3a20 5f74 2e54 656e    :rtype: _t.Ten
-00010e80: 736f 720a 2020 2020 2020 2020 2222 220a  sor.        """.
-00010e90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00010ea0: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
-00010eb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00010ec0: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00010ed0: 7874 0a0a 2020 2020 2020 2020 696d 706f  xt..        impo
-00010ee0: 7274 2072 6574 7572 6e6e 2e66 726f 6e74  rt returnn.front
-00010ef0: 656e 6420 6173 2072 660a 0a20 2020 2020  end as rf..     
-00010f00: 2020 2061 7373 6572 7420 7365 6c66 2e73     assert self.s
-00010f10: 697a 6520 6973 206e 6f74 204e 6f6e 650a  ize is not None.
-00010f20: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00010f30: 662e 636f 6e76 6572 745f 746f 5f74 656e  f.convert_to_ten
-00010f40: 736f 7228 7365 6c66 2e73 697a 652c 206e  sor(self.size, n
-00010f50: 616d 653d 2225 733a 7369 7a65 2220 2520  ame="%s:size" % 
-00010f60: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
-00010f70: 290a 0a20 2020 2064 6566 2067 6574 5f64  )..    def get_d
-00010f80: 696d 5f76 616c 7565 2873 656c 6629 202d  im_value(self) -
-00010f90: 3e20 556e 696f 6e5b 696e 742c 205f 742e  > Union[int, _t.
-00010fa0: 5261 7754 656e 736f 7254 7970 655d 3a0a  RawTensorType]:.
-00010fb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010fc0: 2020 2020 496e 6665 7273 2074 6865 2064      Infers the d
-00010fd0: 696d 2074 6869 7320 6178 6973 2073 686f  im this axis sho
-00010fe0: 756c 6420 6861 7665 2069 6620 756e 6272  uld have if unbr
-00010ff0: 6f61 6463 6173 7465 642e 0a20 2020 2020  oadcasted..     
-00011000: 2020 2049 6620 6073 656c 662e 7372 635f     If `self.src_
-00011010: 6461 7461 6020 6861 7320 6120 706c 6163  data` has a plac
-00011020: 6568 6f6c 6465 722c 2077 696c 6c20 7573  eholder, will us
-00011030: 6520 7468 6520 7368 6170 6520 6672 6f6d  e the shape from
-00011040: 2074 6865 7265 2e0a 2020 2020 2020 2020   there..        
-00011050: 4f74 6865 7277 6973 652c 2075 7365 7320  Otherwise, uses 
-00011060: 6073 656c 662e 6469 6d65 6e73 696f 6e60  `self.dimension`
-00011070: 2028 6966 2073 7461 7469 6329 206f 7220   (if static) or 
-00011080: 6073 656c 662e 6479 6e5f 7369 7a65 6020  `self.dyn_size` 
-00011090: 2869 6620 6479 6e61 6d69 6329 2e0a 0a20  (if dynamic)... 
-000110a0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-000110b0: 6d61 7828 7369 7a65 206f 7220 6479 6e5f  max(size or dyn_
-000110c0: 7369 7a65 290a 2020 2020 2020 2020 2222  size).        ""
-000110d0: 220a 2020 2020 2020 2020 7265 7320 3d20  ".        res = 
-000110e0: 7365 6c66 2e67 6574 5f64 696d 5f76 616c  self.get_dim_val
-000110f0: 7565 5f74 656e 736f 7228 290a 2020 2020  ue_tensor().    
-00011100: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00011110: 6528 7265 732c 205f 742e 5465 6e73 6f72  e(res, _t.Tensor
-00011120: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
-00011130: 7373 6572 7420 7265 732e 6469 6d73 203d  ssert res.dims =
-00011140: 3d20 2829 0a20 2020 2020 2020 2020 2020  = ().           
-00011150: 2072 6574 7572 6e20 7265 732e 7261 775f   return res.raw_
-00011160: 7465 6e73 6f72 0a20 2020 2020 2020 2061  tensor.        a
-00011170: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-00011180: 2872 6573 2c20 696e 7429 0a20 2020 2020  (res, int).     
-00011190: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
-000111a0: 2020 2064 6566 2067 6574 5f64 696d 5f76     def get_dim_v
-000111b0: 616c 7565 5f74 656e 736f 7228 7365 6c66  alue_tensor(self
-000111c0: 2920 2d3e 2055 6e69 6f6e 5b69 6e74 2c20  ) -> Union[int, 
-000111d0: 5f74 2e54 656e 736f 725d 3a0a 2020 2020  _t.Tensor]:.    
-000111e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000111f0: 496e 6665 7273 2074 6865 2064 696d 2074  Infers the dim t
-00011200: 6869 7320 6178 6973 2073 686f 756c 6420  his axis should 
-00011210: 6861 7665 2069 6620 756e 6272 6f61 6463  have if unbroadc
-00011220: 6173 7465 642e 0a20 2020 2020 2020 2049  asted..        I
-00011230: 6620 6073 656c 662e 7372 635f 6461 7461  f `self.src_data
-00011240: 6020 6861 7320 6120 706c 6163 6568 6f6c  ` has a placehol
-00011250: 6465 722c 2077 696c 6c20 7573 6520 7468  der, will use th
-00011260: 6520 7368 6170 6520 6672 6f6d 2074 6865  e shape from the
-00011270: 7265 2e0a 2020 2020 2020 2020 4f74 6865  re..        Othe
-00011280: 7277 6973 652c 2075 7365 7320 6073 656c  rwise, uses `sel
-00011290: 662e 6469 6d65 6e73 696f 6e60 2028 6966  f.dimension` (if
-000112a0: 2073 7461 7469 6329 206f 7220 6073 656c   static) or `sel
-000112b0: 662e 6479 6e5f 7369 7a65 6020 2869 6620  f.dyn_size` (if 
-000112c0: 6479 6e61 6d69 6329 2e0a 0a20 2020 2020  dynamic)...     
-000112d0: 2020 203a 7265 7475 726e 3a20 6d61 7828     :return: max(
-000112e0: 7369 7a65 206f 7220 6479 6e5f 7369 7a65  size or dyn_size
-000112f0: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-00011300: 2020 2020 2020 696d 706f 7274 2072 6574        import ret
-00011310: 7572 6e6e 2e66 726f 6e74 656e 6420 6173  urnn.frontend as
-00011320: 2072 660a 0a20 2020 2020 2020 2069 6620   rf..        if 
-00011330: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
-00011340: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011350: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00011360: 656c 662e 6469 6d65 6e73 696f 6e0a 2020  elf.dimension.  
-00011370: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
-00011380: 6e5f 7369 7a65 5f65 7874 2061 6e64 2073  n_size_ext and s
-00011390: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-000113a0: 2e70 6c61 6365 686f 6c64 6572 2069 7320  .placeholder is 
-000113b0: 6e6f 7420 4e6f 6e65 3a20 2023 2066 6173  not None:  # fas
-000113c0: 7420 7061 7468 0a20 2020 2020 2020 2020  t path.         
-000113d0: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
-000113e0: 697a 655f 6578 742e 6261 7463 685f 6e64  ize_ext.batch_nd
-000113f0: 696d 203e 2030 3a0a 2020 2020 2020 2020  im > 0:.        
-00011400: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00011410: 662e 7265 6475 6365 5f6d 6178 280a 2020  f.reduce_max(.  
-00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011430: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
-00011440: 6578 742c 0a20 2020 2020 2020 2020 2020  ext,.           
-00011450: 2020 2020 2020 2020 2061 7869 733d 7365           axis=se
-00011460: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00011470: 6469 6d5f 7461 6773 2c0a 2020 2020 2020  dim_tags,.      
-00011480: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00011490: 4d61 736b 696e 6720 6973 206e 6f74 2061  Masking is not a
-000114a0: 6c77 6179 7320 706f 7373 6962 6c65 2068  lways possible h
-000114b0: 6572 652c 2065 2e67 2e0a 2020 2020 2020  ere, e.g..      
-000114c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000114d0: 7365 6c66 203d 2044 696d 7b27 7365 6c66  self = Dim{'self
-000114e0: 2d61 7474 2d6b 6579 7327 5b27 7469 6d65  -att-keys'['time
-000114f0: 3a76 6172 3a65 7874 6572 6e5f 6461 7461  :var:extern_data
-00011500: 3a63 6c61 7373 6573 275b 425d 5d7d 2e0a  :classes'[B]]}..
-00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011520: 2020 2020 7573 655f 6d61 736b 3d46 616c      use_mask=Fal
-00011530: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00011540: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00011550: 2020 7265 7475 726e 2073 656c 662e 6479    return self.dy
-00011560: 6e5f 7369 7a65 5f65 7874 0a20 2020 2020  n_size_ext.     
-00011570: 2020 2069 6620 7365 6c66 2e69 735f 6261     if self.is_ba
-00011580: 7463 685f 6469 6d28 293a 0a20 2020 2020  tch_dim():.     
-00011590: 2020 2020 2020 2072 6573 203d 204e 6f6e         res = Non
-000115a0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-000115b0: 2073 656c 662e 5f65 7874 7261 2061 6e64   self._extra and
-000115c0: 2073 656c 662e 5f65 7874 7261 2e73 7263   self._extra.src
-000115d0: 5f64 6174 613a 0a20 2020 2020 2020 2020  _data:.         
-000115e0: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-000115f0: 662e 5f65 7874 7261 2e73 7263 5f64 6174  f._extra.src_dat
-00011600: 612e 6765 745f 6261 7463 685f 6469 6d28  a.get_batch_dim(
-00011610: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00011620: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
-00011630: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011640: 6573 203d 2073 656c 662e 6261 7463 682e  es = self.batch.
-00011650: 6469 6d0a 2020 2020 2020 2020 2020 2020  dim.            
-00011660: 6966 2069 7369 6e73 7461 6e63 6528 7265  if isinstance(re
-00011670: 732c 2069 6e74 293a 0a20 2020 2020 2020  s, int):.       
-00011680: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00011690: 7265 730a 2020 2020 2020 2020 2020 2020  res.            
-000116a0: 6966 2072 6573 2069 7320 6e6f 7420 4e6f  if res is not No
-000116b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000116c0: 2020 2020 7265 7475 726e 205f 742e 5465      return _t.Te
-000116d0: 6e73 6f72 2822 6261 7463 6822 2c20 6469  nsor("batch", di
-000116e0: 6d73 3d28 292c 2064 7479 7065 3d72 662e  ms=(), dtype=rf.
-000116f0: 6765 745f 6465 6661 756c 745f 6172 7261  get_default_arra
-00011700: 795f 696e 6465 785f 6474 7970 6528 292c  y_index_dtype(),
-00011710: 2072 6177 5f74 656e 736f 723d 7265 7329   raw_tensor=res)
-00011720: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
-00011730: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00011740: 6578 7472 610a 2020 2020 2020 2020 2020  extra.          
-00011750: 2020 616e 6420 7365 6c66 2e5f 6578 7472    and self._extr
-00011760: 612e 7372 635f 6461 7461 2069 7320 6e6f  a.src_data is no
-00011770: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
-00011780: 2020 2061 6e64 2073 656c 662e 5f65 7874     and self._ext
-00011790: 7261 2e73 7263 5f61 7869 7320 6973 206e  ra.src_axis is n
-000117a0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-000117b0: 2020 2020 616e 6420 7365 6c66 2e5f 6578      and self._ex
-000117c0: 7472 612e 7372 635f 6461 7461 2e70 6c61  tra.src_data.pla
-000117d0: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
-000117e0: 4e6f 6e65 0a20 2020 2020 2020 2029 3a0a  None.        ):.
-000117f0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-00011800: 3d20 7365 6c66 2e5f 6578 7472 612e 7372  = self._extra.sr
-00011810: 635f 6461 7461 2e67 6574 5f64 696d 2873  c_data.get_dim(s
-00011820: 656c 662e 5f65 7874 7261 2e73 7263 5f61  elf._extra.src_a
-00011830: 7869 7329 0a20 2020 2020 2020 2020 2020  xis).           
-00011840: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
-00011850: 6573 2c20 696e 7429 3a0a 2020 2020 2020  es, int):.      
-00011860: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011870: 2072 6573 0a20 2020 2020 2020 2020 2020   res.           
-00011880: 2072 6574 7572 6e20 5f74 2e54 656e 736f   return _t.Tenso
-00011890: 7228 2262 6174 6368 222c 2064 696d 733d  r("batch", dims=
-000118a0: 2829 2c20 6474 7970 653d 7266 2e67 6574  (), dtype=rf.get
-000118b0: 5f64 6566 6175 6c74 5f61 7272 6179 5f69  _default_array_i
-000118c0: 6e64 6578 5f64 7479 7065 2829 2c20 7261  ndex_dtype(), ra
-000118d0: 775f 7465 6e73 6f72 3d72 6573 290a 2020  w_tensor=res).  
-000118e0: 2020 2020 2020 7365 6c66 2e63 6f6d 706c        self.compl
-000118f0: 6574 655f 6479 6e5f 7369 7a65 2829 0a20  ete_dyn_size(). 
-00011900: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00011910: 796e 5f73 697a 655f 6578 7420 616e 6420  yn_size_ext and 
-00011920: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00011930: 742e 706c 6163 6568 6f6c 6465 7220 6973  t.placeholder is
-00011940: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00011950: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00011960: 796e 5f73 697a 655f 6578 742e 6261 7463  yn_size_ext.batc
-00011970: 685f 6e64 696d 203e 2030 3a0a 2020 2020  h_ndim > 0:.    
-00011980: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011990: 726e 2072 662e 7265 6475 6365 5f6d 6178  rn rf.reduce_max
-000119a0: 2873 656c 662e 6479 6e5f 7369 7a65 5f65  (self.dyn_size_e
-000119b0: 7874 2c20 6178 6973 3d73 656c 662e 6479  xt, axis=self.dy
-000119c0: 6e5f 7369 7a65 5f65 7874 2e64 696d 5f74  n_size_ext.dim_t
-000119d0: 6167 7329 0a20 2020 2020 2020 2020 2020  ags).           
-000119e0: 2072 6574 7572 6e20 7365 6c66 2e64 796e   return self.dyn
-000119f0: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
-00011a00: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00011a10: 6e28 2225 733a 206e 6565 6420 706c 6163  n("%s: need plac
-00011a20: 6568 6f6c 6465 722c 2073 656c 662e 6469  eholder, self.di
-00011a30: 6d65 6e73 696f 6e20 6f72 2073 656c 662e  mension or self.
-00011a40: 6479 6e5f 7369 7a65 2066 6f72 2064 696d  dyn_size for dim
-00011a50: 2076 616c 7565 2220 2520 7365 6c66 290a   value" % self).
-00011a60: 0a20 2020 2064 6566 2061 7869 735f 7370  .    def axis_sp
-00011a70: 6c69 745f 696e 666f 2873 656c 6629 3a0a  lit_info(self):.
-00011a80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011a90: 2020 2020 3a72 6574 7572 6e3a 2061 7869      :return: axi
-00011aa0: 7320 7370 6c69 7420 696e 666f 2e20 7365  s split info. se
-00011ab0: 6520 3a66 756e 633a 6067 6574 5f70 6172  e :func:`get_par
-00011ac0: 616d 5f61 7865 735f 7370 6c69 745f 696e  am_axes_split_in
-00011ad0: 666f 6020 616e 6420 7573 6167 6520 2865  fo` and usage (e
-00011ae0: 2e67 2e20 7072 6574 7261 696e 696e 6729  .g. pretraining)
-00011af0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00011b00: 206c 6973 745b 696e 747c 4e6f 6e65 5d0a   list[int|None].
-00011b10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011b20: 2020 2020 7361 6d65 5f62 6173 6520 3d20      same_base = 
-00011b30: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
-00011b40: 7365 2829 0a20 2020 2020 2020 206f 7020  se().        op 
-00011b50: 3d20 7365 6c66 2e64 6572 6976 6564 5f66  = self.derived_f
-00011b60: 726f 6d5f 6f70 206f 7220 7361 6d65 5f62  rom_op or same_b
-00011b70: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
-00011b80: 5f6f 700a 2020 2020 2020 2020 6966 206e  _op.        if n
-00011b90: 6f74 206f 703a 0a20 2020 2020 2020 2020  ot op:.         
-00011ba0: 2020 2072 6574 7572 6e20 5b73 656c 662e     return [self.
-00011bb0: 6469 6d65 6e73 696f 6e5d 0a20 2020 2020  dimension].     
-00011bc0: 2020 2069 6620 6f70 2e6b 696e 6420 3d3d     if op.kind ==
-00011bd0: 2022 6164 6422 3a0a 2020 2020 2020 2020   "add":.        
-00011be0: 2020 2020 7265 7475 726e 2073 756d 285b      return sum([
-00011bf0: 782e 6178 6973 5f73 706c 6974 5f69 6e66  x.axis_split_inf
-00011c00: 6f28 2920 666f 7220 7820 696e 206f 702e  o() for x in op.
-00011c10: 696e 7075 7473 5d2c 205b 5d29 2020 2320  inputs], [])  # 
-00011c20: 666c 6174 7465 6e0a 2020 2020 2020 2020  flatten.        
-00011c30: 6966 206f 702e 6b69 6e64 203d 3d20 226d  if op.kind == "m
-00011c40: 756c 223a 0a20 2020 2020 2020 2020 2020  ul":.           
-00011c50: 2072 6573 203d 205b 315d 0a20 2020 2020   res = [1].     
-00011c60: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
-00011c70: 6f70 2e69 6e70 7574 733a 0a20 2020 2020  op.inputs:.     
-00011c80: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00011c90: 2073 756d 285b 6e20 2a20 782e 6178 6973   sum([n * x.axis
-00011ca0: 5f73 706c 6974 5f69 6e66 6f28 2920 6966  _split_info() if
-00011cb0: 206e 2069 7320 6e6f 7420 4e6f 6e65 2065   n is not None e
-00011cc0: 6c73 6520 4e6f 6e65 2066 6f72 206e 2069  lse None for n i
-00011cd0: 6e20 7265 735d 2c20 5b5d 2920 2023 2066  n res], [])  # f
-00011ce0: 6c61 7474 656e 0a20 2020 2020 2020 2020  latten.         
-00011cf0: 2020 2072 6574 7572 6e20 7265 730a 2020     return res.  
-00011d00: 2020 2020 2020 7265 7475 726e 205b 7365        return [se
-00011d10: 6c66 2e64 696d 656e 7369 6f6e 5d0a 0a20  lf.dimension].. 
-00011d20: 2020 2064 6566 205f 6765 745f 7361 6d65     def _get_same
-00011d30: 5f62 6173 655f 6578 7472 6128 7365 6c66  _base_extra(self
-00011d40: 2920 2d3e 204f 7074 696f 6e61 6c5b 5f44  ) -> Optional[_D
-00011d50: 696d 4578 7472 615d 3a0a 2020 2020 2020  imExtra]:.      
-00011d60: 2020 6966 206e 6f74 2073 656c 662e 5f65    if not self._e
-00011d70: 7874 7261 3a0a 2020 2020 2020 2020 2020  xtra:.          
-00011d80: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00011d90: 2020 2020 2020 6261 7365 203d 2073 656c        base = sel
-00011da0: 662e 6765 745f 7361 6d65 5f62 6173 6528  f.get_same_base(
-00011db0: 290a 2020 2020 2020 2020 2320 6e6f 696e  ).        # noin
-00011dc0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-00011dd0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-00011de0: 2020 2072 6574 7572 6e20 6261 7365 2e5f     return base._
-00011df0: 6578 7472 610a 0a20 2020 2064 6566 205f  extra..    def _
-00011e00: 6d61 6b65 5f65 7874 7261 2873 656c 663a  make_extra(self:
-00011e10: 205f 642e 4469 6d29 202d 3e20 5f44 696d   _d.Dim) -> _Dim
-00011e20: 4578 7472 613a 0a20 2020 2020 2020 2069  Extra:.        i
-00011e30: 6620 6e6f 7420 7365 6c66 2e5f 6578 7472  f not self._extr
-00011e40: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
-00011e50: 656c 662e 5f65 7874 7261 203d 205f 4469  elf._extra = _Di
-00011e60: 6d45 7874 7261 2864 696d 3d73 656c 6629  mExtra(dim=self)
-00011e70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011e80: 7365 6c66 2e5f 6578 7472 610a 0a20 2020  self._extra..   
-00011e90: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00011ea0: 6566 2076 6f63 6162 2873 656c 6629 3a0a  ef vocab(self):.
-00011eb0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011ec0: 2020 2020 3a72 7479 7065 3a20 7265 7475      :rtype: retu
-00011ed0: 726e 6e2e 6461 7461 7365 7473 2e75 7469  rnn.datasets.uti
-00011ee0: 6c2e 766f 6361 6275 6c61 7279 2e56 6f63  l.vocabulary.Voc
-00011ef0: 6162 756c 6172 797c 4e6f 6e65 0a20 2020  abulary|None.   
-00011f00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011f10: 2065 7874 7261 203d 2073 656c 662e 5f67   extra = self._g
-00011f20: 6574 5f73 616d 655f 6261 7365 5f65 7874  et_same_base_ext
-00011f30: 7261 2829 0a20 2020 2020 2020 2069 6620  ra().        if 
-00011f40: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
-00011f50: 2020 2072 6574 7572 6e20 6578 7472 612e     return extra.
-00011f60: 766f 6361 620a 2020 2020 2020 2020 7265  vocab.        re
-00011f70: 7475 726e 204e 6f6e 650a 0a20 2020 2040  turn None..    @
-00011f80: 766f 6361 622e 7365 7474 6572 0a20 2020  vocab.setter.   
-00011f90: 2064 6566 2076 6f63 6162 2873 656c 662c   def vocab(self,
-00011fa0: 2076 6f63 6162 293a 0a20 2020 2020 2020   vocab):.       
-00011fb0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00011fc0: 7261 6d20 7265 7475 726e 6e2e 6461 7461  ram returnn.data
-00011fd0: 7365 7473 2e75 7469 6c2e 766f 6361 6275  sets.util.vocabu
-00011fe0: 6c61 7279 2e56 6f63 6162 756c 6172 797c  lary.Vocabulary|
-00011ff0: 4e6f 6e65 2076 6f63 6162 3a0a 2020 2020  None vocab:.    
-00012000: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012010: 6966 2076 6f63 6162 2069 7320 7365 6c66  if vocab is self
-00012020: 2e76 6f63 6162 3a0a 2020 2020 2020 2020  .vocab:.        
-00012030: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00012040: 2020 2069 6620 7365 6c66 2e73 616d 655f     if self.same_
-00012050: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
-00012060: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
-00012070: 7365 2829 2e76 6f63 6162 203d 2076 6f63  se().vocab = voc
-00012080: 6162 0a20 2020 2020 2020 2020 2020 2072  ab.            r
-00012090: 6574 7572 6e0a 2020 2020 2020 2020 6578  eturn.        ex
-000120a0: 7472 6120 3d20 7365 6c66 2e5f 6765 745f  tra = self._get_
-000120b0: 7361 6d65 5f62 6173 655f 6578 7472 6128  same_base_extra(
-000120c0: 290a 2020 2020 2020 2020 6966 2065 7874  ).        if ext
-000120d0: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
-000120e0: 6578 7472 612e 766f 6361 6220 3d20 766f  extra.vocab = vo
-000120f0: 6361 620a 0a20 2020 2023 2054 6865 206b  cab..    # The k
-00012100: 696e 6420 6f66 206f 7065 7261 7469 6f6e  ind of operation
-00012110: 7320 7765 2068 6176 653a 0a20 2020 2023  s we have:.    #
-00012120: 2061 202b 2062 3a20 7061 6464 696e 672c   a + b: padding,
-00012130: 2063 6f6e 6361 740a 2020 2020 2320 6120   concat.    # a 
-00012140: 2d20 623a 2077 696e 646f 7720 7769 7468  - b: window with
-00012150: 2076 616c 6964 2066 7261 6d65 7320 6f6e   valid frames on
-00012160: 6c79 0a20 2020 2023 2061 202a 2062 3a20  ly.    # a * b: 
-00012170: 6d65 7267 6520 6469 6d73 2c20 7570 7361  merge dims, upsa
-00012180: 6d70 6c65 2c20 7472 616e 7370 6f73 6564  mple, transposed
-00012190: 2063 6f6e 7620 7769 7468 2073 7472 6964   conv with strid
-000121a0: 696e 670a 2020 2020 2320 6120 2f20 6220  ing.    # a / b 
-000121b0: 2877 6865 6e20 6120 2520 6220 3d3d 2030  (when a % b == 0
-000121c0: 293a 2073 706c 6974 2064 696d 732c 2064  ): split dims, d
-000121d0: 6f77 6e73 616d 706c 652c 2063 6f6e 7620  ownsample, conv 
-000121e0: 7769 7468 2073 7472 6964 696e 670a 2020  with striding.  
-000121f0: 2020 2320 6365 696c 6469 7628 612c 2062    # ceildiv(a, b
-00012200: 293a 2063 6f6e 7620 7769 7468 2073 7472  ): conv with str
-00012210: 6964 696e 670a 2020 2020 2320 6375 7374  iding.    # cust
-00012220: 6f6d 3a20 7265 7065 6174 2c20 7265 6d6f  om: repeat, remo
-00012230: 7665 2c20 6d61 736b 2c20 6c6f 6f70 2077  ve, mask, loop w
-00012240: 6974 6820 6479 6e20 656e 640a 2020 2020  ith dyn end.    
-00012250: 2320 4e6f 7465 2074 6861 7420 7765 2064  # Note that we d
-00012260: 6966 6665 7265 6e74 6961 7465 2062 6574  ifferentiate bet
-00012270: 7765 656e 2074 6865 206f 7264 6572 2c20  ween the order, 
-00012280: 692e 652e 2061 202b 2062 2021 3d20 6220  i.e. a + b != b 
-00012290: 2b20 612e 0a20 2020 2023 204e 6f74 6520  + a..    # Note 
-000122a0: 7468 6174 2077 6520 616c 7761 7973 2068  that we always h
-000122b0: 6176 6520 7468 6520 6173 7375 6d70 7469  ave the assumpti
-000122c0: 6f6e 2074 6861 7420 6120 6469 6d65 6e73  on that a dimens
-000122d0: 696f 6e20 6973 206e 6f6e 2d6e 6567 6174  ion is non-negat
-000122e0: 6976 652e 0a20 2020 2023 2054 6869 7320  ive..    # This 
-000122f0: 6173 7375 6d70 7469 6f6e 2069 7320 6e65  assumption is ne
-00012300: 6365 7373 6172 7920 666f 7220 736f 6d65  cessary for some
-00012310: 2073 696d 706c 6966 6963 6174 696f 6e73   simplifications
-00012320: 2e0a 2020 2020 2320 6874 7470 733a 2f2f  ..    # https://
-00012330: 6769 7468 7562 2e63 6f6d 2f72 7774 682d  github.com/rwth-
-00012340: 6936 2f72 6574 7572 6e6e 2f70 756c 6c2f  i6/returnn/pull/
-00012350: 3835 330a 0a20 2020 2064 6566 205f 5f61  853..    def __a
-00012360: 6464 5f5f 2873 656c 663a 2044 696d 2c20  dd__(self: Dim, 
-00012370: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-00012380: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-00012390: 616d 2044 696d 7c69 6e74 206f 7468 6572  am Dim|int other
-000123a0: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
-000123b0: 6e3a 2073 656c 6620 2b20 6f74 6865 722e  n: self + other.
-000123c0: 206e 6f74 6520 7468 6174 2074 6869 7320   note that this 
-000123d0: 6973 206e 6f74 2063 6f6d 6d75 7461 7469  is not commutati
-000123e0: 7665 2c20 692e 652e 2064 6966 6665 7265  ve, i.e. differe
-000123f0: 6e74 2066 726f 6d20 6f74 6865 7220 2b20  nt from other + 
-00012400: 7365 6c66 2e0a 2020 2020 2020 2020 3a72  self..        :r
-00012410: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
-00012420: 2020 2222 220a 2020 2020 2020 2020 7465    """.        te
-00012430: 726d 203d 205f 4f70 4c69 6e65 6172 5465  rm = _OpLinearTe
-00012440: 726d 2e66 726f 6d5f 6469 6d28 7365 6c66  rm.from_dim(self
-00012450: 290a 2020 2020 2020 2020 7465 726d 2e65  ).        term.e
-00012460: 7874 656e 645f 6164 645f 7375 625f 286f  xtend_add_sub_(o
-00012470: 7468 6572 2c20 6b69 6e64 3d22 6164 6422  ther, kind="add"
-00012480: 2c20 7269 6768 743d 5472 7565 290a 2020  , right=True).  
-00012490: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-000124a0: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
-000124b0: 6465 6620 5f5f 7261 6464 5f5f 2873 656c  def __radd__(sel
-000124c0: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
-000124d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000124e0: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
-000124f0: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
-00012500: 2020 3a72 6574 7572 6e3a 206f 7468 6572    :return: other
-00012510: 202b 2073 656c 660a 2020 2020 2020 2020   + self.        
-00012520: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
-00012530: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012540: 7465 726d 203d 205f 4f70 4c69 6e65 6172  term = _OpLinear
-00012550: 5465 726d 2e66 726f 6d5f 6469 6d28 7365  Term.from_dim(se
-00012560: 6c66 290a 2020 2020 2020 2020 7465 726d  lf).        term
-00012570: 2e65 7874 656e 645f 6164 645f 7375 625f  .extend_add_sub_
-00012580: 286f 7468 6572 2c20 6b69 6e64 3d22 6164  (other, kind="ad
-00012590: 6422 2c20 7269 6768 743d 4661 6c73 6529  d", right=False)
-000125a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000125b0: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
-000125c0: 2020 2064 6566 205f 5f73 7562 5f5f 2873     def __sub__(s
-000125d0: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-000125e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000125f0: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-00012600: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00012610: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00012620: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00012630: 6574 7572 6e20 7365 6c66 2e73 7562 5f72  eturn self.sub_r
-00012640: 6967 6874 286f 7468 6572 290a 0a20 2020  ight(other)..   
-00012650: 2064 6566 2073 7562 5f72 6967 6874 2873   def sub_right(s
-00012660: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
-00012670: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00012680: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00012690: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
-000126a0: 2020 2020 3a72 6574 7572 6e3a 2073 656c      :return: sel
-000126b0: 6620 2d20 6f74 6865 720a 2020 2020 2020  f - other.      
-000126c0: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
-000126d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000126e0: 2020 7465 726d 203d 205f 4f70 4c69 6e65    term = _OpLine
-000126f0: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
-00012700: 7365 6c66 290a 2020 2020 2020 2020 7465  self).        te
-00012710: 726d 2e65 7874 656e 645f 6164 645f 7375  rm.extend_add_su
-00012720: 625f 286f 7468 6572 2c20 6b69 6e64 3d22  b_(other, kind="
-00012730: 7375 6222 2c20 7269 6768 743d 5472 7565  sub", right=True
-00012740: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00012750: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
-00012760: 2020 2020 6465 6620 7375 625f 6c65 6674      def sub_left
-00012770: 2873 656c 663a 2044 696d 2c20 6f74 6865  (self: Dim, othe
-00012780: 7229 3a0a 2020 2020 2020 2020 2222 220a  r):.        """.
-00012790: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-000127a0: 696d 7c69 6e74 206f 7468 6572 3a0a 2020  im|int other:.  
-000127b0: 2020 2020 2020 3a72 6574 7572 6e3a 2028        :return: (
-000127c0: 2d6f 7468 6572 2920 2b20 7365 6c66 0a20  -other) + self. 
-000127d0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-000127e0: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-000127f0: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-00012800: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
-00012810: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-00012820: 2020 2074 6572 6d2e 6578 7465 6e64 5f61     term.extend_a
-00012830: 6464 5f73 7562 5f28 6f74 6865 722c 206b  dd_sub_(other, k
-00012840: 696e 643d 2273 7562 222c 2072 6967 6874  ind="sub", right
-00012850: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00012860: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
-00012870: 696d 2829 0a0a 2020 2020 6465 6620 5f5f  im()..    def __
-00012880: 6d75 6c5f 5f28 7365 6c66 3a20 4469 6d2c  mul__(self: Dim,
-00012890: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-000128a0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-000128b0: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-000128c0: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-000128d0: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-000128e0: 2222 0a20 2020 2020 2020 2074 6572 6d20  "".        term 
-000128f0: 3d20 5f4f 704c 696e 6561 7254 6572 6d2e  = _OpLinearTerm.
-00012900: 6672 6f6d 5f64 696d 2873 656c 6629 0a20  from_dim(self). 
-00012910: 2020 2020 2020 2074 6572 6d2e 6578 7465         term.exte
-00012920: 6e64 5f6d 756c 5f64 6976 5f28 6f74 6865  nd_mul_div_(othe
-00012930: 722c 206b 696e 643d 226d 756c 222c 2072  r, kind="mul", r
-00012940: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
-00012950: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
-00012960: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
-00012970: 205f 5f72 6d75 6c5f 5f28 7365 6c66 3a20   __rmul__(self: 
-00012980: 4469 6d2c 206f 7468 6572 293a 0a20 2020  Dim, other):.   
-00012990: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000129a0: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-000129b0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-000129c0: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-000129d0: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-000129e0: 6572 6d20 3d20 5f4f 704c 696e 6561 7254  erm = _OpLinearT
-000129f0: 6572 6d2e 6672 6f6d 5f64 696d 2873 656c  erm.from_dim(sel
-00012a00: 6629 0a20 2020 2020 2020 2074 6572 6d2e  f).        term.
-00012a10: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
-00012a20: 6f74 6865 722c 206b 696e 643d 226d 756c  other, kind="mul
-00012a30: 222c 2072 6967 6874 3d46 616c 7365 290a  ", right=False).
-00012a40: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00012a50: 6572 6d2e 6173 5f64 696d 2829 0a0a 2020  erm.as_dim()..  
-00012a60: 2020 6465 6620 5f5f 666c 6f6f 7264 6976    def __floordiv
-00012a70: 5f5f 2873 656c 663a 2044 696d 2c20 6f74  __(self: Dim, ot
-00012a80: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
-00012a90: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00012aa0: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
-00012ab0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00012ac0: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
-00012ad0: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
-00012ae0: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
-00012af0: 6d5f 6469 6d28 7365 6c66 290a 2020 2020  m_dim(self).    
-00012b00: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
-00012b10: 6d75 6c5f 6469 765f 286f 7468 6572 2c20  mul_div_(other, 
-00012b20: 6b69 6e64 3d22 666c 6f6f 7264 6976 222c  kind="floordiv",
-00012b30: 2072 6967 6874 3d54 7275 6529 0a20 2020   right=True).   
-00012b40: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
-00012b50: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
-00012b60: 6566 205f 5f74 7275 6564 6976 5f5f 2873  ef __truediv__(s
-00012b70: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-00012b80: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012b90: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-00012ba0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00012bb0: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00012bc0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00012bd0: 6574 7572 6e20 7365 6c66 2e64 6976 5f72  eturn self.div_r
-00012be0: 6967 6874 286f 7468 6572 290a 0a20 2020  ight(other)..   
-00012bf0: 2064 6566 2064 6976 5f6c 6566 7428 7365   def div_left(se
-00012c00: 6c66 3a20 4469 6d2c 206f 7468 6572 293a  lf: Dim, other):
-00012c10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012c20: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
-00012c30: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
-00012c40: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-00012c50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012c60: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
-00012c70: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
-00012c80: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
-00012c90: 6572 6d2e 6578 7465 6e64 5f6d 756c 5f64  erm.extend_mul_d
-00012ca0: 6976 5f28 6f74 6865 722c 206b 696e 643d  iv_(other, kind=
-00012cb0: 2274 7275 6564 6976 222c 2072 6967 6874  "truediv", right
-00012cc0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00012cd0: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
-00012ce0: 696d 2829 0a0a 2020 2020 6465 6620 6469  im()..    def di
-00012cf0: 765f 7269 6768 7428 7365 6c66 3a20 4469  v_right(self: Di
-00012d00: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
-00012d10: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00012d20: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
-00012d30: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
-00012d40: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
-00012d50: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
-00012d60: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
-00012d70: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
-00012d80: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
-00012d90: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
-00012da0: 6865 722c 206b 696e 643d 2274 7275 6564  her, kind="trued
-00012db0: 6976 222c 2072 6967 6874 3d54 7275 6529  iv", right=True)
-00012dc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012dd0: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
-00012de0: 2020 2064 6566 2063 6569 6c64 6976 5f6c     def ceildiv_l
-00012df0: 6566 7428 7365 6c66 3a20 4469 6d2c 206f  eft(self: Dim, o
-00012e00: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
-00012e10: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00012e20: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
-00012e30: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00012e40: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
-00012e50: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
-00012e60: 5f4f 704c 696e 6561 7254 6572 6d2e 6672  _OpLinearTerm.fr
-00012e70: 6f6d 5f64 696d 2873 656c 6629 0a20 2020  om_dim(self).   
-00012e80: 2020 2020 2074 6572 6d2e 6578 7465 6e64       term.extend
-00012e90: 5f6d 756c 5f64 6976 5f28 6f74 6865 722c  _mul_div_(other,
-00012ea0: 206b 696e 643d 2263 6569 6c64 6976 222c   kind="ceildiv",
-00012eb0: 2072 6967 6874 3d46 616c 7365 290a 2020   right=False).  
-00012ec0: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-00012ed0: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
-00012ee0: 6465 6620 6365 696c 6469 765f 7269 6768  def ceildiv_righ
-00012ef0: 7428 7365 6c66 3a20 4469 6d2c 206f 7468  t(self: Dim, oth
-00012f00: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
-00012f10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00012f20: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-00012f30: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00012f40: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-00012f50: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-00012f60: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
-00012f70: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-00012f80: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
-00012f90: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
-00012fa0: 696e 643d 2263 6569 6c64 6976 222c 2072  ind="ceildiv", r
-00012fb0: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
-00012fc0: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
-00012fd0: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
-00012fe0: 205f 5f6e 6567 5f5f 2873 656c 6629 3a0a   __neg__(self):.
-00012ff0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013000: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-00013010: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013020: 2020 2020 7265 7475 726e 202d 3120 2a20      return -1 * 
-00013030: 7365 6c66 0a0a 2020 2020 6465 6620 6973  self..    def is
-00013040: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-00013050: 5f64 696d 2873 656c 6629 202d 3e20 626f  _dim(self) -> bo
-00013060: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-00013070: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00013080: 2064 6572 6976 6564 206f 7020 6f66 2074   derived op of t
-00013090: 7970 6520 636f 6e73 7461 6e74 0a20 2020  ype constant.   
-000130a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000130b0: 2072 6574 7572 6e20 7365 6c66 2e64 6572   return self.der
-000130c0: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
-000130d0: 2073 656c 662e 6465 7269 7665 645f 6672   self.derived_fr
-000130e0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2263  om_op.kind == "c
-000130f0: 6f6e 7374 616e 7422 0a0a 0a64 6566 205f  onstant"...def _
-00013100: 6d61 6b65 5f63 6f6e 7374 616e 745f 7374  make_constant_st
-00013110: 6174 6963 5f64 696d 2876 616c 7565 2c20  atic_dim(value, 
-00013120: 6b69 6e64 3d4e 6f6e 6529 3a0a 2020 2020  kind=None):.    
-00013130: 2222 220a 2020 2020 3a70 6172 616d 2069  """.    :param i
-00013140: 6e74 2076 616c 7565 3a0a 2020 2020 3a70  nt value:.    :p
-00013150: 6172 616d 2045 6e74 6974 797c 4e6f 6e65  aram Entity|None
-00013160: 206b 696e 643a 0a20 2020 203a 7274 7970   kind:.    :rtyp
-00013170: 653a 2044 696d 0a20 2020 2022 2222 0a20  e: Dim.    """. 
-00013180: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
-00013190: 280a 2020 2020 2020 2020 6469 6d65 6e73  (.        dimens
-000131a0: 696f 6e3d 7661 6c75 652c 0a20 2020 2020  ion=value,.     
-000131b0: 2020 206b 696e 643d 6b69 6e64 206f 7220     kind=kind or 
-000131c0: 4469 6d54 7970 6573 2e55 6e73 7065 6369  DimTypes.Unspeci
-000131d0: 6669 6564 2c0a 2020 2020 2020 2020 6465  fied,.        de
-000131e0: 7363 7269 7074 696f 6e3d 2275 6e6e 616d  scription="unnam
-000131f0: 6564 5f25 7364 696d 5f25 6922 2025 2028  ed_%sdim_%i" % (
-00013200: 6b69 6e64 2e6e 616d 6520 2b20 225f 2220  kind.name + "_" 
-00013210: 6966 206b 696e 6420 656c 7365 2022 222c  if kind else "",
-00013220: 2076 616c 7565 292c 0a20 2020 2020 2020   value),.       
-00013230: 2064 6572 6976 6564 5f66 726f 6d5f 6f70   derived_from_op
-00013240: 3d4f 7028 6b69 6e64 3d22 636f 6e73 7461  =Op(kind="consta
-00013250: 6e74 222c 2069 6e70 7574 733d 5b5d 2c20  nt", inputs=[], 
-00013260: 6174 7472 6962 733d 7b22 7661 6c75 6522  attribs={"value"
-00013270: 3a20 7661 6c75 657d 292c 0a20 2020 2020  : value}),.     
-00013280: 2020 2061 7574 6f5f 6765 6e65 7261 7465     auto_generate
-00013290: 643d 5472 7565 2c0a 2020 2020 290a 0a0a  d=True,.    )...
-000132a0: 636c 6173 7320 4f70 3a0a 2020 2020 2222  class Op:.    ""
-000132b0: 220a 2020 2020 4f70 206f 6e20 3a63 6c61  ".    Op on :cla
-000132c0: 7373 3a60 4469 6d60 2077 6869 6368 2072  ss:`Dim` which r
-000132d0: 6573 756c 7473 2069 6e20 6120 6465 7269  esults in a deri
-000132e0: 7665 6420 3a63 6c61 7373 3a60 4469 6d60  ved :class:`Dim`
-000132f0: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00013300: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00013310: 2c20 6b69 6e64 2c20 696e 7075 7473 2c20  , kind, inputs, 
-00013320: 6174 7472 6962 733d 4e6f 6e65 293a 0a20  attribs=None):. 
-00013330: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013340: 2020 203a 7061 7261 6d20 7374 7220 6b69     :param str ki
-00013350: 6e64 3a20 2261 6464 222c 2022 7375 6222  nd: "add", "sub"
-00013360: 2c20 226d 756c 222c 2022 6365 696c 6469  , "mul", "ceildi
-00013370: 7622 0a20 2020 2020 2020 203a 7061 7261  v".        :para
-00013380: 6d20 6c69 7374 5b44 696d 5d20 696e 7075  m list[Dim] inpu
-00013390: 7473 3a0a 2020 2020 2020 2020 3a70 6172  ts:.        :par
-000133a0: 616d 2064 6963 745b 7374 725d 7c4e 6f6e  am dict[str]|Non
-000133b0: 6520 6174 7472 6962 733a 0a20 2020 2020  e attribs:.     
-000133c0: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-000133d0: 656c 662e 6b69 6e64 203d 206b 696e 640a  elf.kind = kind.
-000133e0: 2020 2020 2020 2020 7365 6c66 2e69 6e70          self.inp
-000133f0: 7574 7320 3d20 696e 7075 7473 0a20 2020  uts = inputs.   
-00013400: 2020 2020 2073 656c 662e 6f75 7470 7574       self.output
-00013410: 203d 204e 6f6e 6520 2023 2074 7970 653a   = None  # type:
-00013420: 204f 7074 696f 6e61 6c5b 5f64 2e44 696d   Optional[_d.Dim
-00013430: 5d0a 2020 2020 2020 2020 7365 6c66 2e61  ].        self.a
-00013440: 7474 7269 6273 203d 2061 7474 7269 6273  ttribs = attribs
-00013450: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
-00013460: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00013470: 2020 6174 7472 6962 7320 3d20 2822 2025    attribs = (" %
-00013480: 7222 2025 2073 656c 662e 6174 7472 6962  r" % self.attrib
-00013490: 7329 2069 6620 7365 6c66 2e61 7474 7269  s) if self.attri
-000134a0: 6273 2065 6c73 6520 2222 0a20 2020 2020  bs else "".     
-000134b0: 2020 2072 6574 7572 6e20 223c 4469 6d2e     return "<Dim.
-000134c0: 4f70 2025 7220 2573 2573 3e22 2025 2028  Op %r %s%s>" % (
-000134d0: 7365 6c66 2e6b 696e 642c 2073 656c 662e  self.kind, self.
-000134e0: 696e 7075 7473 2c20 6174 7472 6962 7329  inputs, attribs)
-000134f0: 0a0a 2020 2020 6465 6620 5f76 616c 7565  ..    def _value
-00013500: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00013510: 7265 7475 726e 2073 656c 662e 6b69 6e64  return self.kind
-00013520: 2c20 7475 706c 6528 7365 6c66 2e69 6e70  , tuple(self.inp
-00013530: 7574 7329 2c20 6672 6f7a 656e 7365 7428  uts), frozenset(
-00013540: 7365 6c66 2e61 7474 7269 6273 2e69 7465  self.attribs.ite
-00013550: 6d73 2829 2920 6966 2073 656c 662e 6174  ms()) if self.at
-00013560: 7472 6962 7320 656c 7365 204e 6f6e 650a  tribs else None.
-00013570: 0a20 2020 2064 6566 205f 5f68 6173 685f  .    def __hash_
-00013580: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00013590: 2072 6574 7572 6e20 6861 7368 2873 656c   return hash(sel
-000135a0: 662e 5f76 616c 7565 2829 290a 0a20 2020  f._value())..   
-000135b0: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
-000135c0: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-000135d0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-000135e0: 6f74 6865 722c 204f 7029 3a0a 2020 2020  other, Op):.    
-000135f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00013600: 656c 662e 5f76 616c 7565 2829 203d 3d20  elf._value() == 
-00013610: 6f74 6865 722e 5f76 616c 7565 2829 0a20  other._value(). 
-00013620: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00013630: 6c73 650a 0a20 2020 2064 6566 205f 5f6e  lse..    def __n
-00013640: 655f 5f28 7365 6c66 2c20 6f74 6865 7229  e__(self, other)
-00013650: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00013660: 206e 6f74 2073 656c 662e 5f5f 6571 5f5f   not self.__eq__
-00013670: 286f 7468 6572 290a 0a0a 6465 6620 5f67  (other)...def _g
-00013680: 6574 5f64 6573 6372 6970 7469 6f6e 2864  et_description(d
-00013690: 696d 2c20 6272 6163 6b65 7473 3d54 7275  im, brackets=Tru
-000136a0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-000136b0: 3a70 6172 616d 2044 696d 2064 696d 3a0a  :param Dim dim:.
-000136c0: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-000136d0: 6272 6163 6b65 7473 3a20 6164 6420 6272  brackets: add br
-000136e0: 6163 6b65 7473 2077 6865 6e20 6e65 6365  ackets when nece
-000136f0: 7373 6172 790a 2020 2020 3a72 7479 7065  ssary.    :rtype
-00013700: 3a20 7374 720a 2020 2020 2222 220a 2020  : str.    """.  
-00013710: 2020 6966 2064 696d 2e64 6573 6372 6970    if dim.descrip
-00013720: 7469 6f6e 2061 6e64 2064 696d 2e64 6573  tion and dim.des
-00013730: 6372 6970 7469 6f6e 2e73 7461 7274 7377  cription.startsw
-00013740: 6974 6828 2275 6e6e 616d 6564 5f22 2920  ith("unnamed_") 
-00013750: 616e 6420 6469 6d2e 6469 6d65 6e73 696f  and dim.dimensio
-00013760: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00013770: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-00013780: 7228 6469 6d2e 6469 6d65 6e73 696f 6e29  r(dim.dimension)
-00013790: 0a20 2020 2069 6620 6469 6d2e 6465 7363  .    if dim.desc
-000137a0: 7269 7074 696f 6e3a 0a20 2020 2020 2020  ription:.       
-000137b0: 2069 6620 6272 6163 6b65 7473 3a0a 2020   if brackets:.  
-000137c0: 2020 2020 2020 2020 2020 696d 706f 7274            import
-000137d0: 2072 650a 0a20 2020 2020 2020 2020 2020   re..           
-000137e0: 2069 6620 7265 2e73 6561 7263 6828 225b   if re.search("[
-000137f0: 2b5c 5c2d 2f20 5d22 2c20 6469 6d2e 6465  +\\-/ ]", dim.de
-00013800: 7363 7269 7074 696f 6e29 3a0a 2020 2020  scription):.    
-00013810: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00013820: 726e 2022 2825 7329 2220 2520 6469 6d2e  rn "(%s)" % dim.
-00013830: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
-00013840: 2020 2020 7265 7475 726e 2064 696d 2e64      return dim.d
-00013850: 6573 6372 6970 7469 6f6e 0a20 2020 2072  escription.    r
-00013860: 6574 7572 6e20 2275 6e6e 616d 6564 5f25  eturn "unnamed_%
-00013870: 735f 6469 6d25 7322 2025 2028 6469 6d2e  s_dim%s" % (dim.
-00013880: 6b69 6e64 2c20 6469 6d2e 6469 6d65 6e73  kind, dim.dimens
-00013890: 696f 6e20 6966 2064 696d 2e64 696d 656e  ion if dim.dimen
-000138a0: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
-000138b0: 2065 6c73 6520 223f 2229 0a0a 0a63 6c61   else "?")...cla
-000138c0: 7373 205f 4f70 4d75 6c74 5465 726d 3a0a  ss _OpMultTerm:.
-000138d0: 2020 2020 2222 220a 2020 2020 7265 7072      """.    repr
-000138e0: 6573 656e 7473 2073 7468 206c 696b 6520  esents sth like 
-000138f0: 6120 2a20 6220 2a20 630a 2020 2020 2222  a * b * c.    ""
-00013900: 220a 0a20 2020 2040 636c 6173 736d 6574  "..    @classmet
-00013910: 686f 640a 2020 2020 6465 6620 6672 6f6d  hod.    def from
-00013920: 5f64 696d 2863 6c73 2c20 6469 6d3a 205f  _dim(cls, dim: _
-00013930: 642e 4469 6d29 202d 3e20 5f4f 704d 756c  d.Dim) -> _OpMul
-00013940: 7454 6572 6d3a 0a20 2020 2020 2020 2022  tTerm:.        "
-00013950: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00013960: 6d20 6469 6d3a 0a20 2020 2020 2020 203a  m dim:.        :
-00013970: 7265 7475 726e 3a20 6f70 206d 756c 7420  return: op mult 
-00013980: 7465 726d 0a20 2020 2020 2020 2022 2222  term.        """
-00013990: 0a20 2020 2020 2020 2064 696d 203d 2064  .        dim = d
-000139a0: 696d 2e67 6574 5f73 616d 655f 6261 7365  im.get_same_base
-000139b0: 2829 0a20 2020 2020 2020 2069 6620 6469  ().        if di
-000139c0: 6d2e 6469 6d65 6e73 696f 6e20 3d3d 2031  m.dimension == 1
-000139d0: 2061 6e64 2064 696d 2e69 735f 636f 6e73   and dim.is_cons
-000139e0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-000139f0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00013a00: 6574 7572 6e20 636c 732e 6f6e 6528 290a  eturn cls.one().
-00013a10: 2020 2020 2020 2020 6966 2064 696d 2e64          if dim.d
-00013a20: 6572 6976 6564 5f66 726f 6d5f 6f70 2061  erived_from_op a
-00013a30: 6e64 2064 696d 2e64 6572 6976 6564 5f66  nd dim.derived_f
-00013a40: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-00013a50: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
-00013a60: 2020 7265 7475 726e 2063 6c73 286c 6973    return cls(lis
-00013a70: 7428 6469 6d2e 6465 7269 7665 645f 6672  t(dim.derived_fr
-00013a80: 6f6d 5f6f 702e 696e 7075 7473 2929 0a20  om_op.inputs)). 
-00013a90: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-00013aa0: 7328 5b64 696d 5d29 0a0a 2020 2020 4063  s([dim])..    @c
-00013ab0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00013ac0: 6566 2066 726f 6d5f 6469 6d5f 6661 6374  ef from_dim_fact
-00013ad0: 6f72 7328 636c 732c 2064 696d 7329 3a0a  ors(cls, dims):.
-00013ae0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013af0: 2020 2020 3a70 6172 616d 206c 6973 745b      :param list[
-00013b00: 4469 6d5d 2064 696d 733a 0a20 2020 2020  Dim] dims:.     
-00013b10: 2020 203a 7274 7970 653a 2044 696d 2e5f     :rtype: Dim._
-00013b20: 4f70 4d75 6c74 5465 726d 0a20 2020 2020  OpMultTerm.     
-00013b30: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00013b40: 6573 203d 2063 6c73 2e6f 6e65 2829 0a20  es = cls.one(). 
-00013b50: 2020 2020 2020 2066 6f72 2064 2069 6e20         for d in 
-00013b60: 6469 6d73 3a0a 2020 2020 2020 2020 2020  dims:.          
-00013b70: 2020 7265 732e 6578 7465 6e64 5f6d 756c    res.extend_mul
-00013b80: 5f64 6976 5f28 642c 206b 696e 643d 226d  _div_(d, kind="m
-00013b90: 756c 222c 2072 6967 6874 3d54 7275 6529  ul", right=True)
-00013ba0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013bb0: 7265 730a 0a20 2020 2040 636c 6173 736d  res..    @classm
-00013bc0: 6574 686f 640a 2020 2020 6465 6620 6f6e  ethod.    def on
-00013bd0: 6528 636c 7329 3a0a 2020 2020 2020 2020  e(cls):.        
-00013be0: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
-00013bf0: 7065 3a20 4469 6d2e 5f4f 704d 756c 7454  pe: Dim._OpMultT
-00013c00: 6572 6d0a 2020 2020 2020 2020 2222 220a  erm.        """.
-00013c10: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00013c20: 6c73 285b 5d29 0a0a 2020 2020 6465 6620  ls([])..    def 
-00013c30: 5f5f 696e 6974 5f5f 2873 656c 662c 2074  __init__(self, t
-00013c40: 6572 6d73 293a 0a20 2020 2020 2020 2022  erms):.        "
-00013c50: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00013c60: 6d20 6c69 7374 5b44 696d 5d20 7465 726d  m list[Dim] term
-00013c70: 733a 0a20 2020 2020 2020 2022 2222 0a20  s:.        """. 
-00013c80: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
-00013c90: 7320 3d20 7465 726d 730a 0a20 2020 2064  s = terms..    d
-00013ca0: 6566 205f 5f68 6173 685f 5f28 7365 6c66  ef __hash__(self
-00013cb0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00013cc0: 6e20 6861 7368 2874 7570 6c65 2873 656c  n hash(tuple(sel
-00013cd0: 662e 7465 726d 7329 290a 0a20 2020 2064  f.terms))..    d
-00013ce0: 6566 205f 5f65 715f 5f28 7365 6c66 2c20  ef __eq__(self, 
-00013cf0: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-00013d00: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-00013d10: 616d 2044 696d 7c44 696d 2e5f 4f70 4d75  am Dim|Dim._OpMu
-00013d20: 6c74 5465 726d 206f 7468 6572 3a0a 2020  ltTerm other:.  
-00013d30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013d40: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013d50: 6f74 6865 722c 205f 4f70 4d75 6c74 5465  other, _OpMultTe
-00013d60: 726d 293a 0a20 2020 2020 2020 2020 2020  rm):.           
-00013d70: 2072 6574 7572 6e20 7365 6c66 2e74 6572   return self.ter
-00013d80: 6d73 203d 3d20 6f74 6865 722e 7465 726d  ms == other.term
-00013d90: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-00013da0: 2046 616c 7365 0a0a 2020 2020 6465 6620   False..    def 
-00013db0: 5f5f 6e65 5f5f 2873 656c 662c 206f 7468  __ne__(self, oth
-00013dc0: 6572 293a 0a20 2020 2020 2020 2072 6574  er):.        ret
-00013dd0: 7572 6e20 6e6f 7420 7365 6c66 2e5f 5f65  urn not self.__e
-00013de0: 715f 5f28 6f74 6865 7229 0a0a 2020 2020  q__(other)..    
-00013df0: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
-00013e00: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00013e10: 726e 2022 4469 6d2e 5f4f 704d 756c 7454  rn "Dim._OpMultT
-00013e20: 6572 6d28 2572 2922 2025 2028 7365 6c66  erm(%r)" % (self
-00013e30: 2e74 6572 6d73 2c29 0a0a 2020 2020 4070  .terms,)..    @p
-00013e40: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00013e50: 6469 6d65 6e73 696f 6e28 7365 6c66 293a  dimension(self):
-00013e60: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013e70: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
-00013e80: 7c4e 6f6e 650a 2020 2020 2020 2020 2222  |None.        ""
-00013e90: 220a 2020 2020 2020 2020 6469 6d20 3d20  ".        dim = 
-00013ea0: 310a 2020 2020 2020 2020 666f 7220 7061  1.        for pa
-00013eb0: 7274 2069 6e20 7365 6c66 2e74 6572 6d73  rt in self.terms
-00013ec0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00013ed0: 2070 6172 742e 6469 6d65 6e73 696f 6e20   part.dimension 
-00013ee0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00013ef0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00013f00: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00013f10: 2064 696d 202a 3d20 7061 7274 2e64 696d   dim *= part.dim
-00013f20: 656e 7369 6f6e 0a20 2020 2020 2020 2072  ension.        r
-00013f30: 6574 7572 6e20 6469 6d0a 0a20 2020 2064  eturn dim..    d
-00013f40: 6566 2062 6173 655f 7465 726d 2873 656c  ef base_term(sel
-00013f50: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-00013f60: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00013f70: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
-00013f80: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00013f90: 656c 662e 7465 726d 730a 2020 2020 2020  elf.terms.      
-00013fa0: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
-00013fb0: 726d 735b 2d31 5d0a 0a20 2020 2064 6566  rms[-1]..    def
-00013fc0: 2069 735f 6f6e 6528 7365 6c66 293a 0a20   is_one(self):. 
-00013fd0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013fe0: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-00013ff0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00014000: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
-00014010: 656c 662e 7465 726d 730a 0a20 2020 2064  elf.terms..    d
-00014020: 6566 2069 735f 636f 6e73 7461 6e74 5f73  ef is_constant_s
-00014030: 7461 7469 635f 6469 6d28 7365 6c66 293a  tatic_dim(self):
-00014040: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014050: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00014060: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-00014070: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00014080: 662e 7465 726d 733a 0a20 2020 2020 2020  f.terms:.       
-00014090: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-000140a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000140b0: 616c 6c28 7465 726d 2e69 735f 636f 6e73  all(term.is_cons
-000140c0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-000140d0: 2920 666f 7220 7465 726d 2069 6e20 7365  ) for term in se
-000140e0: 6c66 2e74 6572 6d73 290a 0a20 2020 2064  lf.terms)..    d
-000140f0: 6566 2063 6f70 7928 7365 6c66 293a 0a20  ef copy(self):. 
-00014100: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00014110: 2020 203a 7274 7970 653a 2044 696d 2e5f     :rtype: Dim._
-00014120: 4f70 4d75 6c74 5465 726d 0a20 2020 2020  OpMultTerm.     
-00014130: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00014140: 6574 7572 6e20 5f4f 704d 756c 7454 6572  eturn _OpMultTer
-00014150: 6d28 6c69 7374 2873 656c 662e 7465 726d  m(list(self.term
-00014160: 7329 290a 0a20 2020 2064 6566 206e 6567  s))..    def neg
-00014170: 6174 6976 6528 7365 6c66 293a 0a20 2020  ative(self):.   
-00014180: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014190: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
-000141a0: 4d75 6c74 5465 726d 0a20 2020 2020 2020  MultTerm.       
-000141b0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-000141c0: 7365 6c66 2e74 6572 6d73 2061 6e64 2073  self.terms and s
-000141d0: 656c 662e 7465 726d 735b 305d 2e69 735f  elf.terms[0].is_
-000141e0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-000141f0: 6469 6d28 2920 616e 6420 7365 6c66 2e74  dim() and self.t
-00014200: 6572 6d73 5b30 5d2e 6469 6d65 6e73 696f  erms[0].dimensio
-00014210: 6e20 3d3d 202d 313a 0a20 2020 2020 2020  n == -1:.       
-00014220: 2020 2020 2072 6574 7572 6e20 5f4f 704d       return _OpM
-00014230: 756c 7454 6572 6d28 7365 6c66 2e74 6572  ultTerm(self.ter
-00014240: 6d73 5b31 3a5d 290a 2020 2020 2020 2020  ms[1:]).        
-00014250: 7265 7320 3d20 7365 6c66 2e63 6f70 7928  res = self.copy(
-00014260: 290a 2020 2020 2020 2020 7265 732e 6578  ).        res.ex
-00014270: 7465 6e64 5f6d 756c 5f64 6976 5f28 5f6d  tend_mul_div_(_m
-00014280: 616b 655f 636f 6e73 7461 6e74 5f73 7461  ake_constant_sta
-00014290: 7469 635f 6469 6d28 2d31 292c 206b 696e  tic_dim(-1), kin
-000142a0: 643d 226d 756c 222c 2072 6967 6874 3d46  d="mul", right=F
-000142b0: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
-000142c0: 7475 726e 2072 6573 0a0a 2020 2020 6465  turn res..    de
-000142d0: 6620 6469 7669 7369 626c 6528 7365 6c66  f divisible(self
-000142e0: 2c20 6f74 6865 722c 2072 6967 6874 293a  , other, right):
-000142f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014300: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
-00014310: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00014320: 7061 7261 6d20 626f 6f6c 2072 6967 6874  param bool right
-00014330: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
-00014340: 6e3a 2077 6865 7468 6572 2077 6520 6361  n: whether we ca
-00014350: 6e20 6469 7669 6465 206f 7468 6572 2c20  n divide other, 
-00014360: 7769 7468 6f75 7420 7265 6d61 696e 6465  without remainde
-00014370: 720a 2020 2020 2020 2020 3a72 7479 7065  r.        :rtype
-00014380: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-00014390: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-000143a0: 7420 7365 6c66 2e74 6572 6d73 3a0a 2020  t self.terms:.  
-000143b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000143c0: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
-000143d0: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
-000143e0: 6672 6f6d 5f6f 7020 616e 6420 6f74 6865  from_op and othe
-000143f0: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00014400: 702e 6b69 6e64 203d 3d20 226d 756c 223a  p.kind == "mul":
-00014410: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-00014420: 203d 2073 656c 662e 636f 7079 2829 0a20   = self.copy(). 
-00014430: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-00014440: 6572 6d20 696e 206f 7468 6572 2e64 6572  erm in other.der
-00014450: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-00014460: 7574 7320 6966 2072 6967 6874 2065 6c73  uts if right els
-00014470: 6520 7265 7665 7273 6564 286f 7468 6572  e reversed(other
-00014480: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00014490: 2e69 6e70 7574 7329 3a0a 2020 2020 2020  .inputs):.      
-000144a0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000144b0: 2074 6d70 2e64 6976 6973 6962 6c65 2874   tmp.divisible(t
-000144c0: 6572 6d2c 2072 6967 6874 3d72 6967 6874  erm, right=right
-000144d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000144e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000144f0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00014500: 2020 2020 746d 702e 6578 7465 6e64 5f6d      tmp.extend_m
-00014510: 756c 5f64 6976 5f28 7465 726d 2c20 6b69  ul_div_(term, ki
-00014520: 6e64 3d22 7472 7565 6469 7622 2c20 7269  nd="truediv", ri
-00014530: 6768 743d 7269 6768 7429 0a20 2020 2020  ght=right).     
-00014540: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00014550: 7565 0a20 2020 2020 2020 206d 6f73 745f  ue.        most_
-00014560: 7265 6365 6e74 5f74 6572 6d20 3d20 7365  recent_term = se
-00014570: 6c66 2e74 6572 6d73 5b2d 3120 6966 2072  lf.terms[-1 if r
-00014580: 6967 6874 2065 6c73 6520 305d 0a20 2020  ight else 0].   
-00014590: 2020 2020 2069 6620 6f74 6865 7220 3d3d       if other ==
-000145a0: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
-000145b0: 6d3a 0a20 2020 2020 2020 2020 2020 2072  m:.            r
-000145c0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-000145d0: 2020 2069 6620 6d6f 7374 5f72 6563 656e     if most_recen
-000145e0: 745f 7465 726d 2e64 696d 656e 7369 6f6e  t_term.dimension
-000145f0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00014600: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
-00014610: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00014620: 2020 2020 2020 2020 2020 6966 206d 6f73            if mos
-00014630: 745f 7265 6365 6e74 5f74 6572 6d2e 6469  t_recent_term.di
-00014640: 6d65 6e73 696f 6e20 2520 6f74 6865 722e  mension % other.
-00014650: 6469 6d65 6e73 696f 6e20 3d3d 2030 3a0a  dimension == 0:.
-00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014670: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-00014680: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00014690: 0a0a 2020 2020 6465 6620 6361 6e5f 7369  ..    def can_si
-000146a0: 6d70 6c69 6679 2873 656c 662c 206f 7468  mplify(self, oth
-000146b0: 6572 2c20 6b69 6e64 2c20 7269 6768 7429  er, kind, right)
-000146c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000146d0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-000146e0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
-000146f0: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
-00014700: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00014710: 626f 6f6c 2072 6967 6874 3a0a 2020 2020  bool right:.    
-00014720: 2020 2020 3a72 6574 7572 6e3a 2077 6865      :return: whe
-00014730: 7468 6572 2077 6520 6361 6e20 7369 6d70  ther we can simp
-00014740: 6c69 6679 2077 6865 6e20 6170 706c 7969  lify when applyi
-00014750: 6e67 2074 6869 7320 6f70 6572 6174 696f  ng this operatio
-00014760: 6e0a 2020 2020 2020 2020 3a72 7479 7065  n.        :rtype
-00014770: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-00014780: 2222 0a20 2020 2020 2020 2069 6620 6f74  "".        if ot
-00014790: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
-000147a0: 5f6f 7020 616e 6420 6f74 6865 722e 6465  _op and other.de
-000147b0: 7269 7665 645f 6672 6f6d 5f6f 702e 6b69  rived_from_op.ki
-000147c0: 6e64 203d 3d20 226d 756c 223a 0a20 2020  nd == "mul":.   
-000147d0: 2020 2020 2020 2020 2074 6d70 203d 2073           tmp = s
-000147e0: 656c 662e 636f 7079 2829 0a20 2020 2020  elf.copy().     
-000147f0: 2020 2020 2020 2066 6f72 2074 6572 6d20         for term 
-00014800: 696e 206f 7468 6572 2e64 6572 6976 6564  in other.derived
-00014810: 5f66 726f 6d5f 6f70 2e69 6e70 7574 7320  _from_op.inputs 
-00014820: 6966 2072 6967 6874 2065 6c73 6520 7265  if right else re
-00014830: 7665 7273 6564 286f 7468 6572 2e64 6572  versed(other.der
-00014840: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-00014850: 7574 7329 3a0a 2020 2020 2020 2020 2020  uts):.          
-00014860: 2020 2020 2020 6966 206e 6f74 2074 6d70        if not tmp
-00014870: 2e63 616e 5f73 696d 706c 6966 7928 7465  .can_simplify(te
-00014880: 726d 2c20 6b69 6e64 3d6b 696e 642c 2072  rm, kind=kind, r
-00014890: 6967 6874 3d72 6967 6874 293a 0a20 2020  ight=right):.   
-000148a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148b0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-000148c0: 2020 2020 2020 2020 2020 2020 2020 746d                tm
-000148d0: 702e 6578 7465 6e64 5f6d 756c 5f64 6976  p.extend_mul_div
-000148e0: 5f28 7465 726d 2c20 6b69 6e64 3d6b 696e  _(term, kind=kin
-000148f0: 642c 2072 6967 6874 3d72 6967 6874 290a  d, right=right).
-00014900: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00014910: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-00014920: 6964 7820 3d20 7365 6c66 2e5f 7369 6d70  idx = self._simp
-00014930: 6c69 6679 5f74 6572 6d5f 6964 7828 6f74  lify_term_idx(ot
-00014940: 6865 722c 206b 696e 643d 6b69 6e64 2c20  her, kind=kind, 
-00014950: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
-00014960: 2020 2020 2072 6574 7572 6e20 6964 7820       return idx 
-00014970: 6973 206e 6f74 204e 6f6e 650a 0a20 2020  is not None..   
-00014980: 2064 6566 205f 7369 6d70 6c69 6679 5f74   def _simplify_t
-00014990: 6572 6d5f 6964 7828 7365 6c66 2c20 6f74  erm_idx(self, ot
-000149a0: 6865 722c 206b 696e 642c 2072 6967 6874  her, kind, right
-000149b0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-000149c0: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
-000149d0: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
-000149e0: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
-000149f0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-00014a00: 2062 6f6f 6c20 7269 6768 743a 0a20 2020   bool right:.   
-00014a10: 2020 2020 203a 7265 7475 726e 3a20 696e       :return: in
-00014a20: 6465 7820 6f66 2074 6572 6d20 746f 2073  dex of term to s
-00014a30: 696d 706c 6966 790a 2020 2020 2020 2020  implify.        
-00014a40: 3a72 7479 7065 3a20 696e 747c 4e6f 6e65  :rtype: int|None
-00014a50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014a60: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00014a70: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00014a80: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00014a90: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
-00014aa0: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
-00014ab0: 2020 2020 2020 2320 5765 2077 616e 7420        # We want 
-00014ac0: 2862 202a 2061 2920 2f2f 2062 2021 3d20  (b * a) // b != 
-00014ad0: 612e 0a20 2020 2020 2020 2020 2020 2023  a..            #
-00014ae0: 2048 6f77 6576 6572 2c20 7765 2077 616e   However, we wan
-00014af0: 7420 6820 2a20 2832 202a 2061 202f 2f20  t h * (2 * a // 
-00014b00: 6829 203d 3d20 3220 2a20 612e 0a20 2020  h) == 2 * a..   
-00014b10: 2020 2020 2020 2020 2023 2053 6f2c 2066           # So, f
-00014b20: 6f72 2060 6d75 6c60 2c20 616e 6420 6f6e  or `mul`, and on
-00014b30: 6c79 2066 6f72 2060 6d75 6c60 2c20 6368  ly for `mul`, ch
-00014b40: 6563 6b20 616c 6c20 7465 726d 732c 2077  eck all terms, w
-00014b50: 6865 7468 6572 2077 6520 6361 6e20 7369  hether we can si
-00014b60: 6d70 6c69 6679 2073 6f6d 6520 6469 7669  mplify some divi
-00014b70: 7369 6f6e 2d74 6572 6d2e 0a20 2020 2020  sion-term..     
-00014b80: 2020 2020 2020 2066 6f72 2069 2c20 7465         for i, te
-00014b90: 726d 2069 6e20 7265 7665 7273 6564 286c  rm in reversed(l
-00014ba0: 6973 7428 656e 756d 6572 6174 6528 7365  ist(enumerate(se
-00014bb0: 6c66 2e74 6572 6d73 2929 2920 6966 2072  lf.terms))) if r
-00014bc0: 6967 6874 2065 6c73 6520 656e 756d 6572  ight else enumer
-00014bd0: 6174 6528 7365 6c66 2e74 6572 6d73 293a  ate(self.terms):
-00014be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014bf0: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-00014c00: 6365 2874 6572 6d2c 205f 642e 4469 6d29  ce(term, _d.Dim)
-00014c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014c20: 2069 6620 7465 726d 2e64 6572 6976 6564   if term.derived
-00014c30: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
-00014c40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014c50: 2074 6572 6d2e 6465 7269 7665 645f 6672   term.derived_fr
-00014c60: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
-00014c70: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
-00014c80: 6874 2220 6966 2072 6967 6874 2065 6c73  ht" if right els
-00014c90: 6520 226c 6566 7422 293a 0a20 2020 2020  e "left"):.     
-00014ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cb0: 2020 2069 6620 7465 726d 2e64 6572 6976     if term.deriv
-00014cc0: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
-00014cd0: 735b 2d31 5d20 3d3d 206f 7468 6572 3a0a  s[-1] == other:.
-00014ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cf0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00014d00: 726e 2069 0a20 2020 2020 2020 2020 2020  rn i.           
-00014d10: 2020 2020 2069 6620 6f74 6865 722e 6465       if other.de
-00014d20: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d40: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-00014d50: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
-00014d60: 203d 3d20 2274 7275 6564 6976 5f22 202b   == "truediv_" +
-00014d70: 2028 2272 6967 6874 2220 6966 206e 6f74   ("right" if not
-00014d80: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
-00014d90: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
-00014da0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00014db0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00014dc0: 6f6d 5f6f 702e 696e 7075 7473 5b2d 315d  om_op.inputs[-1]
-00014dd0: 203d 3d20 7465 726d 3a0a 2020 2020 2020   == term:.      
-00014de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014df0: 2020 2020 2020 7265 7475 726e 2069 0a20        return i. 
-00014e00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014e10: 6620 7465 726d 2e69 735f 636f 6e73 7461  f term.is_consta
-00014e20: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
-00014e30: 616e 6420 6f74 6865 722e 6973 5f63 6f6e  and other.is_con
-00014e40: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
-00014e50: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00014e60: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00014e70: 0a20 2020 2020 2020 2023 2046 6f72 2074  .        # For t
-00014e80: 6865 206c 6173 742f 6669 7273 7420 7465  he last/first te
-00014e90: 726d 2c20 6578 7472 6120 6368 6563 6b73  rm, extra checks
-00014ea0: 2e0a 2020 2020 2020 2020 6920 3d20 6c65  ..        i = le
-00014eb0: 6e28 7365 6c66 2e74 6572 6d73 2920 2d20  n(self.terms) - 
-00014ec0: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
-00014ed0: 300a 2020 2020 2020 2020 7465 726d 203d  0.        term =
-00014ee0: 2073 656c 662e 7465 726d 735b 695d 0a20   self.terms[i]. 
-00014ef0: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-00014f00: 6e64 7377 6974 6828 2264 6976 2229 2061  ndswith("div") a
-00014f10: 6e64 206f 7468 6572 203d 3d20 7465 726d  nd other == term
-00014f20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00014f30: 7475 726e 2069 0a20 2020 2020 2020 206f  turn i.        o
-00014f40: 705f 6b69 6e64 203d 206b 696e 6420 2b20  p_kind = kind + 
-00014f50: 225f 2220 2b20 2822 7269 6768 7422 2069  "_" + ("right" i
-00014f60: 6620 7269 6768 7420 656c 7365 2022 6c65  f right else "le
-00014f70: 6674 2229 0a20 2020 2020 2020 2069 6620  ft").        if 
-00014f80: 7465 726d 2e64 6572 6976 6564 5f66 726f  term.derived_fro
-00014f90: 6d5f 6f70 2061 6e64 2074 6572 6d2e 6465  m_op and term.de
-00014fa0: 7269 7665 645f 6672 6f6d 5f6f 702e 6b69  rived_from_op.ki
-00014fb0: 6e64 203d 3d20 6f70 5f6b 696e 643a 0a20  nd == op_kind:. 
-00014fc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014fd0: 6e20 690a 2020 2020 2020 2020 7265 7475  n i.        retu
-00014fe0: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
-00014ff0: 2065 7874 656e 645f 6d75 6c5f 6469 765f   extend_mul_div_
-00015000: 2873 656c 662c 206f 7468 6572 2c20 6b69  (self, other, ki
-00015010: 6e64 2c20 7269 6768 7429 3a0a 2020 2020  nd, right):.    
-00015020: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00015030: 3a70 6172 616d 2044 696d 206f 7468 6572  :param Dim other
-00015040: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-00015050: 2073 7472 206b 696e 643a 0a20 2020 2020   str kind:.     
-00015060: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
-00015070: 6967 6874 3a0a 2020 2020 2020 2020 2222  ight:.        ""
-00015080: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00015090: 206b 696e 6420 696e 207b 226d 756c 222c   kind in {"mul",
-000150a0: 2022 666c 6f6f 7264 6976 222c 2022 7472   "floordiv", "tr
-000150b0: 7565 6469 7622 2c20 2263 6569 6c64 6976  uediv", "ceildiv
-000150c0: 227d 0a20 2020 2020 2020 2069 6620 6f74  "}.        if ot
-000150d0: 6865 722e 6973 5f63 6f6e 7374 616e 745f  her.is_constant_
-000150e0: 7374 6174 6963 5f64 696d 2829 2061 6e64  static_dim() and
-000150f0: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
-00015100: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-00015110: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00015120: 2020 6966 206e 6f74 2073 656c 662e 7465    if not self.te
-00015130: 726d 733a 0a20 2020 2020 2020 2020 2020  rms:.           
-00015140: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
-00015150: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00015160: 2020 2073 656c 662e 7465 726d 732e 6170     self.terms.ap
-00015170: 7065 6e64 286f 7468 6572 290a 2020 2020  pend(other).    
-00015180: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
-00015190: 642e 656e 6473 7769 7468 2822 6469 7622  d.endswith("div"
-000151a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000151b0: 2020 2073 656c 662e 7465 726d 7320 3d20     self.terms = 
-000151c0: 5b5f 4f70 4d75 6c74 5465 726d 2e6e 6577  [_OpMultTerm.new
-000151d0: 5f64 6976 5f64 696d 2873 656c 662e 6173  _div_dim(self.as
-000151e0: 5f64 696d 2829 2c20 6f74 6865 722c 206b  _dim(), other, k
-000151f0: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
-00015200: 7269 6768 7429 5d0a 2020 2020 2020 2020  right)].        
-00015210: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00015220: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-00015230: 7665 645f 6672 6f6d 5f6f 7020 616e 6420  ved_from_op and 
-00015240: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00015250: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 226d  om_op.kind == "m
-00015260: 756c 223a 0a20 2020 2020 2020 2020 2020  ul":.           
-00015270: 2066 6f72 2074 6572 6d20 696e 206f 7468   for term in oth
-00015280: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
-00015290: 6f70 2e69 6e70 7574 7320 6966 2072 6967  op.inputs if rig
-000152a0: 6874 2065 6c73 6520 7265 7665 7273 6564  ht else reversed
-000152b0: 286f 7468 6572 2e64 6572 6976 6564 5f66  (other.derived_f
-000152c0: 726f 6d5f 6f70 2e69 6e70 7574 7329 3a0a  rom_op.inputs):.
-000152d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152e0: 7365 6c66 2e65 7874 656e 645f 6d75 6c5f  self.extend_mul_
-000152f0: 6469 765f 2874 6572 6d2c 206b 696e 643d  div_(term, kind=
-00015300: 6b69 6e64 2c20 7269 6768 743d 7269 6768  kind, right=righ
-00015310: 7429 0a20 2020 2020 2020 2020 2020 2072  t).            r
-00015320: 6574 7572 6e0a 2020 2020 2020 2020 6964  eturn.        id
-00015330: 7820 3d20 7365 6c66 2e5f 7369 6d70 6c69  x = self._simpli
-00015340: 6679 5f74 6572 6d5f 6964 7828 6f74 6865  fy_term_idx(othe
-00015350: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
-00015360: 6768 743d 7269 6768 7429 0a20 2020 2020  ght=right).     
-00015370: 2020 2069 6620 6964 7820 6973 206e 6f74     if idx is not
-00015380: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00015390: 2020 2074 6572 6d20 3d20 7365 6c66 2e74     term = self.t
-000153a0: 6572 6d73 5b69 6478 5d0a 2020 2020 2020  erms[idx].      
-000153b0: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-000153c0: 6e73 7461 6e63 6528 7465 726d 2c20 5f64  nstance(term, _d
-000153d0: 2e44 696d 290a 2020 2020 2020 2020 2020  .Dim).          
-000153e0: 2020 6966 206b 696e 642e 656e 6473 7769    if kind.endswi
-000153f0: 7468 2822 6469 7622 2920 616e 6420 6f74  th("div") and ot
-00015400: 6865 7220 3d3d 2074 6572 6d3a 0a20 2020  her == term:.   
-00015410: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015420: 662e 7465 726d 732e 706f 7028 6964 7829  f.terms.pop(idx)
-00015430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015440: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00015450: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
-00015460: 6d75 6c22 2061 6e64 2074 6572 6d2e 6465  mul" and term.de
-00015470: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-00015480: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015490: 6620 7465 726d 2e64 6572 6976 6564 5f66  f term.derived_f
-000154a0: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-000154b0: 7472 7565 6469 765f 2220 2b20 2822 7269  truediv_" + ("ri
-000154c0: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
-000154d0: 7365 2022 6c65 6674 2229 3a0a 2020 2020  se "left"):.    
-000154e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154f0: 6966 2074 6572 6d2e 6465 7269 7665 645f  if term.derived_
-00015500: 6672 6f6d 5f6f 702e 696e 7075 7473 5b2d  from_op.inputs[-
-00015510: 315d 203d 3d20 6f74 6865 723a 0a20 2020  1] == other:.   
-00015520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015530: 2020 2020 2073 656c 662e 7465 726d 735b       self.terms[
-00015540: 6964 785d 203d 2074 6572 6d2e 6465 7269  idx] = term.deri
-00015550: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-00015560: 7473 5b30 5d0a 2020 2020 2020 2020 2020  ts[0].          
-00015570: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015580: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00015590: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
-000155a0: 2220 616e 6420 6f74 6865 722e 6465 7269  " and other.deri
-000155b0: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
-000155c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000155d0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-000155e0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
-000155f0: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
-00015600: 6874 2220 6966 206e 6f74 2072 6967 6874  ht" if not right
-00015610: 2065 6c73 6520 226c 6566 7422 293a 0a20   else "left"):. 
-00015620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015630: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-00015640: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-00015650: 7473 5b2d 315d 203d 3d20 7465 726d 3a0a  ts[-1] == term:.
-00015660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015670: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-00015680: 6d73 5b69 6478 5d20 3d20 6f74 6865 722e  ms[idx] = other.
-00015690: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-000156a0: 696e 7075 7473 5b30 5d0a 2020 2020 2020  inputs[0].      
-000156b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156c0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-000156d0: 2020 2020 2069 6620 7465 726d 2e69 735f       if term.is_
-000156e0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-000156f0: 6469 6d28 2920 616e 6420 6f74 6865 722e  dim() and other.
-00015700: 6973 5f63 6f6e 7374 616e 745f 7374 6174  is_constant_stat
-00015710: 6963 5f64 696d 2829 3a0a 2020 2020 2020  ic_dim():.      
-00015720: 2020 2020 2020 2020 2020 6966 206b 696e            if kin
-00015730: 6420 3d3d 2022 6d75 6c22 3a0a 2020 2020  d == "mul":.    
-00015740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015750: 6966 2074 6572 6d2e 6469 6d65 6e73 696f  if term.dimensio
-00015760: 6e20 2a20 6f74 6865 722e 6469 6d65 6e73  n * other.dimens
-00015770: 696f 6e20 3d3d 2031 3a0a 2020 2020 2020  ion == 1:.      
-00015780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015790: 2020 7365 6c66 2e74 6572 6d73 2e70 6f70    self.terms.pop
-000157a0: 2869 6478 290a 2020 2020 2020 2020 2020  (idx).          
-000157b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000157c0: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-000157d0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-000157e0: 726d 735b 6964 785d 203d 205f 6d61 6b65  rms[idx] = _make
-000157f0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-00015800: 5f64 696d 2874 6572 6d2e 6469 6d65 6e73  _dim(term.dimens
-00015810: 696f 6e20 2a20 6f74 6865 722e 6469 6d65  ion * other.dime
-00015820: 6e73 696f 6e2c 206b 696e 643d 7465 726d  nsion, kind=term
-00015830: 2e6b 696e 6429 0a20 2020 2020 2020 2020  .kind).         
-00015840: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015850: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00015860: 2020 6966 206b 696e 642e 656e 6473 7769    if kind.endswi
-00015870: 7468 2822 6469 7622 2920 616e 6420 7465  th("div") and te
-00015880: 726d 2e64 696d 656e 7369 6f6e 2025 206f  rm.dimension % o
-00015890: 7468 6572 2e64 696d 656e 7369 6f6e 203d  ther.dimension =
-000158a0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-000158b0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-000158c0: 726d 735b 6964 785d 203d 205f 6d61 6b65  rms[idx] = _make
-000158d0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-000158e0: 5f64 696d 2874 6572 6d2e 6469 6d65 6e73  _dim(term.dimens
-000158f0: 696f 6e20 2f2f 206f 7468 6572 2e64 696d  ion // other.dim
-00015900: 656e 7369 6f6e 2c20 6b69 6e64 3d74 6572  ension, kind=ter
-00015910: 6d2e 6b69 6e64 290a 2020 2020 2020 2020  m.kind).        
-00015920: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015930: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
-00015940: 2020 2023 2046 616c 6c62 6163 6b20 7769     # Fallback wi
-00015950: 7468 2067 656e 6572 6963 2068 616e 646c  th generic handl
-00015960: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
-00015970: 206f 705f 6b69 6e64 203d 206b 696e 6420   op_kind = kind 
-00015980: 2b20 225f 2220 2b20 2822 7269 6768 7422  + "_" + ("right"
-00015990: 2069 6620 7269 6768 7420 656c 7365 2022   if right else "
-000159a0: 6c65 6674 2229 0a20 2020 2020 2020 2020  left").         
-000159b0: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
-000159c0: 6974 6828 2264 6976 2229 2061 6e64 2074  ith("div") and t
-000159d0: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
-000159e0: 5f6f 7020 616e 6420 7465 726d 2e64 6572  _op and term.der
-000159f0: 6976 6564 5f66 726f 6d5f 6f70 2e6b 696e  ived_from_op.kin
-00015a00: 6420 3d3d 206f 705f 6b69 6e64 3a0a 2020  d == op_kind:.  
-00015a10: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00015a20: 6d65 7261 746f 7220 3d20 7465 726d 2e64  merator = term.d
-00015a30: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
-00015a40: 6e70 7574 735b 305d 0a20 2020 2020 2020  nputs[0].       
-00015a50: 2020 2020 2020 2020 2064 656e 6f6d 696e           denomin
-00015a60: 6174 6f72 203d 2074 6572 6d2e 6465 7269  ator = term.deri
-00015a70: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-00015a80: 7473 5b31 5d0a 2020 2020 2020 2020 2020  ts[1].          
-00015a90: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00015aa0: 5b69 6478 5d20 3d20 5f4f 704d 756c 7454  [idx] = _OpMultT
-00015ab0: 6572 6d2e 6e65 775f 6469 765f 6469 6d28  erm.new_div_dim(
-00015ac0: 6e75 6d65 7261 746f 722c 2064 656e 6f6d  numerator, denom
-00015ad0: 696e 6174 6f72 202a 206f 7468 6572 2c20  inator * other, 
-00015ae0: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00015af0: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
-00015b00: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00015b10: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-00015b20: 6e64 7377 6974 6828 2264 6976 2229 3a0a  ndswith("div"):.
-00015b30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015b40: 2e74 6572 6d73 203d 205b 5f4f 704d 756c  .terms = [_OpMul
-00015b50: 7454 6572 6d2e 6e65 775f 6469 765f 6469  tTerm.new_div_di
-00015b60: 6d28 7365 6c66 2e61 735f 6469 6d28 292c  m(self.as_dim(),
-00015b70: 206f 7468 6572 2c20 6b69 6e64 3d6b 696e   other, kind=kin
-00015b80: 642c 2072 6967 6874 3d72 6967 6874 295d  d, right=right)]
-00015b90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00015ba0: 7572 6e0a 2020 2020 2020 2020 6966 206b  urn.        if k
-00015bb0: 696e 6420 3d3d 2022 6d75 6c22 3a0a 2020  ind == "mul":.  
-00015bc0: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
-00015bd0: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
-00015be0: 2020 2020 7365 6c66 2e74 6572 6d73 2e61      self.terms.a
-00015bf0: 7070 656e 6428 6f74 6865 7229 0a20 2020  ppend(other).   
-00015c00: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00015c10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015c20: 656c 662e 7465 726d 732e 696e 7365 7274  elf.terms.insert
-00015c30: 2830 2c20 6f74 6865 7229 0a20 2020 2020  (0, other).     
-00015c40: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00015c50: 2020 2020 2020 6173 7365 7274 2046 616c        assert Fal
-00015c60: 7365 0a0a 2020 2020 4063 6c61 7373 6d65  se..    @classme
-00015c70: 7468 6f64 0a20 2020 2064 6566 206e 6577  thod.    def new
-00015c80: 5f64 6976 5f64 696d 2863 6c73 2c20 6e75  _div_dim(cls, nu
-00015c90: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
-00015ca0: 6174 6f72 2c20 6b69 6e64 2c20 7269 6768  ator, kind, righ
-00015cb0: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
-00015cc0: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-00015cd0: 696d 206e 756d 6572 6174 6f72 3a0a 2020  im numerator:.  
-00015ce0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00015cf0: 2064 656e 6f6d 696e 6174 6f72 3a0a 2020   denominator:.  
-00015d00: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
-00015d10: 206b 696e 643a 2022 666c 6f6f 7264 6976   kind: "floordiv
-00015d20: 2220 6f72 2022 6365 696c 6469 7622 206f  " or "ceildiv" o
-00015d30: 7220 2274 7275 6564 6976 220a 2020 2020  r "truediv".    
-00015d40: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-00015d50: 7269 6768 743a 0a20 2020 2020 2020 203a  right:.        :
-00015d60: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00015d70: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
-00015d80: 696d 5f76 616c 7565 203d 204e 6f6e 650a  im_value = None.
-00015d90: 2020 2020 2020 2020 6120 3d20 6e75 6d65          a = nume
-00015da0: 7261 746f 722e 6469 6d65 6e73 696f 6e0a  rator.dimension.
-00015db0: 2020 2020 2020 2020 6220 3d20 6465 6e6f          b = deno
-00015dc0: 6d69 6e61 746f 722e 6469 6d65 6e73 696f  minator.dimensio
-00015dd0: 6e0a 2020 2020 2020 2020 6966 2061 2069  n.        if a i
-00015de0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2062  s not None and b
-00015df0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00015e00: 2020 2020 2020 2020 2020 6966 206b 696e            if kin
-00015e10: 6420 3d3d 2022 666c 6f6f 7264 6976 223a  d == "floordiv":
-00015e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015e30: 2064 696d 5f76 616c 7565 203d 2061 202f   dim_value = a /
-00015e40: 2f20 620a 2020 2020 2020 2020 2020 2020  / b.            
-00015e50: 656c 6966 206b 696e 6420 3d3d 2022 6365  elif kind == "ce
-00015e60: 696c 6469 7622 3a0a 2020 2020 2020 2020  ildiv":.        
-00015e70: 2020 2020 2020 2020 6469 6d5f 7661 6c75          dim_valu
-00015e80: 6520 3d20 2d28 2d61 202f 2f20 6229 0a20  e = -(-a // b). 
-00015e90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015ea0: 6620 6120 2520 6220 3d3d 2030 2061 6e64  f a % b == 0 and
-00015eb0: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-00015ec0: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
-00015ed0: 203d 2022 666c 6f6f 7264 6976 2220 2023   = "floordiv"  #
-00015ee0: 2066 6f72 206e 6963 6572 2064 6573 6372   for nicer descr
-00015ef0: 6970 7469 6f6e 2c20 616e 6420 646f 6573  iption, and does
-00015f00: 206e 6f74 206d 6174 7465 720a 2020 2020   not matter.    
-00015f10: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
-00015f20: 6420 3d3d 2022 7472 7565 6469 7622 3a0a  d == "truediv":.
-00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f40: 6966 2061 2025 2062 2021 3d20 303a 0a20  if a % b != 0:. 
-00015f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f60: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00015f70: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00015f80: 2020 2020 2020 2020 2020 2020 2022 2573               "%s
-00015f90: 2074 7275 6564 6976 2025 7320 6f6e 6c79   truediv %s only
-00015fa0: 2061 6c6c 6f77 6564 2069 6620 7468 6520   allowed if the 
-00015fb0: 7265 7375 6c74 2069 7320 616e 2069 6e74  result is an int
-00015fc0: 6567 6572 2220 2520 286e 756d 6572 6174  eger" % (numerat
-00015fd0: 6f72 2c20 6465 6e6f 6d69 6e61 746f 7229  or, denominator)
-00015fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ff0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00016000: 2020 2020 2020 2064 696d 5f76 616c 7565         dim_value
-00016010: 203d 2061 202f 2f20 620a 2020 2020 2020   = a // b.      
-00016020: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
-00016030: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
-00016040: 2020 2020 2020 2020 6b69 6e64 203d 2022          kind = "
-00016050: 666c 6f6f 7264 6976 2220 2023 2066 6f72  floordiv"  # for
-00016060: 206e 6963 6572 2064 6573 6372 6970 7469   nicer descripti
-00016070: 6f6e 2c20 616e 6420 646f 6573 206e 6f74  on, and does not
-00016080: 206d 6174 7465 720a 2020 2020 2020 2020   matter.        
-00016090: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000160a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000160b0: 5661 6c75 6545 7272 6f72 2822 696e 7661  ValueError("inva
-000160c0: 6c69 6420 6b69 6e64 2025 7222 2025 2028  lid kind %r" % (
-000160d0: 6b69 6e64 2c29 290a 2020 2020 2020 2020  kind,)).        
-000160e0: 6966 206b 696e 6420 3d3d 2022 666c 6f6f  if kind == "floo
-000160f0: 7264 6976 2220 616e 6420 7269 6768 743a  rdiv" and right:
-00016100: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00016110: 6372 6970 7469 6f6e 203d 2022 2573 2f2f  cription = "%s//
-00016120: 2573 2220 2520 285f 6765 745f 6465 7363  %s" % (_get_desc
-00016130: 7269 7074 696f 6e28 6e75 6d65 7261 746f  ription(numerato
-00016140: 7229 2c20 5f67 6574 5f64 6573 6372 6970  r), _get_descrip
-00016150: 7469 6f6e 2864 656e 6f6d 696e 6174 6f72  tion(denominator
-00016160: 2929 0a20 2020 2020 2020 2065 6c69 6620  )).        elif 
-00016170: 6b69 6e64 203d 3d20 2263 6569 6c64 6976  kind == "ceildiv
-00016180: 2220 616e 6420 7269 6768 743a 0a20 2020  " and right:.   
-00016190: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-000161a0: 7469 6f6e 203d 2022 e28c 8825 732f 2573  tion = "...%s/%s
-000161b0: e28c 8922 2025 2028 5f67 6574 5f64 6573  ..." % (_get_des
-000161c0: 6372 6970 7469 6f6e 286e 756d 6572 6174  cription(numerat
-000161d0: 6f72 292c 205f 6765 745f 6465 7363 7269  or), _get_descri
-000161e0: 7074 696f 6e28 6465 6e6f 6d69 6e61 746f  ption(denominato
-000161f0: 7229 290a 2020 2020 2020 2020 656c 7365  r)).        else
-00016200: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-00016210: 7363 7269 7074 696f 6e20 3d20 2225 735f  scription = "%s_
-00016220: 2573 2825 732c 2025 7329 2220 2520 280a  %s(%s, %s)" % (.
-00016230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016240: 6b69 6e64 2c0a 2020 2020 2020 2020 2020  kind,.          
-00016250: 2020 2020 2020 2272 6967 6874 2220 6966        "right" if
-00016260: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
-00016270: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00016280: 2020 2020 5f67 6574 5f64 6573 6372 6970      _get_descrip
-00016290: 7469 6f6e 286e 756d 6572 6174 6f72 2c20  tion(numerator, 
-000162a0: 6272 6163 6b65 7473 3d46 616c 7365 292c  brackets=False),
-000162b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000162c0: 205f 6765 745f 6465 7363 7269 7074 696f   _get_descriptio
-000162d0: 6e28 6465 6e6f 6d69 6e61 746f 722c 2062  n(denominator, b
-000162e0: 7261 636b 6574 733d 4661 6c73 6529 2c0a  rackets=False),.
-000162f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00016300: 2020 2020 2020 6f70 5f6b 696e 6420 3d20        op_kind = 
-00016310: 6b69 6e64 0a20 2020 2020 2020 2069 6620  kind.        if 
-00016320: 6120 6973 206e 6f74 204e 6f6e 6520 616e  a is not None an
-00016330: 6420 6220 6973 206e 6f74 204e 6f6e 6520  d b is not None 
-00016340: 616e 6420 6120 2520 6220 3d3d 2030 3a0a  and a % b == 0:.
-00016350: 2020 2020 2020 2020 2020 2020 6f70 5f6b              op_k
-00016360: 696e 6420 3d20 2274 7275 6564 6976 2220  ind = "truediv" 
-00016370: 2023 206d 616b 6573 2073 6f6d 6520 6f74   # makes some ot
-00016380: 6865 7220 6368 6563 6b73 2073 696d 706c  her checks simpl
-00016390: 6572 0a20 2020 2020 2020 206f 705f 6b69  er.        op_ki
-000163a0: 6e64 202b 3d20 225f 2220 2b20 2822 7269  nd += "_" + ("ri
-000163b0: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
-000163c0: 7365 2022 6c65 6674 2229 0a20 2020 2020  se "left").     
-000163d0: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
-000163e0: 280a 2020 2020 2020 2020 2020 2020 6465  (.            de
-000163f0: 7363 7269 7074 696f 6e3d 6465 7363 7269  scription=descri
-00016400: 7074 696f 6e2c 0a20 2020 2020 2020 2020  ption,.         
-00016410: 2020 206b 696e 643d 6e75 6d65 7261 746f     kind=numerato
-00016420: 722e 6b69 6e64 2c0a 2020 2020 2020 2020  r.kind,.        
-00016430: 2020 2020 6469 6d65 6e73 696f 6e3d 6469      dimension=di
-00016440: 6d5f 7661 6c75 652c 0a20 2020 2020 2020  m_value,.       
-00016450: 2020 2020 2064 6572 6976 6564 5f66 726f       derived_fro
-00016460: 6d5f 6f70 3d4f 7028 6b69 6e64 3d6f 705f  m_op=Op(kind=op_
-00016470: 6b69 6e64 2c20 696e 7075 7473 3d5b 6e75  kind, inputs=[nu
-00016480: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
-00016490: 6174 6f72 5d29 2c0a 2020 2020 2020 2020  ator]),.        
-000164a0: 2020 2020 6465 7269 7665 645f 6672 6f6d      derived_from
-000164b0: 5f74 6167 3d6e 756d 6572 6174 6f72 2c0a  _tag=numerator,.
-000164c0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-000164d0: 6566 2061 735f 6469 6d28 7365 6c66 293a  ef as_dim(self):
-000164e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000164f0: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00016500: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016510: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
-00016520: 6f6e 6528 293a 0a20 2020 2020 2020 2020  one():.         
-00016530: 2020 2072 6574 7572 6e20 5f6d 616b 655f     return _make_
-00016540: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-00016550: 6469 6d28 3129 0a20 2020 2020 2020 2069  dim(1).        i
-00016560: 6620 6c65 6e28 7365 6c66 2e74 6572 6d73  f len(self.terms
-00016570: 2920 3d3d 2031 3a0a 2020 2020 2020 2020  ) == 1:.        
-00016580: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00016590: 7465 726d 735b 305d 0a20 2020 2020 2020  terms[0].       
-000165a0: 2064 696d 5f6b 696e 6420 3d20 5f67 6574   dim_kind = _get
-000165b0: 5f6d 6572 6765 645f 6469 6d5f 6b69 6e64  _merged_dim_kind
-000165c0: 2873 656c 662e 7465 726d 7329 0a20 2020  (self.terms).   
-000165d0: 2020 2020 2072 6574 7572 6e20 5f64 2e44       return _d.D
-000165e0: 696d 280a 2020 2020 2020 2020 2020 2020  im(.            
-000165f0: 6b69 6e64 3d64 696d 5f6b 696e 642c 0a20  kind=dim_kind,. 
-00016600: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00016610: 6970 7469 6f6e 3d22 2a22 2e6a 6f69 6e28  iption="*".join(
-00016620: 6d61 7028 5f67 6574 5f64 6573 6372 6970  map(_get_descrip
-00016630: 7469 6f6e 2c20 7365 6c66 2e74 6572 6d73  tion, self.terms
-00016640: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-00016650: 6469 6d65 6e73 696f 6e3d 7365 6c66 2e64  dimension=self.d
-00016660: 696d 656e 7369 6f6e 2c0a 2020 2020 2020  imension,.      
-00016670: 2020 2020 2020 6465 7269 7665 645f 6672        derived_fr
-00016680: 6f6d 5f6f 703d 4f70 286b 696e 643d 226d  om_op=Op(kind="m
-00016690: 756c 222c 2069 6e70 7574 733d 6c69 7374  ul", inputs=list
-000166a0: 2873 656c 662e 7465 726d 7329 292c 0a20  (self.terms)),. 
-000166b0: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
-000166c0: 6564 5f66 726f 6d5f 7461 673d 7365 6c66  ed_from_tag=self
-000166d0: 2e72 6570 7265 7365 6e74 6174 6976 655f  .representative_
-000166e0: 7461 6728 292c 0a20 2020 2020 2020 2029  tag(),.        )
-000166f0: 0a0a 2020 2020 6465 6620 7265 7072 6573  ..    def repres
-00016700: 656e 7461 7469 7665 5f74 6167 2873 656c  entative_tag(sel
-00016710: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-00016720: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00016730: 4469 6d7c 4e6f 6e65 0a20 2020 2020 2020  Dim|None.       
-00016740: 2022 2222 0a20 2020 2020 2020 2023 2041   """.        # A
-00016750: 6c73 6f20 7365 6520 4469 6d2e 5f4f 704c  lso see Dim._OpL
-00016760: 696e 6561 7254 6572 6d2e 7265 7072 6573  inearTerm.repres
-00016770: 656e 7461 7469 7665 5f74 6167 2829 2e0a  entative_tag()..
-00016780: 2020 2020 2020 2020 2320 4669 7273 7420          # First 
-00016790: 6669 6e64 2061 6e79 2064 796e 616d 6963  find any dynamic
-000167a0: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
-000167b0: 726d 5f20 696e 2073 656c 662e 7465 726d  rm_ in self.term
-000167c0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-000167d0: 6620 7465 726d 5f2e 6973 5f64 796e 616d  f term_.is_dynam
-000167e0: 6963 2829 3a0a 2020 2020 2020 2020 2020  ic():.          
-000167f0: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-00016800: 6d5f 0a20 2020 2020 2020 2023 204e 6f77  m_.        # Now
-00016810: 2066 696e 6420 6e6f 6e2d 756e 7370 6563   find non-unspec
-00016820: 6966 6965 642e 0a20 2020 2020 2020 2066  ified..        f
-00016830: 6f72 2074 6572 6d5f 2069 6e20 7365 6c66  or term_ in self
-00016840: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00016850: 2020 2020 6966 2074 6572 6d5f 2e6b 696e      if term_.kin
-00016860: 6420 213d 2044 696d 5479 7065 732e 556e  d != DimTypes.Un
-00016870: 7370 6563 6966 6965 643a 0a20 2020 2020  specified:.     
-00016880: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00016890: 6e20 7465 726d 5f0a 2020 2020 2020 2020  n term_.        
-000168a0: 2320 4e6f 7720 6669 6e64 2061 6e79 2e0a  # Now find any..
-000168b0: 2020 2020 2020 2020 666f 7220 7465 726d          for term
-000168c0: 5f20 696e 2073 656c 662e 7465 726d 733a  _ in self.terms:
-000168d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000168e0: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
-000168f0: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
-00016900: 636c 6173 7320 5f4f 704c 696e 6561 7254  class _OpLinearT
-00016910: 6572 6d3a 0a20 2020 2022 2222 0a20 2020  erm:.    """.   
-00016920: 2072 6570 7265 7365 6e74 7320 7374 6820   represents sth 
-00016930: 6c69 6b65 2061 202a 2062 202b 2063 0a20  like a * b + c. 
-00016940: 2020 2022 2222 0a0a 2020 2020 4063 6c61     """..    @cla
-00016950: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00016960: 2066 726f 6d5f 6469 6d28 636c 732c 2064   from_dim(cls, d
-00016970: 696d 293a 0a20 2020 2020 2020 2022 2222  im):.        """
-00016980: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00016990: 4469 6d20 6469 6d3a 0a20 2020 2020 2020  Dim dim:.       
-000169a0: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
-000169b0: 4c69 6e65 6172 5465 726d 0a20 2020 2020  LinearTerm.     
-000169c0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-000169d0: 6573 203d 2063 6c73 2e7a 6572 6f28 290a  es = cls.zero().
-000169e0: 2020 2020 2020 2020 7265 732e 6578 7465          res.exte
-000169f0: 6e64 5f61 6464 5f73 7562 5f28 6469 6d2c  nd_add_sub_(dim,
-00016a00: 206b 696e 643d 2261 6464 222c 2072 6967   kind="add", rig
-00016a10: 6874 3d54 7275 6529 0a20 2020 2020 2020  ht=True).       
-00016a20: 2072 6574 7572 6e20 7265 730a 0a20 2020   return res..   
-00016a30: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00016a40: 2020 6465 6620 7a65 726f 2863 6c73 293a    def zero(cls):
-00016a50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016a60: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00016a70: 2e5f 4f70 4c69 6e65 6172 5465 726d 0a20  ._OpLinearTerm. 
-00016a80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016a90: 2020 2072 6574 7572 6e20 5f4f 704c 696e     return _OpLin
-00016aa0: 6561 7254 6572 6d28 5b5d 290a 0a20 2020  earTerm([])..   
-00016ab0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00016ac0: 6c66 2c20 7465 726d 7329 3a0a 2020 2020  lf, terms):.    
-00016ad0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00016ae0: 3a70 6172 616d 206c 6973 745b 4469 6d2e  :param list[Dim.
-00016af0: 5f4f 704d 756c 7454 6572 6d5d 2074 6572  _OpMultTerm] ter
-00016b00: 6d73 3a0a 2020 2020 2020 2020 2222 220a  ms:.        """.
-00016b10: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-00016b20: 6d73 203d 2074 6572 6d73 0a0a 2020 2020  ms = terms..    
-00016b30: 6465 6620 5f5f 6861 7368 5f5f 2873 656c  def __hash__(sel
-00016b40: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00016b50: 726e 2068 6173 6828 7475 706c 6528 7365  rn hash(tuple(se
-00016b60: 6c66 2e74 6572 6d73 2929 0a0a 2020 2020  lf.terms))..    
-00016b70: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
-00016b80: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00016b90: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
-00016ba0: 7468 6572 2c20 5f4f 704c 696e 6561 7254  ther, _OpLinearT
-00016bb0: 6572 6d29 3a0a 2020 2020 2020 2020 2020  erm):.          
-00016bc0: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
-00016bd0: 726d 7320 3d3d 206f 7468 6572 2e74 6572  rms == other.ter
-00016be0: 6d73 0a20 2020 2020 2020 2072 6574 7572  ms.        retur
-00016bf0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00016c00: 205f 5f6e 655f 5f28 7365 6c66 2c20 6f74   __ne__(self, ot
-00016c10: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
-00016c20: 7475 726e 206e 6f74 2073 656c 662e 5f5f  turn not self.__
-00016c30: 6571 5f5f 286f 7468 6572 290a 0a20 2020  eq__(other)..   
-00016c40: 2064 6566 2061 735f 6469 6d28 7365 6c66   def as_dim(self
-00016c50: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00016c60: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00016c70: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-00016c80: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00016c90: 735f 7a65 726f 2829 3a0a 2020 2020 2020  s_zero():.      
-00016ca0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00016cb0: 6b65 5f63 6f6e 7374 616e 745f 7374 6174  ke_constant_stat
-00016cc0: 6963 5f64 696d 2830 290a 2020 2020 2020  ic_dim(0).      
-00016cd0: 2020 6966 206c 656e 2873 656c 662e 7465    if len(self.te
-00016ce0: 726d 7329 203d 3d20 313a 0a20 2020 2020  rms) == 1:.     
-00016cf0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00016d00: 6c66 2e74 6572 6d73 5b30 5d2e 6173 5f64  lf.terms[0].as_d
-00016d10: 696d 2829 0a20 2020 2020 2020 2061 6464  im().        add
-00016d20: 5f70 6172 7473 203d 205b 5d0a 2020 2020  _parts = [].    
-00016d30: 2020 2020 6465 7363 5f70 6172 7473 203d      desc_parts =
-00016d40: 205b 5d0a 2020 2020 2020 2020 6469 6d20   [].        dim 
-00016d50: 3d20 300a 2020 2020 2020 2020 666f 7220  = 0.        for 
-00016d60: 7465 726d 2069 6e20 7365 6c66 2e74 6572  term in self.ter
-00016d70: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00016d80: 7320 3d20 7465 726d 2e61 735f 6469 6d28  s = term.as_dim(
-00016d90: 290a 2020 2020 2020 2020 2020 2020 6164  ).            ad
-00016da0: 645f 7061 7274 732e 6170 7065 6e64 2873  d_parts.append(s
-00016db0: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
-00016dc0: 7363 5f70 6172 7473 2e61 7070 656e 6428  sc_parts.append(
-00016dd0: 5f67 6574 5f64 6573 6372 6970 7469 6f6e  _get_description
-00016de0: 2873 2929 0a20 2020 2020 2020 2020 2020  (s)).           
-00016df0: 2069 6620 6469 6d20 6973 206e 6f74 204e   if dim is not N
-00016e00: 6f6e 6520 616e 6420 732e 6469 6d65 6e73  one and s.dimens
-00016e10: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-00016e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016e30: 2064 696d 202b 3d20 732e 6469 6d65 6e73   dim += s.dimens
-00016e40: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00016e50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00016e60: 2020 2020 2020 6469 6d20 3d20 4e6f 6e65        dim = None
-00016e70: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00016e80: 6164 645f 7061 7274 7329 203d 3d20 313a  add_parts) == 1:
-00016e90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00016ea0: 7572 6e20 6164 645f 7061 7274 735b 305d  urn add_parts[0]
-00016eb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00016ec0: 5f64 2e44 696d 280a 2020 2020 2020 2020  _d.Dim(.        
-00016ed0: 2020 2020 6b69 6e64 3d5f 6765 745f 6d65      kind=_get_me
-00016ee0: 7267 6564 5f64 696d 5f6b 696e 6428 6164  rged_dim_kind(ad
-00016ef0: 645f 7061 7274 7329 2c0a 2020 2020 2020  d_parts),.      
-00016f00: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00016f10: 6e3d 222b 222e 6a6f 696e 2864 6573 635f  n="+".join(desc_
-00016f20: 7061 7274 7329 2c0a 2020 2020 2020 2020  parts),.        
-00016f30: 2020 2020 6469 6d65 6e73 696f 6e3d 6469      dimension=di
-00016f40: 6d2c 0a20 2020 2020 2020 2020 2020 2064  m,.            d
-00016f50: 6572 6976 6564 5f66 726f 6d5f 6f70 3d4f  erived_from_op=O
-00016f60: 7028 6b69 6e64 3d22 6164 6422 2c20 696e  p(kind="add", in
-00016f70: 7075 7473 3d61 6464 5f70 6172 7473 292c  puts=add_parts),
-00016f80: 0a20 2020 2020 2020 2020 2020 2064 6572  .            der
-00016f90: 6976 6564 5f66 726f 6d5f 7461 673d 7365  ived_from_tag=se
-00016fa0: 6c66 2e72 6570 7265 7365 6e74 6174 6976  lf.representativ
-00016fb0: 655f 7461 6728 292c 0a20 2020 2020 2020  e_tag(),.       
-00016fc0: 2029 0a0a 2020 2020 6465 6620 5f5f 7265   )..    def __re
-00016fd0: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-00016fe0: 2020 2020 7265 7475 726e 2022 4469 6d2e      return "Dim.
-00016ff0: 5f4f 704c 696e 6561 7254 6572 6d28 2572  _OpLinearTerm(%r
-00017000: 2922 2025 2028 7365 6c66 2e74 6572 6d73  )" % (self.terms
-00017010: 2c29 0a0a 2020 2020 6465 6620 6973 5f7a  ,)..    def is_z
-00017020: 6572 6f28 7365 6c66 293a 0a20 2020 2020  ero(self):.     
-00017030: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00017040: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-00017050: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00017060: 7265 7475 726e 206e 6f74 2073 656c 662e  return not self.
-00017070: 7465 726d 730a 0a20 2020 2064 6566 2065  terms..    def e
-00017080: 7874 656e 645f 6164 645f 7375 625f 2873  xtend_add_sub_(s
-00017090: 656c 662c 206f 7468 6572 2c20 6b69 6e64  elf, other, kind
-000170a0: 2c20 7269 6768 7429 3a0a 2020 2020 2020  , right):.      
-000170b0: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-000170c0: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
-000170d0: 6572 3a0a 2020 2020 2020 2020 3a70 6172  er:.        :par
-000170e0: 616d 2073 7472 206b 696e 643a 2022 6164  am str kind: "ad
-000170f0: 6422 206f 7220 2273 7562 220a 2020 2020  d" or "sub".    
-00017100: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-00017110: 7269 6768 743a 206f 7220 6c65 6674 2e20  right: or left. 
-00017120: 7269 6768 7420 6d65 616e 7320 7365 6c66  right means self
-00017130: 202b 206f 7468 6572 2c20 6c65 6674 206d   + other, left m
-00017140: 6561 6e73 206f 7468 6572 202b 2073 656c  eans other + sel
-00017150: 660a 2020 2020 2020 2020 2222 220a 2020  f.        """.  
-00017160: 2020 2020 2020 6173 7365 7274 206b 696e        assert kin
-00017170: 6420 696e 207b 2261 6464 222c 2022 7375  d in {"add", "su
-00017180: 6222 7d0a 2020 2020 2020 2020 6f74 6865  b"}.        othe
-00017190: 7220 3d20 7365 6c66 2e5f 6d61 6b65 5f64  r = self._make_d
-000171a0: 696d 286f 7468 6572 2c20 6b69 6e64 3d6b  im(other, kind=k
-000171b0: 696e 6429 0a20 2020 2020 2020 2069 6620  ind).        if 
-000171c0: 6f74 6865 722e 6973 5f63 6f6e 7374 616e  other.is_constan
-000171d0: 745f 7374 6174 6963 5f64 696d 2829 2061  t_static_dim() a
-000171e0: 6e64 206f 7468 6572 2e64 696d 656e 7369  nd other.dimensi
-000171f0: 6f6e 203d 3d20 303a 0a20 2020 2020 2020  on == 0:.       
-00017200: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00017210: 2020 2020 6966 206f 7468 6572 2e64 6572      if other.der
-00017220: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
-00017230: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
-00017240: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-00017250: 6164 6422 3a0a 2020 2020 2020 2020 2020  add":.          
-00017260: 2020 666f 7220 6f74 6865 725f 2069 6e20    for other_ in 
-00017270: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00017280: 6f6d 5f6f 702e 696e 7075 7473 2069 6620  om_op.inputs if 
-00017290: 7269 6768 7420 656c 7365 2072 6576 6572  right else rever
-000172a0: 7365 6428 6f74 6865 722e 6465 7269 7665  sed(other.derive
-000172b0: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
-000172c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000172d0: 2020 2073 656c 662e 6578 7465 6e64 5f61     self.extend_a
-000172e0: 6464 5f73 7562 5f28 6f74 6865 725f 2c20  dd_sub_(other_, 
-000172f0: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00017300: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
-00017310: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00017320: 2020 2074 6572 6d20 3d20 5f4f 704d 756c     term = _OpMul
-00017330: 7454 6572 6d2e 6672 6f6d 5f64 696d 286f  tTerm.from_dim(o
-00017340: 7468 6572 290a 2020 2020 2020 2020 6e65  ther).        ne
-00017350: 675f 7465 726d 203d 2074 6572 6d2e 6e65  g_term = term.ne
-00017360: 6761 7469 7665 2829 0a20 2020 2020 2020  gative().       
-00017370: 2069 6620 6b69 6e64 203d 3d20 2273 7562   if kind == "sub
-00017380: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
-00017390: 6572 6d2c 206e 6567 5f74 6572 6d20 3d20  erm, neg_term = 
-000173a0: 6e65 675f 7465 726d 2c20 7465 726d 0a20  neg_term, term. 
-000173b0: 2020 2020 2020 206d 6f73 745f 7265 6365         most_rece
-000173c0: 6e74 5f74 6572 6d20 3d20 7365 6c66 2e74  nt_term = self.t
-000173d0: 6572 6d73 5b2d 3120 6966 2072 6967 6874  erms[-1 if right
-000173e0: 2065 6c73 6520 305d 2069 6620 7365 6c66   else 0] if self
-000173f0: 2e74 6572 6d73 2065 6c73 6520 4e6f 6e65  .terms else None
-00017400: 0a20 2020 2020 2020 2069 6620 6d6f 7374  .        if most
-00017410: 5f72 6563 656e 745f 7465 726d 3a0a 2020  _recent_term:.  
-00017420: 2020 2020 2020 2020 2020 6966 206d 6f73            if mos
-00017430: 745f 7265 6365 6e74 5f74 6572 6d20 3d3d  t_recent_term ==
-00017440: 206e 6567 5f74 6572 6d3a 0a20 2020 2020   neg_term:.     
-00017450: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017460: 7465 726d 732e 706f 7028 2d31 2069 6620  terms.pop(-1 if 
-00017470: 7269 6768 7420 656c 7365 2030 290a 2020  right else 0).  
-00017480: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00017490: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-000174a0: 2069 6620 6d6f 7374 5f72 6563 656e 745f   if most_recent_
-000174b0: 7465 726d 2e69 735f 636f 6e73 7461 6e74  term.is_constant
-000174c0: 5f73 7461 7469 635f 6469 6d28 2920 616e  _static_dim() an
-000174d0: 6420 7465 726d 2e69 735f 636f 6e73 7461  d term.is_consta
-000174e0: 6e74 5f73 7461 7469 635f 6469 6d28 293a  nt_static_dim():
-000174f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017500: 2073 656c 662e 7465 726d 735b 2d31 2069   self.terms[-1 i
-00017510: 6620 7269 6768 7420 656c 7365 2030 5d20  f right else 0] 
-00017520: 3d20 5f4f 704d 756c 7454 6572 6d2e 6672  = _OpMultTerm.fr
-00017530: 6f6d 5f64 696d 280a 2020 2020 2020 2020  om_dim(.        
-00017540: 2020 2020 2020 2020 2020 2020 5f6d 616b              _mak
-00017550: 655f 636f 6e73 7461 6e74 5f73 7461 7469  e_constant_stati
-00017560: 635f 6469 6d28 6d6f 7374 5f72 6563 656e  c_dim(most_recen
-00017570: 745f 7465 726d 2e64 696d 656e 7369 6f6e  t_term.dimension
-00017580: 202b 2074 6572 6d2e 6469 6d65 6e73 696f   + term.dimensio
-00017590: 6e2c 206b 696e 643d 6f74 6865 722e 6b69  n, kind=other.ki
-000175a0: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
-000175b0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000175c0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-000175d0: 2020 2020 2020 2020 2069 6620 6d6f 7374           if most
-000175e0: 5f72 6563 656e 745f 7465 726d 2e74 6572  _recent_term.ter
-000175f0: 6d73 2061 6e64 2074 6572 6d2e 7465 726d  ms and term.term
-00017600: 7320 616e 6420 6d6f 7374 5f72 6563 656e  s and most_recen
-00017610: 745f 7465 726d 2e74 6572 6d73 5b2d 315d  t_term.terms[-1]
-00017620: 203d 3d20 7465 726d 2e74 6572 6d73 5b2d   == term.terms[-
-00017630: 315d 3a0a 2020 2020 2020 2020 2020 2020  1]:.            
-00017640: 2020 2020 2320 4d65 7267 6520 7465 726d      # Merge term
-00017650: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00017660: 2020 6120 3d20 5f4f 704d 756c 7454 6572    a = _OpMultTer
-00017670: 6d2e 6672 6f6d 5f64 696d 5f66 6163 746f  m.from_dim_facto
-00017680: 7273 286d 6f73 745f 7265 6365 6e74 5f74  rs(most_recent_t
-00017690: 6572 6d2e 7465 726d 735b 3a2d 315d 292e  erm.terms[:-1]).
-000176a0: 6173 5f64 696d 2829 0a20 2020 2020 2020  as_dim().       
-000176b0: 2020 2020 2020 2020 2062 203d 205f 4f70           b = _Op
-000176c0: 4d75 6c74 5465 726d 2e66 726f 6d5f 6469  MultTerm.from_di
-000176d0: 6d5f 6661 6374 6f72 7328 7465 726d 2e74  m_factors(term.t
-000176e0: 6572 6d73 5b3a 2d31 5d29 2e61 735f 6469  erms[:-1]).as_di
-000176f0: 6d28 290a 2020 2020 2020 2020 2020 2020  m().            
-00017700: 2020 2020 7265 7320 3d20 5f4f 704d 756c      res = _OpMul
-00017710: 7454 6572 6d2e 6672 6f6d 5f64 696d 2828  tTerm.from_dim((
-00017720: 6120 2b20 6229 2069 6620 7269 6768 7420  a + b) if right 
-00017730: 656c 7365 2028 6220 2b20 6129 290a 2020  else (b + a)).  
-00017740: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00017750: 732e 6578 7465 6e64 5f6d 756c 5f64 6976  s.extend_mul_div
-00017760: 5f28 7465 726d 2e74 6572 6d73 5b2d 315d  _(term.terms[-1]
-00017770: 2c20 6b69 6e64 3d22 6d75 6c22 2c20 7269  , kind="mul", ri
-00017780: 6768 743d 5472 7565 290a 2020 2020 2020  ght=True).      
-00017790: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000177a0: 6572 6d73 5b2d 3120 6966 2072 6967 6874  erms[-1 if right
-000177b0: 2065 6c73 6520 305d 203d 2072 6573 0a20   else 0] = res. 
-000177c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000177d0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-000177e0: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-000177f0: 2020 2020 7365 6c66 2e74 6572 6d73 2e61      self.terms.a
-00017800: 7070 656e 6428 7465 726d 290a 2020 2020  ppend(term).    
-00017810: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00017820: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00017830: 2e69 6e73 6572 7428 302c 2074 6572 6d29  .insert(0, term)
-00017840: 0a0a 2020 2020 6465 6620 6578 7465 6e64  ..    def extend
-00017850: 5f6d 756c 5f64 6976 5f28 7365 6c66 2c20  _mul_div_(self, 
-00017860: 6f74 6865 722c 206b 696e 642c 2072 6967  other, kind, rig
-00017870: 6874 293a 0a20 2020 2020 2020 2022 2222  ht):.        """
-00017880: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00017890: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-000178a0: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-000178b0: 7220 6b69 6e64 3a20 226d 756c 2220 6f72  r kind: "mul" or
-000178c0: 2022 6365 696c 6469 7622 0a20 2020 2020   "ceildiv".     
-000178d0: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
-000178e0: 6967 6874 3a20 6f72 206c 6566 742e 2072  ight: or left. r
-000178f0: 6967 6874 206d 6561 6e73 2073 656c 6620  ight means self 
-00017900: 2a20 6f74 6865 722c 206c 6566 7420 6d65  * other, left me
-00017910: 616e 7320 6f74 6865 7220 2a20 7365 6c66  ans other * self
-00017920: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00017930: 2020 2020 2061 7373 6572 7420 6b69 6e64       assert kind
-00017940: 2069 6e20 7b22 6d75 6c22 2c20 2266 6c6f   in {"mul", "flo
-00017950: 6f72 6469 7622 2c20 2274 7275 6564 6976  ordiv", "truediv
-00017960: 222c 2022 6365 696c 6469 7622 7d0a 2020  ", "ceildiv"}.  
-00017970: 2020 2020 2020 6f74 6865 7220 3d20 7365        other = se
-00017980: 6c66 2e5f 6d61 6b65 5f64 696d 286f 7468  lf._make_dim(oth
-00017990: 6572 2c20 6b69 6e64 3d6b 696e 6429 0a20  er, kind=kind). 
-000179a0: 2020 2020 2020 2069 6620 6b69 6e64 203d         if kind =
-000179b0: 3d20 226d 756c 2220 616e 6420 7269 6768  = "mul" and righ
-000179c0: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
-000179d0: 6620 6e6f 7420 616c 6c28 7465 726d 2e63  f not all(term.c
-000179e0: 616e 5f73 696d 706c 6966 7928 6f74 6865  an_simplify(othe
-000179f0: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
-00017a00: 6768 743d 7269 6768 7429 2066 6f72 2074  ght=right) for t
-00017a10: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
-00017a20: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00017a30: 2020 2020 2320 446f 2069 7420 7468 6520      # Do it the 
-00017a40: 6f74 6865 7220 7761 7920 6172 6f75 6e64  other way around
-00017a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017a60: 2073 656c 662e 7465 726d 732c 206f 7468   self.terms, oth
-00017a70: 6572 203d 205f 4f70 4c69 6e65 6172 5465  er = _OpLinearTe
-00017a80: 726d 2e66 726f 6d5f 6469 6d28 6f74 6865  rm.from_dim(othe
-00017a90: 7229 2e74 6572 6d73 2c20 7365 6c66 2e61  r).terms, self.a
-00017aa0: 735f 6469 6d28 290a 2020 2020 2020 2020  s_dim().        
-00017ab0: 2020 2020 2020 2020 7269 6768 7420 3d20          right = 
-00017ac0: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
-00017ad0: 206f 7468 6572 2e69 735f 636f 6e73 7461   other.is_consta
-00017ae0: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
-00017af0: 616e 6420 6f74 6865 722e 6469 6d65 6e73  and other.dimens
-00017b00: 696f 6e20 3d3d 2031 3a0a 2020 2020 2020  ion == 1:.      
-00017b10: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00017b20: 2020 2020 2069 6620 6b69 6e64 2e65 6e64       if kind.end
-00017b30: 7377 6974 6828 2264 6976 2229 2061 6e64  swith("div") and
-00017b40: 206c 656e 2873 656c 662e 7465 726d 7329   len(self.terms)
-00017b50: 203e 3d20 323a 0a20 2020 2020 2020 2020   >= 2:.         
-00017b60: 2020 2069 6620 616e 7928 6e6f 7420 7465     if any(not te
-00017b70: 726d 2e64 6976 6973 6962 6c65 286f 7468  rm.divisible(oth
-00017b80: 6572 2c20 7269 6768 743d 7269 6768 7429  er, right=right)
-00017b90: 2066 6f72 2074 6572 6d20 696e 2073 656c   for term in sel
-00017ba0: 662e 7465 726d 7329 3a0a 2020 2020 2020  f.terms):.      
-00017bb0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00017bc0: 6572 6d73 203d 205b 0a20 2020 2020 2020  erms = [.       
-00017bd0: 2020 2020 2020 2020 2020 2020 205f 4f70               _Op
-00017be0: 4d75 6c74 5465 726d 2e66 726f 6d5f 6469  MultTerm.from_di
-00017bf0: 6d28 5f4f 704d 756c 7454 6572 6d2e 6e65  m(_OpMultTerm.ne
-00017c00: 775f 6469 765f 6469 6d28 7365 6c66 2e61  w_div_dim(self.a
-00017c10: 735f 6469 6d28 292c 206f 7468 6572 2c20  s_dim(), other, 
-00017c20: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00017c30: 3d72 6967 6874 2929 0a20 2020 2020 2020  =right)).       
-00017c40: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00017c50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00017c60: 6e0a 2020 2020 2020 2020 666f 7220 7465  n.        for te
-00017c70: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
-00017c80: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-00017c90: 726d 2e65 7874 656e 645f 6d75 6c5f 6469  rm.extend_mul_di
-00017ca0: 765f 286f 7468 6572 2c20 6b69 6e64 3d6b  v_(other, kind=k
+00010a40: 2020 2020 2020 2065 7869 7374 696e 675f         existing_
+00010a50: 7461 672e 756e 6465 6669 6e65 6420 616e  tag.undefined an
+00010a60: 6420 6e6f 7420 7461 672e 756e 6465 6669  d not tag.undefi
+00010a70: 6e65 6420 616e 6420 7461 672e 6469 6d65  ned and tag.dime
+00010a80: 6e73 696f 6e20 3d3d 2065 7869 7374 696e  nsion == existin
+00010a90: 675f 7461 672e 6469 6d65 6e73 696f 6e0a  g_tag.dimension.
+00010aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ab0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00010ac0: 2020 2020 2020 2020 2020 6966 2072 6570            if rep
+00010ad0: 6c61 6365 5f65 7869 7374 696e 673a 2020  lace_existing:  
+00010ae0: 2320 5265 706c 6163 6520 7468 6520 6578  # Replace the ex
+00010af0: 6973 7469 6e67 2062 7920 7468 6520 6e65  isting by the ne
+00010b00: 7720 7461 672e 0a20 2020 2020 2020 2020  w tag..         
+00010b10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00010b20: 6167 735b 7461 6773 2e69 6e64 6578 2865  ags[tags.index(e
+00010b30: 7869 7374 696e 675f 7461 6729 5d20 3d20  xisting_tag)] = 
+00010b40: 7461 670a 2020 2020 2020 2020 2020 2020  tag.            
+00010b50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00010b60: 5f2c 2064 696d 735f 2069 6e20 6461 7461  _, dims_ in data
+00010b70: 5f61 7865 735f 6469 6374 2e69 7465 6d73  _axes_dict.items
+00010b80: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ba0: 6469 6d73 5f5b 3a5d 203d 205b 7461 6720  dims_[:] = [tag 
+00010bb0: 6966 2064 203d 3d20 6578 6973 7469 6e67  if d == existing
+00010bc0: 5f74 6167 2065 6c73 6520 6420 666f 7220  _tag else d for 
+00010bd0: 6420 696e 2064 696d 735f 5d0a 2020 2020  d in dims_].    
+00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bf0: 2020 2020 6578 6973 7469 6e67 5f74 6167      existing_tag
+00010c00: 203d 2074 6167 0a20 2020 2020 2020 2020   = tag.         
+00010c10: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
+00010c20: 6e6f 2065 7869 7374 696e 6720 7461 670a  no existing tag.
+00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c40: 2020 2020 7461 6773 2e61 7070 656e 6428      tags.append(
+00010c50: 7461 6729 0a20 2020 2020 2020 2020 2020  tag).           
+00010c60: 2020 2020 2064 6174 615f 6178 6573 5f64       data_axes_d
+00010c70: 6963 745b 6461 7461 5d2e 6170 7065 6e64  ict[data].append
+00010c80: 2865 7869 7374 696e 675f 7461 6720 6f72  (existing_tag or
+00010c90: 2074 6167 290a 2020 2020 2020 2020 7265   tag).        re
+00010ca0: 7475 726e 2074 6167 732c 2064 6174 615f  turn tags, data_
+00010cb0: 6178 6573 5f64 6963 740a 0a20 2020 2040  axes_dict..    @
+00010cc0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+00010cd0: 6465 6620 6765 745f 756e 6971 5f63 6f6c  def get_uniq_col
+00010ce0: 6c65 6374 696f 6e28 636c 732c 2074 6167  lection(cls, tag
+00010cf0: 732c 2069 735f 6571 7561 6c5f 6f70 7473  s, is_equal_opts
+00010d00: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00010d10: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+00010d20: 616d 206c 6973 745b 4469 6d5d 7c74 7570  am list[Dim]|tup
+00010d30: 6c65 5b44 696d 5d7c 7365 745b 4469 6d5d  le[Dim]|set[Dim]
+00010d40: 2074 6167 733a 0a20 2020 2020 2020 203a   tags:.        :
+00010d50: 7061 7261 6d20 6469 6374 5b73 7472 5d7c  param dict[str]|
+00010d60: 4e6f 6e65 2069 735f 6571 7561 6c5f 6f70  None is_equal_op
+00010d70: 7473 3a20 7061 7373 6564 2074 6f20 4469  ts: passed to Di
+00010d80: 6d2e 6973 5f65 7175 616c 0a20 2020 2020  m.is_equal.     
+00010d90: 2020 203a 7274 7970 653a 206c 6973 745b     :rtype: list[
+00010da0: 4469 6d5d 0a20 2020 2020 2020 2022 2222  Dim].        """
+00010db0: 0a20 2020 2020 2020 2072 6573 203d 205b  .        res = [
+00010dc0: 5d0a 2020 2020 2020 2020 666f 7220 7461  ].        for ta
+00010dd0: 6720 696e 2074 6167 733a 0a20 2020 2020  g in tags:.     
+00010de0: 2020 2020 2020 2065 7820 3d20 636c 732e         ex = cls.
+00010df0: 6765 745f 6578 6973 7469 6e67 5f74 6167  get_existing_tag
+00010e00: 5f66 726f 6d5f 636f 6c6c 6563 7469 6f6e  _from_collection
+00010e10: 2874 6167 2c20 7265 732c 2069 735f 6571  (tag, res, is_eq
+00010e20: 7561 6c5f 6f70 7473 3d69 735f 6571 7561  ual_opts=is_equa
+00010e30: 6c5f 6f70 7473 290a 2020 2020 2020 2020  l_opts).        
+00010e40: 2020 2020 6966 206e 6f74 2065 783a 0a20      if not ex:. 
+00010e50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010e60: 6573 2e61 7070 656e 6428 7461 6729 0a20  es.append(tag). 
+00010e70: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00010e80: 730a 0a20 2020 2064 6566 2067 6574 5f73  s..    def get_s
+00010e90: 697a 655f 7465 6e73 6f72 2873 656c 6629  ize_tensor(self)
+00010ea0: 202d 3e20 5f74 2e54 656e 736f 723a 0a20   -> _t.Tensor:. 
+00010eb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010ec0: 2020 203a 7265 7475 726e 3a20 7369 7a65     :return: size
+00010ed0: 2074 656e 736f 722c 206f 7220 6479 6e5f   tensor, or dyn_
+00010ee0: 7369 7a65 5f65 7874 2069 6620 6465 6669  size_ext if defi
+00010ef0: 6e65 640a 2020 2020 2020 2020 3a72 7479  ned.        :rty
+00010f00: 7065 3a20 5f74 2e54 656e 736f 720a 2020  pe: _t.Tensor.  
+00010f10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010f20: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
+00010f30: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
+00010f40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00010f50: 6479 6e5f 7369 7a65 5f65 7874 0a0a 2020  dyn_size_ext..  
+00010f60: 2020 2020 2020 696d 706f 7274 2072 6574        import ret
+00010f70: 7572 6e6e 2e66 726f 6e74 656e 6420 6173  urnn.frontend as
+00010f80: 2072 660a 0a20 2020 2020 2020 2061 7373   rf..        ass
+00010f90: 6572 7420 7365 6c66 2e73 697a 6520 6973  ert self.size is
+00010fa0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+00010fb0: 2020 7265 7475 726e 2072 662e 636f 6e76    return rf.conv
+00010fc0: 6572 745f 746f 5f74 656e 736f 7228 7365  ert_to_tensor(se
+00010fd0: 6c66 2e73 697a 652c 206e 616d 653d 2225  lf.size, name="%
+00010fe0: 733a 7369 7a65 2220 2520 7365 6c66 2e64  s:size" % self.d
+00010ff0: 6573 6372 6970 7469 6f6e 290a 0a20 2020  escription)..   
+00011000: 2064 6566 2067 6574 5f64 696d 5f76 616c   def get_dim_val
+00011010: 7565 2873 656c 6629 202d 3e20 556e 696f  ue(self) -> Unio
+00011020: 6e5b 696e 742c 205f 742e 5261 7754 656e  n[int, _t.RawTen
+00011030: 736f 7254 7970 655d 3a0a 2020 2020 2020  sorType]:.      
+00011040: 2020 2222 220a 2020 2020 2020 2020 496e    """.        In
+00011050: 6665 7273 2074 6865 2064 696d 2074 6869  fers the dim thi
+00011060: 7320 6178 6973 2073 686f 756c 6420 6861  s axis should ha
+00011070: 7665 2069 6620 756e 6272 6f61 6463 6173  ve if unbroadcas
+00011080: 7465 642e 0a20 2020 2020 2020 2049 6620  ted..        If 
+00011090: 6073 656c 662e 7372 635f 6461 7461 6020  `self.src_data` 
+000110a0: 6861 7320 6120 706c 6163 6568 6f6c 6465  has a placeholde
+000110b0: 722c 2077 696c 6c20 7573 6520 7468 6520  r, will use the 
+000110c0: 7368 6170 6520 6672 6f6d 2074 6865 7265  shape from there
+000110d0: 2e0a 2020 2020 2020 2020 4f74 6865 7277  ..        Otherw
+000110e0: 6973 652c 2075 7365 7320 6073 656c 662e  ise, uses `self.
+000110f0: 6469 6d65 6e73 696f 6e60 2028 6966 2073  dimension` (if s
+00011100: 7461 7469 6329 206f 7220 6073 656c 662e  tatic) or `self.
+00011110: 6479 6e5f 7369 7a65 6020 2869 6620 6479  dyn_size` (if dy
+00011120: 6e61 6d69 6329 2e0a 0a20 2020 2020 2020  namic)...       
+00011130: 203a 7265 7475 726e 3a20 6d61 7828 7369   :return: max(si
+00011140: 7a65 206f 7220 6479 6e5f 7369 7a65 290a  ze or dyn_size).
+00011150: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011160: 2020 2020 7265 7320 3d20 7365 6c66 2e67      res = self.g
+00011170: 6574 5f64 696d 5f76 616c 7565 5f74 656e  et_dim_value_ten
+00011180: 736f 7228 290a 2020 2020 2020 2020 6966  sor().        if
+00011190: 2069 7369 6e73 7461 6e63 6528 7265 732c   isinstance(res,
+000111a0: 205f 742e 5465 6e73 6f72 293a 0a20 2020   _t.Tensor):.   
+000111b0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000111c0: 7265 732e 6469 6d73 203d 3d20 2829 0a20  res.dims == (). 
+000111d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000111e0: 6e20 7265 732e 7261 775f 7465 6e73 6f72  n res.raw_tensor
+000111f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00011200: 6973 696e 7374 616e 6365 2872 6573 2c20  isinstance(res, 
+00011210: 696e 7429 0a20 2020 2020 2020 2072 6574  int).        ret
+00011220: 7572 6e20 7265 730a 0a20 2020 2064 6566  urn res..    def
+00011230: 2067 6574 5f64 696d 5f76 616c 7565 5f74   get_dim_value_t
+00011240: 656e 736f 7228 7365 6c66 2920 2d3e 2055  ensor(self) -> U
+00011250: 6e69 6f6e 5b69 6e74 2c20 5f74 2e54 656e  nion[int, _t.Ten
+00011260: 736f 725d 3a0a 2020 2020 2020 2020 2222  sor]:.        ""
+00011270: 220a 2020 2020 2020 2020 496e 6665 7273  ".        Infers
+00011280: 2074 6865 2064 696d 2074 6869 7320 6178   the dim this ax
+00011290: 6973 2073 686f 756c 6420 6861 7665 2069  is should have i
+000112a0: 6620 756e 6272 6f61 6463 6173 7465 642e  f unbroadcasted.
+000112b0: 0a20 2020 2020 2020 2049 6620 6073 656c  .        If `sel
+000112c0: 662e 7372 635f 6461 7461 6020 6861 7320  f.src_data` has 
+000112d0: 6120 706c 6163 6568 6f6c 6465 722c 2077  a placeholder, w
+000112e0: 696c 6c20 7573 6520 7468 6520 7368 6170  ill use the shap
+000112f0: 6520 6672 6f6d 2074 6865 7265 2e0a 2020  e from there..  
+00011300: 2020 2020 2020 4f74 6865 7277 6973 652c        Otherwise,
+00011310: 2075 7365 7320 6073 656c 662e 6469 6d65   uses `self.dime
+00011320: 6e73 696f 6e60 2028 6966 2073 7461 7469  nsion` (if stati
+00011330: 6329 206f 7220 6073 656c 662e 6479 6e5f  c) or `self.dyn_
+00011340: 7369 7a65 6020 2869 6620 6479 6e61 6d69  size` (if dynami
+00011350: 6329 2e0a 0a20 2020 2020 2020 203a 7265  c)...        :re
+00011360: 7475 726e 3a20 6d61 7828 7369 7a65 206f  turn: max(size o
+00011370: 7220 6479 6e5f 7369 7a65 290a 2020 2020  r dyn_size).    
+00011380: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00011390: 696d 706f 7274 2072 6574 7572 6e6e 2e66  import returnn.f
+000113a0: 726f 6e74 656e 6420 6173 2072 660a 0a20  rontend as rf.. 
+000113b0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+000113c0: 696d 656e 7369 6f6e 2069 7320 6e6f 7420  imension is not 
+000113d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000113e0: 2020 7265 7475 726e 2073 656c 662e 6469    return self.di
+000113f0: 6d65 6e73 696f 6e0a 2020 2020 2020 2020  mension.        
+00011400: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
+00011410: 5f65 7874 2061 6e64 2073 656c 662e 6479  _ext and self.dy
+00011420: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
+00011430: 686f 6c64 6572 2069 7320 6e6f 7420 4e6f  holder is not No
+00011440: 6e65 3a20 2023 2066 6173 7420 7061 7468  ne:  # fast path
+00011450: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011460: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00011470: 742e 6261 7463 685f 6e64 696d 203e 2030  t.batch_ndim > 0
+00011480: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011490: 2020 7265 7475 726e 2072 662e 7265 6475    return rf.redu
+000114a0: 6365 5f6d 6178 280a 2020 2020 2020 2020  ce_max(.        
+000114b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000114c0: 2e64 796e 5f73 697a 655f 6578 742c 0a20  .dyn_size_ext,. 
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114e0: 2020 2061 7869 733d 7365 6c66 2e64 796e     axis=self.dyn
+000114f0: 5f73 697a 655f 6578 742e 6469 6d5f 7461  _size_ext.dim_ta
+00011500: 6773 2c0a 2020 2020 2020 2020 2020 2020  gs,.            
+00011510: 2020 2020 2020 2020 2320 4d61 736b 696e          # Maskin
+00011520: 6720 6973 206e 6f74 2061 6c77 6179 7320  g is not always 
+00011530: 706f 7373 6962 6c65 2068 6572 652c 2065  possible here, e
+00011540: 2e67 2e0a 2020 2020 2020 2020 2020 2020  .g..            
+00011550: 2020 2020 2020 2020 2320 7365 6c66 203d          # self =
+00011560: 2044 696d 7b27 7365 6c66 2d61 7474 2d6b   Dim{'self-att-k
+00011570: 6579 7327 5b27 7469 6d65 3a76 6172 3a65  eys'['time:var:e
+00011580: 7874 6572 6e5f 6461 7461 3a63 6c61 7373  xtern_data:class
+00011590: 6573 275b 425d 5d7d 2e0a 2020 2020 2020  es'[B]]}..      
+000115a0: 2020 2020 2020 2020 2020 2020 2020 7573                us
+000115b0: 655f 6d61 736b 3d46 616c 7365 2c0a 2020  e_mask=False,.  
+000115c0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000115d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000115e0: 726e 2073 656c 662e 6479 6e5f 7369 7a65  rn self.dyn_size
+000115f0: 5f65 7874 0a20 2020 2020 2020 2069 6620  _ext.        if 
+00011600: 7365 6c66 2e69 735f 6261 7463 685f 6469  self.is_batch_di
+00011610: 6d28 293a 0a20 2020 2020 2020 2020 2020  m():.           
+00011620: 2072 6573 203d 204e 6f6e 650a 2020 2020   res = None.    
+00011630: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011640: 5f65 7874 7261 2061 6e64 2073 656c 662e  _extra and self.
+00011650: 5f65 7874 7261 2e73 7263 5f64 6174 613a  _extra.src_data:
+00011660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011670: 2072 6573 203d 2073 656c 662e 5f65 7874   res = self._ext
+00011680: 7261 2e73 7263 5f64 6174 612e 6765 745f  ra.src_data.get_
+00011690: 6261 7463 685f 6469 6d28 290a 2020 2020  batch_dim().    
+000116a0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+000116b0: 662e 6261 7463 683a 0a20 2020 2020 2020  f.batch:.       
+000116c0: 2020 2020 2020 2020 2072 6573 203d 2073           res = s
+000116d0: 656c 662e 6261 7463 682e 6469 6d0a 2020  elf.batch.dim.  
+000116e0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+000116f0: 6e73 7461 6e63 6528 7265 732c 2069 6e74  nstance(res, int
+00011700: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011710: 2020 2072 6574 7572 6e20 7265 730a 2020     return res.  
+00011720: 2020 2020 2020 2020 2020 6966 2072 6573            if res
+00011730: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00011740: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00011750: 7475 726e 205f 742e 5465 6e73 6f72 2822  turn _t.Tensor("
+00011760: 6261 7463 6822 2c20 6469 6d73 3d28 292c  batch", dims=(),
+00011770: 2064 7479 7065 3d72 662e 6765 745f 6465   dtype=rf.get_de
+00011780: 6661 756c 745f 6172 7261 795f 696e 6465  fault_array_inde
+00011790: 785f 6474 7970 6528 292c 2072 6177 5f74  x_dtype(), raw_t
+000117a0: 656e 736f 723d 7265 7329 0a20 2020 2020  ensor=res).     
+000117b0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+000117c0: 2020 2020 7365 6c66 2e5f 6578 7472 610a      self._extra.
+000117d0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+000117e0: 7365 6c66 2e5f 6578 7472 612e 7372 635f  self._extra.src_
+000117f0: 6461 7461 2069 7320 6e6f 7420 4e6f 6e65  data is not None
+00011800: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+00011810: 2073 656c 662e 5f65 7874 7261 2e73 7263   self._extra.src
+00011820: 5f61 7869 7320 6973 206e 6f74 204e 6f6e  _axis is not Non
+00011830: 650a 2020 2020 2020 2020 2020 2020 616e  e.            an
+00011840: 6420 7365 6c66 2e5f 6578 7472 612e 7372  d self._extra.sr
+00011850: 635f 6461 7461 2e70 6c61 6365 686f 6c64  c_data.placehold
+00011860: 6572 2069 7320 6e6f 7420 4e6f 6e65 0a20  er is not None. 
+00011870: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00011880: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
+00011890: 2e5f 6578 7472 612e 7372 635f 6461 7461  ._extra.src_data
+000118a0: 2e67 6574 5f64 696d 2873 656c 662e 5f65  .get_dim(self._e
+000118b0: 7874 7261 2e73 7263 5f61 7869 7329 0a20  xtra.src_axis). 
+000118c0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+000118d0: 696e 7374 616e 6365 2872 6573 2c20 696e  instance(res, in
+000118e0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000118f0: 2020 2020 7265 7475 726e 2072 6573 0a20      return res. 
+00011900: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00011910: 6e20 5f74 2e54 656e 736f 7228 2262 6174  n _t.Tensor("bat
+00011920: 6368 222c 2064 696d 733d 2829 2c20 6474  ch", dims=(), dt
+00011930: 7970 653d 7266 2e67 6574 5f64 6566 6175  ype=rf.get_defau
+00011940: 6c74 5f61 7272 6179 5f69 6e64 6578 5f64  lt_array_index_d
+00011950: 7479 7065 2829 2c20 7261 775f 7465 6e73  type(), raw_tens
+00011960: 6f72 3d72 6573 290a 2020 2020 2020 2020  or=res).        
+00011970: 7365 6c66 2e63 6f6d 706c 6574 655f 6479  self.complete_dy
+00011980: 6e5f 7369 7a65 2829 0a20 2020 2020 2020  n_size().       
+00011990: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
+000119a0: 655f 6578 7420 616e 6420 7365 6c66 2e64  e_ext and self.d
+000119b0: 796e 5f73 697a 655f 6578 742e 706c 6163  yn_size_ext.plac
+000119c0: 6568 6f6c 6465 7220 6973 206e 6f74 204e  eholder is not N
+000119d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000119e0: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
+000119f0: 655f 6578 742e 6261 7463 685f 6e64 696d  e_ext.batch_ndim
+00011a00: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00011a10: 2020 2020 2020 7265 7475 726e 2072 662e        return rf.
+00011a20: 7265 6475 6365 5f6d 6178 2873 656c 662e  reduce_max(self.
+00011a30: 6479 6e5f 7369 7a65 5f65 7874 2c20 6178  dyn_size_ext, ax
+00011a40: 6973 3d73 656c 662e 6479 6e5f 7369 7a65  is=self.dyn_size
+00011a50: 5f65 7874 2e64 696d 5f74 6167 7329 0a20  _ext.dim_tags). 
+00011a60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00011a70: 6e20 7365 6c66 2e64 796e 5f73 697a 655f  n self.dyn_size_
+00011a80: 6578 740a 2020 2020 2020 2020 7261 6973  ext.        rais
+00011a90: 6520 4578 6365 7074 696f 6e28 2225 733a  e Exception("%s:
+00011aa0: 206e 6565 6420 706c 6163 6568 6f6c 6465   need placeholde
+00011ab0: 722c 2073 656c 662e 6469 6d65 6e73 696f  r, self.dimensio
+00011ac0: 6e20 6f72 2073 656c 662e 6479 6e5f 7369  n or self.dyn_si
+00011ad0: 7a65 2066 6f72 2064 696d 2076 616c 7565  ze for dim value
+00011ae0: 2220 2520 7365 6c66 290a 0a20 2020 2064  " % self)..    d
+00011af0: 6566 2061 7869 735f 7370 6c69 745f 696e  ef axis_split_in
+00011b00: 666f 2873 656c 6629 3a0a 2020 2020 2020  fo(self):.      
+00011b10: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00011b20: 6574 7572 6e3a 2061 7869 7320 7370 6c69  eturn: axis spli
+00011b30: 7420 696e 666f 2e20 7365 6520 3a66 756e  t info. see :fun
+00011b40: 633a 6067 6574 5f70 6172 616d 5f61 7865  c:`get_param_axe
+00011b50: 735f 7370 6c69 745f 696e 666f 6020 616e  s_split_info` an
+00011b60: 6420 7573 6167 6520 2865 2e67 2e20 7072  d usage (e.g. pr
+00011b70: 6574 7261 696e 696e 6729 0a20 2020 2020  etraining).     
+00011b80: 2020 203a 7274 7970 653a 206c 6973 745b     :rtype: list[
+00011b90: 696e 747c 4e6f 6e65 5d0a 2020 2020 2020  int|None].      
+00011ba0: 2020 2222 220a 2020 2020 2020 2020 7361    """.        sa
+00011bb0: 6d65 5f62 6173 6520 3d20 7365 6c66 2e67  me_base = self.g
+00011bc0: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
+00011bd0: 2020 2020 2020 206f 7020 3d20 7365 6c66         op = self
+00011be0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00011bf0: 206f 7220 7361 6d65 5f62 6173 652e 6465   or same_base.de
+00011c00: 7269 7665 645f 6672 6f6d 5f6f 700a 2020  rived_from_op.  
+00011c10: 2020 2020 2020 6966 206e 6f74 206f 703a        if not op:
+00011c20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011c30: 7572 6e20 5b73 656c 662e 6469 6d65 6e73  urn [self.dimens
+00011c40: 696f 6e5d 0a20 2020 2020 2020 2069 6620  ion].        if 
+00011c50: 6f70 2e6b 696e 6420 3d3d 2022 6164 6422  op.kind == "add"
+00011c60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00011c70: 7475 726e 2073 756d 285b 782e 6178 6973  turn sum([x.axis
+00011c80: 5f73 706c 6974 5f69 6e66 6f28 2920 666f  _split_info() fo
+00011c90: 7220 7820 696e 206f 702e 696e 7075 7473  r x in op.inputs
+00011ca0: 5d2c 205b 5d29 2020 2320 666c 6174 7465  ], [])  # flatte
+00011cb0: 6e0a 2020 2020 2020 2020 6966 206f 702e  n.        if op.
+00011cc0: 6b69 6e64 203d 3d20 226d 756c 223a 0a20  kind == "mul":. 
+00011cd0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
+00011ce0: 205b 315d 0a20 2020 2020 2020 2020 2020   [1].           
+00011cf0: 2066 6f72 2078 2069 6e20 6f70 2e69 6e70   for x in op.inp
+00011d00: 7574 733a 0a20 2020 2020 2020 2020 2020  uts:.           
+00011d10: 2020 2020 2072 6573 203d 2073 756d 285b       res = sum([
+00011d20: 6e20 2a20 782e 6178 6973 5f73 706c 6974  n * x.axis_split
+00011d30: 5f69 6e66 6f28 2920 6966 206e 2069 7320  _info() if n is 
+00011d40: 6e6f 7420 4e6f 6e65 2065 6c73 6520 4e6f  not None else No
+00011d50: 6e65 2066 6f72 206e 2069 6e20 7265 735d  ne for n in res]
+00011d60: 2c20 5b5d 2920 2023 2066 6c61 7474 656e  , [])  # flatten
+00011d70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011d80: 7572 6e20 7265 730a 2020 2020 2020 2020  urn res.        
+00011d90: 7265 7475 726e 205b 7365 6c66 2e64 696d  return [self.dim
+00011da0: 656e 7369 6f6e 5d0a 0a20 2020 2064 6566  ension]..    def
+00011db0: 205f 6765 745f 7361 6d65 5f62 6173 655f   _get_same_base_
+00011dc0: 6578 7472 6128 7365 6c66 2920 2d3e 204f  extra(self) -> O
+00011dd0: 7074 696f 6e61 6c5b 5f44 696d 4578 7472  ptional[_DimExtr
+00011de0: 615d 3a0a 2020 2020 2020 2020 6966 206e  a]:.        if n
+00011df0: 6f74 2073 656c 662e 5f65 7874 7261 3a0a  ot self._extra:.
+00011e00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00011e10: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
+00011e20: 6261 7365 203d 2073 656c 662e 6765 745f  base = self.get_
+00011e30: 7361 6d65 5f62 6173 6528 290a 2020 2020  same_base().    
+00011e40: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+00011e50: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+00011e60: 6d62 6572 0a20 2020 2020 2020 2072 6574  mber.        ret
+00011e70: 7572 6e20 6261 7365 2e5f 6578 7472 610a  urn base._extra.
+00011e80: 0a20 2020 2064 6566 205f 6d61 6b65 5f65  .    def _make_e
+00011e90: 7874 7261 2873 656c 663a 205f 642e 4469  xtra(self: _d.Di
+00011ea0: 6d29 202d 3e20 5f44 696d 4578 7472 613a  m) -> _DimExtra:
+00011eb0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00011ec0: 7365 6c66 2e5f 6578 7472 613a 0a20 2020  self._extra:.   
+00011ed0: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
+00011ee0: 7874 7261 203d 205f 4469 6d45 7874 7261  xtra = _DimExtra
+00011ef0: 2864 696d 3d73 656c 6629 0a20 2020 2020  (dim=self).     
+00011f00: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00011f10: 6578 7472 610a 0a20 2020 2040 7072 6f70  extra..    @prop
+00011f20: 6572 7479 0a20 2020 2064 6566 2076 6f63  erty.    def voc
+00011f30: 6162 2873 656c 6629 3a0a 2020 2020 2020  ab(self):.      
+00011f40: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00011f50: 7479 7065 3a20 7265 7475 726e 6e2e 6461  type: returnn.da
+00011f60: 7461 7365 7473 2e75 7469 6c2e 766f 6361  tasets.util.voca
+00011f70: 6275 6c61 7279 2e56 6f63 6162 756c 6172  bulary.Vocabular
+00011f80: 797c 4e6f 6e65 0a20 2020 2020 2020 2022  y|None.        "
+00011f90: 2222 0a20 2020 2020 2020 2065 7874 7261  "".        extra
+00011fa0: 203d 2073 656c 662e 5f67 6574 5f73 616d   = self._get_sam
+00011fb0: 655f 6261 7365 5f65 7874 7261 2829 0a20  e_base_extra(). 
+00011fc0: 2020 2020 2020 2069 6620 6578 7472 613a         if extra:
+00011fd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011fe0: 7572 6e20 6578 7472 612e 766f 6361 620a  urn extra.vocab.
+00011ff0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00012000: 6f6e 650a 0a20 2020 2040 766f 6361 622e  one..    @vocab.
+00012010: 7365 7474 6572 0a20 2020 2064 6566 2076  setter.    def v
+00012020: 6f63 6162 2873 656c 662c 2076 6f63 6162  ocab(self, vocab
+00012030: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012040: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
+00012050: 7475 726e 6e2e 6461 7461 7365 7473 2e75  turnn.datasets.u
+00012060: 7469 6c2e 766f 6361 6275 6c61 7279 2e56  til.vocabulary.V
+00012070: 6f63 6162 756c 6172 797c 4e6f 6e65 2076  ocabulary|None v
+00012080: 6f63 6162 3a0a 2020 2020 2020 2020 2222  ocab:.        ""
+00012090: 220a 2020 2020 2020 2020 6966 2076 6f63  ".        if voc
+000120a0: 6162 2069 7320 7365 6c66 2e76 6f63 6162  ab is self.vocab
+000120b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000120c0: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+000120d0: 7365 6c66 2e73 616d 655f 6173 3a0a 2020  self.same_as:.  
+000120e0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+000120f0: 6574 5f73 616d 655f 6261 7365 2829 2e76  et_same_base().v
+00012100: 6f63 6162 203d 2076 6f63 6162 0a20 2020  ocab = vocab.   
+00012110: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00012120: 2020 2020 2020 2020 6578 7472 6120 3d20          extra = 
+00012130: 7365 6c66 2e5f 6765 745f 7361 6d65 5f62  self._get_same_b
+00012140: 6173 655f 6578 7472 6128 290a 2020 2020  ase_extra().    
+00012150: 2020 2020 6966 2065 7874 7261 3a0a 2020      if extra:.  
+00012160: 2020 2020 2020 2020 2020 6578 7472 612e            extra.
+00012170: 766f 6361 6220 3d20 766f 6361 620a 0a20  vocab = vocab.. 
+00012180: 2020 2023 2054 6865 206b 696e 6420 6f66     # The kind of
+00012190: 206f 7065 7261 7469 6f6e 7320 7765 2068   operations we h
+000121a0: 6176 653a 0a20 2020 2023 2061 202b 2062  ave:.    # a + b
+000121b0: 3a20 7061 6464 696e 672c 2063 6f6e 6361  : padding, conca
+000121c0: 740a 2020 2020 2320 6120 2d20 623a 2077  t.    # a - b: w
+000121d0: 696e 646f 7720 7769 7468 2076 616c 6964  indow with valid
+000121e0: 2066 7261 6d65 7320 6f6e 6c79 0a20 2020   frames only.   
+000121f0: 2023 2061 202a 2062 3a20 6d65 7267 6520   # a * b: merge 
+00012200: 6469 6d73 2c20 7570 7361 6d70 6c65 2c20  dims, upsample, 
+00012210: 7472 616e 7370 6f73 6564 2063 6f6e 7620  transposed conv 
+00012220: 7769 7468 2073 7472 6964 696e 670a 2020  with striding.  
+00012230: 2020 2320 6120 2f20 6220 2877 6865 6e20    # a / b (when 
+00012240: 6120 2520 6220 3d3d 2030 293a 2073 706c  a % b == 0): spl
+00012250: 6974 2064 696d 732c 2064 6f77 6e73 616d  it dims, downsam
+00012260: 706c 652c 2063 6f6e 7620 7769 7468 2073  ple, conv with s
+00012270: 7472 6964 696e 670a 2020 2020 2320 6365  triding.    # ce
+00012280: 696c 6469 7628 612c 2062 293a 2063 6f6e  ildiv(a, b): con
+00012290: 7620 7769 7468 2073 7472 6964 696e 670a  v with striding.
+000122a0: 2020 2020 2320 6375 7374 6f6d 3a20 7265      # custom: re
+000122b0: 7065 6174 2c20 7265 6d6f 7665 2c20 6d61  peat, remove, ma
+000122c0: 736b 2c20 6c6f 6f70 2077 6974 6820 6479  sk, loop with dy
+000122d0: 6e20 656e 640a 2020 2020 2320 4e6f 7465  n end.    # Note
+000122e0: 2074 6861 7420 7765 2064 6966 6665 7265   that we differe
+000122f0: 6e74 6961 7465 2062 6574 7765 656e 2074  ntiate between t
+00012300: 6865 206f 7264 6572 2c20 692e 652e 2061  he order, i.e. a
+00012310: 202b 2062 2021 3d20 6220 2b20 612e 0a20   + b != b + a.. 
+00012320: 2020 2023 204e 6f74 6520 7468 6174 2077     # Note that w
+00012330: 6520 616c 7761 7973 2068 6176 6520 7468  e always have th
+00012340: 6520 6173 7375 6d70 7469 6f6e 2074 6861  e assumption tha
+00012350: 7420 6120 6469 6d65 6e73 696f 6e20 6973  t a dimension is
+00012360: 206e 6f6e 2d6e 6567 6174 6976 652e 0a20   non-negative.. 
+00012370: 2020 2023 2054 6869 7320 6173 7375 6d70     # This assump
+00012380: 7469 6f6e 2069 7320 6e65 6365 7373 6172  tion is necessar
+00012390: 7920 666f 7220 736f 6d65 2073 696d 706c  y for some simpl
+000123a0: 6966 6963 6174 696f 6e73 2e0a 2020 2020  ifications..    
+000123b0: 2320 6874 7470 733a 2f2f 6769 7468 7562  # https://github
+000123c0: 2e63 6f6d 2f72 7774 682d 6936 2f72 6574  .com/rwth-i6/ret
+000123d0: 7572 6e6e 2f70 756c 6c2f 3835 330a 0a20  urnn/pull/853.. 
+000123e0: 2020 2064 6566 205f 5f61 6464 5f5f 2873     def __add__(s
+000123f0: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
+00012400: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012410: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+00012420: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
+00012430: 2020 2020 3a72 6574 7572 6e3a 2073 656c      :return: sel
+00012440: 6620 2b20 6f74 6865 722e 206e 6f74 6520  f + other. note 
+00012450: 7468 6174 2074 6869 7320 6973 206e 6f74  that this is not
+00012460: 2063 6f6d 6d75 7461 7469 7665 2c20 692e   commutative, i.
+00012470: 652e 2064 6966 6665 7265 6e74 2066 726f  e. different fro
+00012480: 6d20 6f74 6865 7220 2b20 7365 6c66 2e0a  m other + self..
+00012490: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000124a0: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
+000124b0: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
+000124c0: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
+000124d0: 6d5f 6469 6d28 7365 6c66 290a 2020 2020  m_dim(self).    
+000124e0: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
+000124f0: 6164 645f 7375 625f 286f 7468 6572 2c20  add_sub_(other, 
+00012500: 6b69 6e64 3d22 6164 6422 2c20 7269 6768  kind="add", righ
+00012510: 743d 5472 7565 290a 2020 2020 2020 2020  t=True).        
+00012520: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
+00012530: 696d 2829 0a0a 2020 2020 6465 6620 5f5f  im()..    def __
+00012540: 7261 6464 5f5f 2873 656c 663a 2044 696d  radd__(self: Dim
+00012550: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+00012560: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00012570: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
+00012580: 6572 3a0a 2020 2020 2020 2020 3a72 6574  er:.        :ret
+00012590: 7572 6e3a 206f 7468 6572 202b 2073 656c  urn: other + sel
+000125a0: 660a 2020 2020 2020 2020 3a72 7479 7065  f.        :rtype
+000125b0: 3a20 4469 6d0a 2020 2020 2020 2020 2222  : Dim.        ""
+000125c0: 220a 2020 2020 2020 2020 7465 726d 203d  ".        term =
+000125d0: 205f 4f70 4c69 6e65 6172 5465 726d 2e66   _OpLinearTerm.f
+000125e0: 726f 6d5f 6469 6d28 7365 6c66 290a 2020  rom_dim(self).  
+000125f0: 2020 2020 2020 7465 726d 2e65 7874 656e        term.exten
+00012600: 645f 6164 645f 7375 625f 286f 7468 6572  d_add_sub_(other
+00012610: 2c20 6b69 6e64 3d22 6164 6422 2c20 7269  , kind="add", ri
+00012620: 6768 743d 4661 6c73 6529 0a20 2020 2020  ght=False).     
+00012630: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
+00012640: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
+00012650: 205f 5f73 7562 5f5f 2873 656c 662c 206f   __sub__(self, o
+00012660: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00012670: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00012680: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+00012690: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000126a0: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+000126b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000126c0: 7365 6c66 2e73 7562 5f72 6967 6874 286f  self.sub_right(o
+000126d0: 7468 6572 290a 0a20 2020 2064 6566 2073  ther)..    def s
+000126e0: 7562 5f72 6967 6874 2873 656c 663a 2044  ub_right(self: D
+000126f0: 696d 2c20 6f74 6865 7229 3a0a 2020 2020  im, other):.    
+00012700: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012710: 3a70 6172 616d 2044 696d 7c69 6e74 206f  :param Dim|int o
+00012720: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
+00012730: 6574 7572 6e3a 2073 656c 6620 2d20 6f74  eturn: self - ot
+00012740: 6865 720a 2020 2020 2020 2020 3a72 7479  her.        :rty
+00012750: 7065 3a20 4469 6d0a 2020 2020 2020 2020  pe: Dim.        
+00012760: 2222 220a 2020 2020 2020 2020 7465 726d  """.        term
+00012770: 203d 205f 4f70 4c69 6e65 6172 5465 726d   = _OpLinearTerm
+00012780: 2e66 726f 6d5f 6469 6d28 7365 6c66 290a  .from_dim(self).
+00012790: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
+000127a0: 656e 645f 6164 645f 7375 625f 286f 7468  end_add_sub_(oth
+000127b0: 6572 2c20 6b69 6e64 3d22 7375 6222 2c20  er, kind="sub", 
+000127c0: 7269 6768 743d 5472 7565 290a 2020 2020  right=True).    
+000127d0: 2020 2020 7265 7475 726e 2074 6572 6d2e      return term.
+000127e0: 6173 5f64 696d 2829 0a0a 2020 2020 6465  as_dim()..    de
+000127f0: 6620 7375 625f 6c65 6674 2873 656c 663a  f sub_left(self:
+00012800: 2044 696d 2c20 6f74 6865 7229 3a0a 2020   Dim, other):.  
+00012810: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012820: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
+00012830: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+00012840: 3a72 6574 7572 6e3a 2028 2d6f 7468 6572  :return: (-other
+00012850: 2920 2b20 7365 6c66 0a20 2020 2020 2020  ) + self.       
+00012860: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
+00012870: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012880: 2074 6572 6d20 3d20 5f4f 704c 696e 6561   term = _OpLinea
+00012890: 7254 6572 6d2e 6672 6f6d 5f64 696d 2873  rTerm.from_dim(s
+000128a0: 656c 6629 0a20 2020 2020 2020 2074 6572  elf).        ter
+000128b0: 6d2e 6578 7465 6e64 5f61 6464 5f73 7562  m.extend_add_sub
+000128c0: 5f28 6f74 6865 722c 206b 696e 643d 2273  _(other, kind="s
+000128d0: 7562 222c 2072 6967 6874 3d46 616c 7365  ub", right=False
+000128e0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000128f0: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
+00012900: 2020 2020 6465 6620 5f5f 6d75 6c5f 5f28      def __mul__(
+00012910: 7365 6c66 3a20 4469 6d2c 206f 7468 6572  self: Dim, other
+00012920: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012930: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+00012940: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
+00012950: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00012960: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012970: 2020 2020 2074 6572 6d20 3d20 5f4f 704c       term = _OpL
+00012980: 696e 6561 7254 6572 6d2e 6672 6f6d 5f64  inearTerm.from_d
+00012990: 696d 2873 656c 6629 0a20 2020 2020 2020  im(self).       
+000129a0: 2074 6572 6d2e 6578 7465 6e64 5f6d 756c   term.extend_mul
+000129b0: 5f64 6976 5f28 6f74 6865 722c 206b 696e  _div_(other, kin
+000129c0: 643d 226d 756c 222c 2072 6967 6874 3d54  d="mul", right=T
+000129d0: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
+000129e0: 7572 6e20 7465 726d 2e61 735f 6469 6d28  urn term.as_dim(
+000129f0: 290a 0a20 2020 2064 6566 205f 5f72 6d75  )..    def __rmu
+00012a00: 6c5f 5f28 7365 6c66 3a20 4469 6d2c 206f  l__(self: Dim, o
+00012a10: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00012a20: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00012a30: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+00012a40: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00012a50: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00012a60: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
+00012a70: 5f4f 704c 696e 6561 7254 6572 6d2e 6672  _OpLinearTerm.fr
+00012a80: 6f6d 5f64 696d 2873 656c 6629 0a20 2020  om_dim(self).   
+00012a90: 2020 2020 2074 6572 6d2e 6578 7465 6e64       term.extend
+00012aa0: 5f6d 756c 5f64 6976 5f28 6f74 6865 722c  _mul_div_(other,
+00012ab0: 206b 696e 643d 226d 756c 222c 2072 6967   kind="mul", rig
+00012ac0: 6874 3d46 616c 7365 290a 2020 2020 2020  ht=False).      
+00012ad0: 2020 7265 7475 726e 2074 6572 6d2e 6173    return term.as
+00012ae0: 5f64 696d 2829 0a0a 2020 2020 6465 6620  _dim()..    def 
+00012af0: 5f5f 666c 6f6f 7264 6976 5f5f 2873 656c  __floordiv__(sel
+00012b00: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
+00012b10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012b20: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
+00012b30: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
+00012b40: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
+00012b50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012b60: 2020 7465 726d 203d 205f 4f70 4c69 6e65    term = _OpLine
+00012b70: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
+00012b80: 7365 6c66 290a 2020 2020 2020 2020 7465  self).        te
+00012b90: 726d 2e65 7874 656e 645f 6d75 6c5f 6469  rm.extend_mul_di
+00012ba0: 765f 286f 7468 6572 2c20 6b69 6e64 3d22  v_(other, kind="
+00012bb0: 666c 6f6f 7264 6976 222c 2072 6967 6874  floordiv", right
+00012bc0: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
+00012bd0: 6574 7572 6e20 7465 726d 2e61 735f 6469  eturn term.as_di
+00012be0: 6d28 290a 0a20 2020 2064 6566 205f 5f74  m()..    def __t
+00012bf0: 7275 6564 6976 5f5f 2873 656c 662c 206f  ruediv__(self, o
+00012c00: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00012c10: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00012c20: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+00012c30: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00012c40: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00012c50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012c60: 7365 6c66 2e64 6976 5f72 6967 6874 286f  self.div_right(o
+00012c70: 7468 6572 290a 0a20 2020 2064 6566 2064  ther)..    def d
+00012c80: 6976 5f6c 6566 7428 7365 6c66 3a20 4469  iv_left(self: Di
+00012c90: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
+00012ca0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00012cb0: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
+00012cc0: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
+00012cd0: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+00012ce0: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
+00012cf0: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
+00012d00: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
+00012d10: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
+00012d20: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
+00012d30: 6865 722c 206b 696e 643d 2274 7275 6564  her, kind="trued
+00012d40: 6976 222c 2072 6967 6874 3d46 616c 7365  iv", right=False
+00012d50: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00012d60: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
+00012d70: 2020 2020 6465 6620 6469 765f 7269 6768      def div_righ
+00012d80: 7428 7365 6c66 3a20 4469 6d2c 206f 7468  t(self: Dim, oth
+00012d90: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
+00012da0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00012db0: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
+00012dc0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+00012dd0: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
+00012de0: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
+00012df0: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
+00012e00: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
+00012e10: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
+00012e20: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
+00012e30: 696e 643d 2274 7275 6564 6976 222c 2072  ind="truediv", r
+00012e40: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
+00012e50: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
+00012e60: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
+00012e70: 2063 6569 6c64 6976 5f6c 6566 7428 7365   ceildiv_left(se
+00012e80: 6c66 3a20 4469 6d2c 206f 7468 6572 293a  lf: Dim, other):
+00012e90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012ea0: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
+00012eb0: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
+00012ec0: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
+00012ed0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012ee0: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
+00012ef0: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
+00012f00: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
+00012f10: 6572 6d2e 6578 7465 6e64 5f6d 756c 5f64  erm.extend_mul_d
+00012f20: 6976 5f28 6f74 6865 722c 206b 696e 643d  iv_(other, kind=
+00012f30: 2263 6569 6c64 6976 222c 2072 6967 6874  "ceildiv", right
+00012f40: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00012f50: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
+00012f60: 696d 2829 0a0a 2020 2020 6465 6620 6365  im()..    def ce
+00012f70: 696c 6469 765f 7269 6768 7428 7365 6c66  ildiv_right(self
+00012f80: 3a20 4469 6d2c 206f 7468 6572 293a 0a20  : Dim, other):. 
+00012f90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012fa0: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
+00012fb0: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
+00012fc0: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
+00012fd0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012fe0: 2074 6572 6d20 3d20 5f4f 704c 696e 6561   term = _OpLinea
+00012ff0: 7254 6572 6d2e 6672 6f6d 5f64 696d 2873  rTerm.from_dim(s
+00013000: 656c 6629 0a20 2020 2020 2020 2074 6572  elf).        ter
+00013010: 6d2e 6578 7465 6e64 5f6d 756c 5f64 6976  m.extend_mul_div
+00013020: 5f28 6f74 6865 722c 206b 696e 643d 2263  _(other, kind="c
+00013030: 6569 6c64 6976 222c 2072 6967 6874 3d54  eildiv", right=T
+00013040: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
+00013050: 7572 6e20 7465 726d 2e61 735f 6469 6d28  urn term.as_dim(
+00013060: 290a 0a20 2020 2064 6566 205f 5f6e 6567  )..    def __neg
+00013070: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00013080: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00013090: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
+000130a0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+000130b0: 7475 726e 202d 3120 2a20 7365 6c66 0a0a  turn -1 * self..
+000130c0: 2020 2020 6465 6620 6973 5f63 6f6e 7374      def is_const
+000130d0: 616e 745f 7374 6174 6963 5f64 696d 2873  ant_static_dim(s
+000130e0: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
+000130f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013100: 2020 3a72 6574 7572 6e3a 2064 6572 6976    :return: deriv
+00013110: 6564 206f 7020 6f66 2074 7970 6520 636f  ed op of type co
+00013120: 6e73 7461 6e74 0a20 2020 2020 2020 2022  nstant.        "
+00013130: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00013140: 6e20 7365 6c66 2e64 6572 6976 6564 5f66  n self.derived_f
+00013150: 726f 6d5f 6f70 2061 6e64 2073 656c 662e  rom_op and self.
+00013160: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00013170: 6b69 6e64 203d 3d20 2263 6f6e 7374 616e  kind == "constan
+00013180: 7422 0a0a 0a64 6566 205f 6d61 6b65 5f63  t"...def _make_c
+00013190: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+000131a0: 696d 2876 616c 7565 2c20 6b69 6e64 3d4e  im(value, kind=N
+000131b0: 6f6e 6529 3a0a 2020 2020 2222 220a 2020  one):.    """.  
+000131c0: 2020 3a70 6172 616d 2069 6e74 2076 616c    :param int val
+000131d0: 7565 3a0a 2020 2020 3a70 6172 616d 2045  ue:.    :param E
+000131e0: 6e74 6974 797c 4e6f 6e65 206b 696e 643a  ntity|None kind:
+000131f0: 0a20 2020 203a 7274 7970 653a 2044 696d  .    :rtype: Dim
+00013200: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+00013210: 7572 6e20 5f64 2e44 696d 280a 2020 2020  urn _d.Dim(.    
+00013220: 2020 2020 6469 6d65 6e73 696f 6e3d 7661      dimension=va
+00013230: 6c75 652c 0a20 2020 2020 2020 206b 696e  lue,.        kin
+00013240: 643d 6b69 6e64 206f 7220 4469 6d54 7970  d=kind or DimTyp
+00013250: 6573 2e55 6e73 7065 6369 6669 6564 2c0a  es.Unspecified,.
+00013260: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00013270: 696f 6e3d 2275 6e6e 616d 6564 5f25 7364  ion="unnamed_%sd
+00013280: 696d 5f25 6922 2025 2028 6b69 6e64 2e6e  im_%i" % (kind.n
+00013290: 616d 6520 2b20 225f 2220 6966 206b 696e  ame + "_" if kin
+000132a0: 6420 656c 7365 2022 222c 2076 616c 7565  d else "", value
+000132b0: 292c 0a20 2020 2020 2020 2064 6572 6976  ),.        deriv
+000132c0: 6564 5f66 726f 6d5f 6f70 3d4f 7028 6b69  ed_from_op=Op(ki
+000132d0: 6e64 3d22 636f 6e73 7461 6e74 222c 2069  nd="constant", i
+000132e0: 6e70 7574 733d 5b5d 2c20 6174 7472 6962  nputs=[], attrib
+000132f0: 733d 7b22 7661 6c75 6522 3a20 7661 6c75  s={"value": valu
+00013300: 657d 292c 0a20 2020 2020 2020 2061 7574  e}),.        aut
+00013310: 6f5f 6765 6e65 7261 7465 643d 5472 7565  o_generated=True
+00013320: 2c0a 2020 2020 290a 0a0a 636c 6173 7320  ,.    )...class 
+00013330: 4f70 3a0a 2020 2020 2222 220a 2020 2020  Op:.    """.    
+00013340: 4f70 206f 6e20 3a63 6c61 7373 3a60 4469  Op on :class:`Di
+00013350: 6d60 2077 6869 6368 2072 6573 756c 7473  m` which results
+00013360: 2069 6e20 6120 6465 7269 7665 6420 3a63   in a derived :c
+00013370: 6c61 7373 3a60 4469 6d60 2e0a 2020 2020  lass:`Dim`..    
+00013380: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+00013390: 6e69 745f 5f28 7365 6c66 2c20 6b69 6e64  nit__(self, kind
+000133a0: 2c20 696e 7075 7473 2c20 6174 7472 6962  , inputs, attrib
+000133b0: 733d 4e6f 6e65 293a 0a20 2020 2020 2020  s=None):.       
+000133c0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+000133d0: 7261 6d20 7374 7220 6b69 6e64 3a20 2261  ram str kind: "a
+000133e0: 6464 222c 2022 7375 6222 2c20 226d 756c  dd", "sub", "mul
+000133f0: 222c 2022 6365 696c 6469 7622 0a20 2020  ", "ceildiv".   
+00013400: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
+00013410: 5b44 696d 5d20 696e 7075 7473 3a0a 2020  [Dim] inputs:.  
+00013420: 2020 2020 2020 3a70 6172 616d 2064 6963        :param dic
+00013430: 745b 7374 725d 7c4e 6f6e 6520 6174 7472  t[str]|None attr
+00013440: 6962 733a 0a20 2020 2020 2020 2022 2222  ibs:.        """
+00013450: 0a20 2020 2020 2020 2073 656c 662e 6b69  .        self.ki
+00013460: 6e64 203d 206b 696e 640a 2020 2020 2020  nd = kind.      
+00013470: 2020 7365 6c66 2e69 6e70 7574 7320 3d20    self.inputs = 
+00013480: 696e 7075 7473 0a20 2020 2020 2020 2073  inputs.        s
+00013490: 656c 662e 6f75 7470 7574 203d 204e 6f6e  elf.output = Non
+000134a0: 6520 2023 2074 7970 653a 204f 7074 696f  e  # type: Optio
+000134b0: 6e61 6c5b 5f64 2e44 696d 5d0a 2020 2020  nal[_d.Dim].    
+000134c0: 2020 2020 7365 6c66 2e61 7474 7269 6273      self.attribs
+000134d0: 203d 2061 7474 7269 6273 0a0a 2020 2020   = attribs..    
+000134e0: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
+000134f0: 6629 3a0a 2020 2020 2020 2020 6174 7472  f):.        attr
+00013500: 6962 7320 3d20 2822 2025 7222 2025 2073  ibs = (" %r" % s
+00013510: 656c 662e 6174 7472 6962 7329 2069 6620  elf.attribs) if 
+00013520: 7365 6c66 2e61 7474 7269 6273 2065 6c73  self.attribs els
+00013530: 6520 2222 0a20 2020 2020 2020 2072 6574  e "".        ret
+00013540: 7572 6e20 223c 4469 6d2e 4f70 2025 7220  urn "<Dim.Op %r 
+00013550: 2573 2573 3e22 2025 2028 7365 6c66 2e6b  %s%s>" % (self.k
+00013560: 696e 642c 2073 656c 662e 696e 7075 7473  ind, self.inputs
+00013570: 2c20 6174 7472 6962 7329 0a0a 2020 2020  , attribs)..    
+00013580: 6465 6620 5f76 616c 7565 2873 656c 6629  def _value(self)
+00013590: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000135a0: 2073 656c 662e 6b69 6e64 2c20 7475 706c   self.kind, tupl
+000135b0: 6528 7365 6c66 2e69 6e70 7574 7329 2c20  e(self.inputs), 
+000135c0: 6672 6f7a 656e 7365 7428 7365 6c66 2e61  frozenset(self.a
+000135d0: 7474 7269 6273 2e69 7465 6d73 2829 2920  ttribs.items()) 
+000135e0: 6966 2073 656c 662e 6174 7472 6962 7320  if self.attribs 
+000135f0: 656c 7365 204e 6f6e 650a 0a20 2020 2064  else None..    d
+00013600: 6566 205f 5f68 6173 685f 5f28 7365 6c66  ef __hash__(self
+00013610: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00013620: 6e20 6861 7368 2873 656c 662e 5f76 616c  n hash(self._val
+00013630: 7565 2829 290a 0a20 2020 2064 6566 205f  ue())..    def _
+00013640: 5f65 715f 5f28 7365 6c66 2c20 6f74 6865  _eq__(self, othe
+00013650: 7229 3a0a 2020 2020 2020 2020 6966 2069  r):.        if i
+00013660: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
+00013670: 204f 7029 3a0a 2020 2020 2020 2020 2020   Op):.          
+00013680: 2020 7265 7475 726e 2073 656c 662e 5f76    return self._v
+00013690: 616c 7565 2829 203d 3d20 6f74 6865 722e  alue() == other.
+000136a0: 5f76 616c 7565 2829 0a20 2020 2020 2020  _value().       
+000136b0: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
+000136c0: 2020 2064 6566 205f 5f6e 655f 5f28 7365     def __ne__(se
+000136d0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+000136e0: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+000136f0: 656c 662e 5f5f 6571 5f5f 286f 7468 6572  elf.__eq__(other
+00013700: 290a 0a0a 6465 6620 5f67 6574 5f64 6573  )...def _get_des
+00013710: 6372 6970 7469 6f6e 2864 696d 2c20 6272  cription(dim, br
+00013720: 6163 6b65 7473 3d54 7275 6529 3a0a 2020  ackets=True):.  
+00013730: 2020 2222 220a 2020 2020 3a70 6172 616d    """.    :param
+00013740: 2044 696d 2064 696d 3a0a 2020 2020 3a70   Dim dim:.    :p
+00013750: 6172 616d 2062 6f6f 6c20 6272 6163 6b65  aram bool bracke
+00013760: 7473 3a20 6164 6420 6272 6163 6b65 7473  ts: add brackets
+00013770: 2077 6865 6e20 6e65 6365 7373 6172 790a   when necessary.
+00013780: 2020 2020 3a72 7479 7065 3a20 7374 720a      :rtype: str.
+00013790: 2020 2020 2222 220a 2020 2020 6966 2064      """.    if d
+000137a0: 696d 2e64 6573 6372 6970 7469 6f6e 2061  im.description a
+000137b0: 6e64 2064 696d 2e64 6573 6372 6970 7469  nd dim.descripti
+000137c0: 6f6e 2e73 7461 7274 7377 6974 6828 2275  on.startswith("u
+000137d0: 6e6e 616d 6564 5f22 2920 616e 6420 6469  nnamed_") and di
+000137e0: 6d2e 6469 6d65 6e73 696f 6e20 6973 206e  m.dimension is n
+000137f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00013800: 2072 6574 7572 6e20 7374 7228 6469 6d2e   return str(dim.
+00013810: 6469 6d65 6e73 696f 6e29 0a20 2020 2069  dimension).    i
+00013820: 6620 6469 6d2e 6465 7363 7269 7074 696f  f dim.descriptio
+00013830: 6e3a 0a20 2020 2020 2020 2069 6620 6272  n:.        if br
+00013840: 6163 6b65 7473 3a0a 2020 2020 2020 2020  ackets:.        
+00013850: 2020 2020 696d 706f 7274 2072 650a 0a20      import re.. 
+00013860: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+00013870: 2e73 6561 7263 6828 225b 2b5c 5c2d 2f20  .search("[+\\-/ 
+00013880: 5d22 2c20 6469 6d2e 6465 7363 7269 7074  ]", dim.descript
+00013890: 696f 6e29 3a0a 2020 2020 2020 2020 2020  ion):.          
+000138a0: 2020 2020 2020 7265 7475 726e 2022 2825        return "(%
+000138b0: 7329 2220 2520 6469 6d2e 6465 7363 7269  s)" % dim.descri
+000138c0: 7074 696f 6e0a 2020 2020 2020 2020 7265  ption.        re
+000138d0: 7475 726e 2064 696d 2e64 6573 6372 6970  turn dim.descrip
+000138e0: 7469 6f6e 0a20 2020 2072 6574 7572 6e20  tion.    return 
+000138f0: 2275 6e6e 616d 6564 5f25 735f 6469 6d25  "unnamed_%s_dim%
+00013900: 7322 2025 2028 6469 6d2e 6b69 6e64 2c20  s" % (dim.kind, 
+00013910: 6469 6d2e 6469 6d65 6e73 696f 6e20 6966  dim.dimension if
+00013920: 2064 696d 2e64 696d 656e 7369 6f6e 2069   dim.dimension i
+00013930: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00013940: 223f 2229 0a0a 0a63 6c61 7373 205f 4f70  "?")...class _Op
+00013950: 4d75 6c74 5465 726d 3a0a 2020 2020 2222  MultTerm:.    ""
+00013960: 220a 2020 2020 7265 7072 6573 656e 7473  ".    represents
+00013970: 2073 7468 206c 696b 6520 6120 2a20 6220   sth like a * b 
+00013980: 2a20 630a 2020 2020 2222 220a 0a20 2020  * c.    """..   
+00013990: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+000139a0: 2020 6465 6620 6672 6f6d 5f64 696d 2863    def from_dim(c
+000139b0: 6c73 2c20 6469 6d3a 205f 642e 4469 6d29  ls, dim: _d.Dim)
+000139c0: 202d 3e20 5f4f 704d 756c 7454 6572 6d3a   -> _OpMultTerm:
+000139d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000139e0: 2020 2020 203a 7061 7261 6d20 6469 6d3a       :param dim:
+000139f0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00013a00: 3a20 6f70 206d 756c 7420 7465 726d 0a20  : op mult term. 
+00013a10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013a20: 2020 2064 696d 203d 2064 696d 2e67 6574     dim = dim.get
+00013a30: 5f73 616d 655f 6261 7365 2829 0a20 2020  _same_base().   
+00013a40: 2020 2020 2069 6620 6469 6d2e 6469 6d65       if dim.dime
+00013a50: 6e73 696f 6e20 3d3d 2031 2061 6e64 2064  nsion == 1 and d
+00013a60: 696d 2e69 735f 636f 6e73 7461 6e74 5f73  im.is_constant_s
+00013a70: 7461 7469 635f 6469 6d28 293a 0a20 2020  tatic_dim():.   
+00013a80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00013a90: 636c 732e 6f6e 6528 290a 2020 2020 2020  cls.one().      
+00013aa0: 2020 6966 2064 696d 2e64 6572 6976 6564    if dim.derived
+00013ab0: 5f66 726f 6d5f 6f70 2061 6e64 2064 696d  _from_op and dim
+00013ac0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00013ad0: 2e6b 696e 6420 3d3d 2022 6d75 6c22 3a0a  .kind == "mul":.
+00013ae0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013af0: 726e 2063 6c73 286c 6973 7428 6469 6d2e  rn cls(list(dim.
+00013b00: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00013b10: 696e 7075 7473 2929 0a20 2020 2020 2020  inputs)).       
+00013b20: 2072 6574 7572 6e20 636c 7328 5b64 696d   return cls([dim
+00013b30: 5d29 0a0a 2020 2020 4063 6c61 7373 6d65  ])..    @classme
+00013b40: 7468 6f64 0a20 2020 2064 6566 2066 726f  thod.    def fro
+00013b50: 6d5f 6469 6d5f 6661 6374 6f72 7328 636c  m_dim_factors(cl
+00013b60: 732c 2064 696d 7329 3a0a 2020 2020 2020  s, dims):.      
+00013b70: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00013b80: 6172 616d 206c 6973 745b 4469 6d5d 2064  aram list[Dim] d
+00013b90: 696d 733a 0a20 2020 2020 2020 203a 7274  ims:.        :rt
+00013ba0: 7970 653a 2044 696d 2e5f 4f70 4d75 6c74  ype: Dim._OpMult
+00013bb0: 5465 726d 0a20 2020 2020 2020 2022 2222  Term.        """
+00013bc0: 0a20 2020 2020 2020 2072 6573 203d 2063  .        res = c
+00013bd0: 6c73 2e6f 6e65 2829 0a20 2020 2020 2020  ls.one().       
+00013be0: 2066 6f72 2064 2069 6e20 6469 6d73 3a0a   for d in dims:.
+00013bf0: 2020 2020 2020 2020 2020 2020 7265 732e              res.
+00013c00: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
+00013c10: 642c 206b 696e 643d 226d 756c 222c 2072  d, kind="mul", r
+00013c20: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
+00013c30: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
+00013c40: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00013c50: 2020 2020 6465 6620 6f6e 6528 636c 7329      def one(cls)
+00013c60: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013c70: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
+00013c80: 6d2e 5f4f 704d 756c 7454 6572 6d0a 2020  m._OpMultTerm.  
+00013c90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013ca0: 2020 7265 7475 726e 2063 6c73 285b 5d29    return cls([])
+00013cb0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00013cc0: 5f5f 2873 656c 662c 2074 6572 6d73 293a  __(self, terms):
+00013cd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013ce0: 2020 2020 203a 7061 7261 6d20 6c69 7374       :param list
+00013cf0: 5b44 696d 5d20 7465 726d 733a 0a20 2020  [Dim] terms:.   
+00013d00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013d10: 2073 656c 662e 7465 726d 7320 3d20 7465   self.terms = te
+00013d20: 726d 730a 0a20 2020 2064 6566 205f 5f68  rms..    def __h
+00013d30: 6173 685f 5f28 7365 6c66 293a 0a20 2020  ash__(self):.   
+00013d40: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
+00013d50: 2874 7570 6c65 2873 656c 662e 7465 726d  (tuple(self.term
+00013d60: 7329 290a 0a20 2020 2064 6566 205f 5f65  s))..    def __e
+00013d70: 715f 5f28 7365 6c66 2c20 6f74 6865 7229  q__(self, other)
+00013d80: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00013d90: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+00013da0: 7c44 696d 2e5f 4f70 4d75 6c74 5465 726d  |Dim._OpMultTerm
+00013db0: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+00013dc0: 2222 220a 2020 2020 2020 2020 6966 2069  """.        if i
+00013dd0: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
+00013de0: 205f 4f70 4d75 6c74 5465 726d 293a 0a20   _OpMultTerm):. 
+00013df0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00013e00: 6e20 7365 6c66 2e74 6572 6d73 203d 3d20  n self.terms == 
+00013e10: 6f74 6865 722e 7465 726d 730a 2020 2020  other.terms.    
+00013e20: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00013e30: 0a0a 2020 2020 6465 6620 5f5f 6e65 5f5f  ..    def __ne__
+00013e40: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
+00013e50: 2020 2020 2020 2072 6574 7572 6e20 6e6f         return no
+00013e60: 7420 7365 6c66 2e5f 5f65 715f 5f28 6f74  t self.__eq__(ot
+00013e70: 6865 7229 0a0a 2020 2020 6465 6620 5f5f  her)..    def __
+00013e80: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
+00013e90: 2020 2020 2020 7265 7475 726e 2022 4469        return "Di
+00013ea0: 6d2e 5f4f 704d 756c 7454 6572 6d28 2572  m._OpMultTerm(%r
+00013eb0: 2922 2025 2028 7365 6c66 2e74 6572 6d73  )" % (self.terms
+00013ec0: 2c29 0a0a 2020 2020 4070 726f 7065 7274  ,)..    @propert
+00013ed0: 790a 2020 2020 6465 6620 6469 6d65 6e73  y.    def dimens
+00013ee0: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
+00013ef0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00013f00: 7274 7970 653a 2069 6e74 7c4e 6f6e 650a  rtype: int|None.
+00013f10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013f20: 2020 2020 6469 6d20 3d20 310a 2020 2020      dim = 1.    
+00013f30: 2020 2020 666f 7220 7061 7274 2069 6e20      for part in 
+00013f40: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
+00013f50: 2020 2020 2020 2020 6966 2070 6172 742e          if part.
+00013f60: 6469 6d65 6e73 696f 6e20 6973 204e 6f6e  dimension is Non
+00013f70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00013f80: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00013f90: 2020 2020 2020 2020 2020 2064 696d 202a             dim *
+00013fa0: 3d20 7061 7274 2e64 696d 656e 7369 6f6e  = part.dimension
+00013fb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013fc0: 6469 6d0a 0a20 2020 2064 6566 2062 6173  dim..    def bas
+00013fd0: 655f 7465 726d 2873 656c 6629 3a0a 2020  e_term(self):.  
+00013fe0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013ff0: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
+00014000: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00014010: 2020 6173 7365 7274 2073 656c 662e 7465    assert self.te
+00014020: 726d 730a 2020 2020 2020 2020 7265 7475  rms.        retu
+00014030: 726e 2073 656c 662e 7465 726d 735b 2d31  rn self.terms[-1
+00014040: 5d0a 0a20 2020 2064 6566 2069 735f 6f6e  ]..    def is_on
+00014050: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00014060: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+00014070: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+00014080: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00014090: 7475 726e 206e 6f74 2073 656c 662e 7465  turn not self.te
+000140a0: 726d 730a 0a20 2020 2064 6566 2069 735f  rms..    def is_
+000140b0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
+000140c0: 6469 6d28 7365 6c66 293a 0a20 2020 2020  dim(self):.     
+000140d0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+000140e0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
+000140f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014100: 6966 206e 6f74 2073 656c 662e 7465 726d  if not self.term
+00014110: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+00014120: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00014130: 2020 2072 6574 7572 6e20 616c 6c28 7465     return all(te
+00014140: 726d 2e69 735f 636f 6e73 7461 6e74 5f73  rm.is_constant_s
+00014150: 7461 7469 635f 6469 6d28 2920 666f 7220  tatic_dim() for 
+00014160: 7465 726d 2069 6e20 7365 6c66 2e74 6572  term in self.ter
+00014170: 6d73 290a 0a20 2020 2064 6566 2063 6f70  ms)..    def cop
+00014180: 7928 7365 6c66 293a 0a20 2020 2020 2020  y(self):.       
+00014190: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+000141a0: 7970 653a 2044 696d 2e5f 4f70 4d75 6c74  ype: Dim._OpMult
+000141b0: 5465 726d 0a20 2020 2020 2020 2022 2222  Term.        """
+000141c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000141d0: 5f4f 704d 756c 7454 6572 6d28 6c69 7374  _OpMultTerm(list
+000141e0: 2873 656c 662e 7465 726d 7329 290a 0a20  (self.terms)).. 
+000141f0: 2020 2064 6566 206e 6567 6174 6976 6528     def negative(
+00014200: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00014210: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
+00014220: 653a 2044 696d 2e5f 4f70 4d75 6c74 5465  e: Dim._OpMultTe
+00014230: 726d 0a20 2020 2020 2020 2022 2222 0a20  rm.        """. 
+00014240: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00014250: 6572 6d73 2061 6e64 2073 656c 662e 7465  erms and self.te
+00014260: 726d 735b 305d 2e69 735f 636f 6e73 7461  rms[0].is_consta
+00014270: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
+00014280: 616e 6420 7365 6c66 2e74 6572 6d73 5b30  and self.terms[0
+00014290: 5d2e 6469 6d65 6e73 696f 6e20 3d3d 202d  ].dimension == -
+000142a0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
+000142b0: 6574 7572 6e20 5f4f 704d 756c 7454 6572  eturn _OpMultTer
+000142c0: 6d28 7365 6c66 2e74 6572 6d73 5b31 3a5d  m(self.terms[1:]
+000142d0: 290a 2020 2020 2020 2020 7265 7320 3d20  ).        res = 
+000142e0: 7365 6c66 2e63 6f70 7928 290a 2020 2020  self.copy().    
+000142f0: 2020 2020 7265 732e 6578 7465 6e64 5f6d      res.extend_m
+00014300: 756c 5f64 6976 5f28 5f6d 616b 655f 636f  ul_div_(_make_co
+00014310: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
+00014320: 6d28 2d31 292c 206b 696e 643d 226d 756c  m(-1), kind="mul
+00014330: 222c 2072 6967 6874 3d46 616c 7365 290a  ", right=False).
+00014340: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00014350: 6573 0a0a 2020 2020 6465 6620 6469 7669  es..    def divi
+00014360: 7369 626c 6528 7365 6c66 2c20 6f74 6865  sible(self, othe
+00014370: 722c 2072 6967 6874 293a 0a20 2020 2020  r, right):.     
+00014380: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00014390: 7061 7261 6d20 4469 6d20 6f74 6865 723a  param Dim other:
+000143a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000143b0: 626f 6f6c 2072 6967 6874 3a0a 2020 2020  bool right:.    
+000143c0: 2020 2020 3a72 6574 7572 6e3a 2077 6865      :return: whe
+000143d0: 7468 6572 2077 6520 6361 6e20 6469 7669  ther we can divi
+000143e0: 6465 206f 7468 6572 2c20 7769 7468 6f75  de other, withou
+000143f0: 7420 7265 6d61 696e 6465 720a 2020 2020  t remainder.    
+00014400: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00014410: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014420: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00014430: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+00014440: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00014450: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
+00014460: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00014470: 7020 616e 6420 6f74 6865 722e 6465 7269  p and other.deri
+00014480: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+00014490: 203d 3d20 226d 756c 223a 0a20 2020 2020   == "mul":.     
+000144a0: 2020 2020 2020 2074 6d70 203d 2073 656c         tmp = sel
+000144b0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+000144c0: 2020 2020 2066 6f72 2074 6572 6d20 696e       for term in
+000144d0: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
+000144e0: 726f 6d5f 6f70 2e69 6e70 7574 7320 6966  rom_op.inputs if
+000144f0: 2072 6967 6874 2065 6c73 6520 7265 7665   right else reve
+00014500: 7273 6564 286f 7468 6572 2e64 6572 6976  rsed(other.deriv
+00014510: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
+00014520: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00014530: 2020 2020 6966 206e 6f74 2074 6d70 2e64      if not tmp.d
+00014540: 6976 6973 6962 6c65 2874 6572 6d2c 2072  ivisible(term, r
+00014550: 6967 6874 3d72 6967 6874 293a 0a20 2020  ight=right):.   
+00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014570: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00014580: 2020 2020 2020 2020 2020 2020 2020 746d                tm
+00014590: 702e 6578 7465 6e64 5f6d 756c 5f64 6976  p.extend_mul_div
+000145a0: 5f28 7465 726d 2c20 6b69 6e64 3d22 7472  _(term, kind="tr
+000145b0: 7565 6469 7622 2c20 7269 6768 743d 7269  uediv", right=ri
+000145c0: 6768 7429 0a20 2020 2020 2020 2020 2020  ght).           
+000145d0: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+000145e0: 2020 2020 206d 6f73 745f 7265 6365 6e74       most_recent
+000145f0: 5f74 6572 6d20 3d20 7365 6c66 2e74 6572  _term = self.ter
+00014600: 6d73 5b2d 3120 6966 2072 6967 6874 2065  ms[-1 if right e
+00014610: 6c73 6520 305d 0a20 2020 2020 2020 2069  lse 0].        i
+00014620: 6620 6f74 6865 7220 3d3d 206d 6f73 745f  f other == most_
+00014630: 7265 6365 6e74 5f74 6572 6d3a 0a20 2020  recent_term:.   
+00014640: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00014650: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
+00014660: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
+00014670: 2e64 696d 656e 7369 6f6e 2069 7320 6e6f  .dimension is no
+00014680: 7420 4e6f 6e65 2061 6e64 206f 7468 6572  t None and other
+00014690: 2e64 696d 656e 7369 6f6e 2069 7320 6e6f  .dimension is no
+000146a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000146b0: 2020 2020 6966 206d 6f73 745f 7265 6365      if most_rece
+000146c0: 6e74 5f74 6572 6d2e 6469 6d65 6e73 696f  nt_term.dimensio
+000146d0: 6e20 2520 6f74 6865 722e 6469 6d65 6e73  n % other.dimens
+000146e0: 696f 6e20 3d3d 2030 3a0a 2020 2020 2020  ion == 0:.      
+000146f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014700: 2054 7275 650a 2020 2020 2020 2020 7265   True.        re
+00014710: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+00014720: 6465 6620 6361 6e5f 7369 6d70 6c69 6679  def can_simplify
+00014730: 2873 656c 662c 206f 7468 6572 2c20 6b69  (self, other, ki
+00014740: 6e64 2c20 7269 6768 7429 3a0a 2020 2020  nd, right):.    
+00014750: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014760: 3a70 6172 616d 2044 696d 206f 7468 6572  :param Dim other
+00014770: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+00014780: 2073 7472 206b 696e 643a 0a20 2020 2020   str kind:.     
+00014790: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
+000147a0: 6967 6874 3a0a 2020 2020 2020 2020 3a72  ight:.        :r
+000147b0: 6574 7572 6e3a 2077 6865 7468 6572 2077  eturn: whether w
+000147c0: 6520 6361 6e20 7369 6d70 6c69 6679 2077  e can simplify w
+000147d0: 6865 6e20 6170 706c 7969 6e67 2074 6869  hen applying thi
+000147e0: 7320 6f70 6572 6174 696f 6e0a 2020 2020  s operation.    
+000147f0: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00014800: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014810: 2020 2020 2069 6620 6f74 6865 722e 6465       if other.de
+00014820: 7269 7665 645f 6672 6f6d 5f6f 7020 616e  rived_from_op an
+00014830: 6420 6f74 6865 722e 6465 7269 7665 645f  d other.derived_
+00014840: 6672 6f6d 5f6f 702e 6b69 6e64 203d 3d20  from_op.kind == 
+00014850: 226d 756c 223a 0a20 2020 2020 2020 2020  "mul":.         
+00014860: 2020 2074 6d70 203d 2073 656c 662e 636f     tmp = self.co
+00014870: 7079 2829 0a20 2020 2020 2020 2020 2020  py().           
+00014880: 2066 6f72 2074 6572 6d20 696e 206f 7468   for term in oth
+00014890: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
+000148a0: 6f70 2e69 6e70 7574 7320 6966 2072 6967  op.inputs if rig
+000148b0: 6874 2065 6c73 6520 7265 7665 7273 6564  ht else reversed
+000148c0: 286f 7468 6572 2e64 6572 6976 6564 5f66  (other.derived_f
+000148d0: 726f 6d5f 6f70 2e69 6e70 7574 7329 3a0a  rom_op.inputs):.
+000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148f0: 6966 206e 6f74 2074 6d70 2e63 616e 5f73  if not tmp.can_s
+00014900: 696d 706c 6966 7928 7465 726d 2c20 6b69  implify(term, ki
+00014910: 6e64 3d6b 696e 642c 2072 6967 6874 3d72  nd=kind, right=r
+00014920: 6967 6874 293a 0a20 2020 2020 2020 2020  ight):.         
+00014930: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00014940: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00014950: 2020 2020 2020 2020 746d 702e 6578 7465          tmp.exte
+00014960: 6e64 5f6d 756c 5f64 6976 5f28 7465 726d  nd_mul_div_(term
+00014970: 2c20 6b69 6e64 3d6b 696e 642c 2072 6967  , kind=kind, rig
+00014980: 6874 3d72 6967 6874 290a 2020 2020 2020  ht=right).      
+00014990: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+000149a0: 650a 2020 2020 2020 2020 6964 7820 3d20  e.        idx = 
+000149b0: 7365 6c66 2e5f 7369 6d70 6c69 6679 5f74  self._simplify_t
+000149c0: 6572 6d5f 6964 7828 6f74 6865 722c 206b  erm_idx(other, k
+000149d0: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
+000149e0: 7269 6768 7429 0a20 2020 2020 2020 2072  right).        r
+000149f0: 6574 7572 6e20 6964 7820 6973 206e 6f74  eturn idx is not
+00014a00: 204e 6f6e 650a 0a20 2020 2064 6566 205f   None..    def _
+00014a10: 7369 6d70 6c69 6679 5f74 6572 6d5f 6964  simplify_term_id
+00014a20: 7828 7365 6c66 2c20 6f74 6865 722c 206b  x(self, other, k
+00014a30: 696e 642c 2072 6967 6874 293a 0a20 2020  ind, right):.   
+00014a40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014a50: 203a 7061 7261 6d20 4469 6d20 6f74 6865   :param Dim othe
+00014a60: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
+00014a70: 6d20 7374 7220 6b69 6e64 3a0a 2020 2020  m str kind:.    
+00014a80: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
+00014a90: 7269 6768 743a 0a20 2020 2020 2020 203a  right:.        :
+00014aa0: 7265 7475 726e 3a20 696e 6465 7820 6f66  return: index of
+00014ab0: 2074 6572 6d20 746f 2073 696d 706c 6966   term to simplif
+00014ac0: 790a 2020 2020 2020 2020 3a72 7479 7065  y.        :rtype
+00014ad0: 3a20 696e 747c 4e6f 6e65 0a20 2020 2020  : int|None.     
+00014ae0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00014af0: 6620 6e6f 7420 7365 6c66 2e74 6572 6d73  f not self.terms
+00014b00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00014b10: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
+00014b20: 2020 6966 206b 696e 6420 3d3d 2022 6d75    if kind == "mu
+00014b30: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
+00014b40: 2320 5765 2077 616e 7420 2862 202a 2061  # We want (b * a
+00014b50: 2920 2f2f 2062 2021 3d20 612e 0a20 2020  ) // b != a..   
+00014b60: 2020 2020 2020 2020 2023 2048 6f77 6576           # Howev
+00014b70: 6572 2c20 7765 2077 616e 7420 6820 2a20  er, we want h * 
+00014b80: 2832 202a 2061 202f 2f20 6829 203d 3d20  (2 * a // h) == 
+00014b90: 3220 2a20 612e 0a20 2020 2020 2020 2020  2 * a..         
+00014ba0: 2020 2023 2053 6f2c 2066 6f72 2060 6d75     # So, for `mu
+00014bb0: 6c60 2c20 616e 6420 6f6e 6c79 2066 6f72  l`, and only for
+00014bc0: 2060 6d75 6c60 2c20 6368 6563 6b20 616c   `mul`, check al
+00014bd0: 6c20 7465 726d 732c 2077 6865 7468 6572  l terms, whether
+00014be0: 2077 6520 6361 6e20 7369 6d70 6c69 6679   we can simplify
+00014bf0: 2073 6f6d 6520 6469 7669 7369 6f6e 2d74   some division-t
+00014c00: 6572 6d2e 0a20 2020 2020 2020 2020 2020  erm..           
+00014c10: 2066 6f72 2069 2c20 7465 726d 2069 6e20   for i, term in 
+00014c20: 7265 7665 7273 6564 286c 6973 7428 656e  reversed(list(en
+00014c30: 756d 6572 6174 6528 7365 6c66 2e74 6572  umerate(self.ter
+00014c40: 6d73 2929 2920 6966 2072 6967 6874 2065  ms))) if right e
+00014c50: 6c73 6520 656e 756d 6572 6174 6528 7365  lse enumerate(se
+00014c60: 6c66 2e74 6572 6d73 293a 0a20 2020 2020  lf.terms):.     
+00014c70: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00014c80: 7420 6973 696e 7374 616e 6365 2874 6572  t isinstance(ter
+00014c90: 6d2c 205f 642e 4469 6d29 0a20 2020 2020  m, _d.Dim).     
+00014ca0: 2020 2020 2020 2020 2020 2069 6620 7465             if te
+00014cb0: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
+00014cc0: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
+00014cd0: 2020 2020 2020 2020 6966 2074 6572 6d2e          if term.
+00014ce0: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00014cf0: 6b69 6e64 203d 3d20 2274 7275 6564 6976  kind == "truediv
+00014d00: 5f22 202b 2028 2272 6967 6874 2220 6966  _" + ("right" if
+00014d10: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
+00014d20: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
+00014d30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014d40: 7465 726d 2e64 6572 6976 6564 5f66 726f  term.derived_fro
+00014d50: 6d5f 6f70 2e69 6e70 7574 735b 2d31 5d20  m_op.inputs[-1] 
+00014d60: 3d3d 206f 7468 6572 3a0a 2020 2020 2020  == other:.      
+00014d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d80: 2020 2020 2020 7265 7475 726e 2069 0a20        return i. 
+00014d90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014da0: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
+00014db0: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
+00014dc0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014dd0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00014de0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
+00014df0: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
+00014e00: 6874 2220 6966 206e 6f74 2072 6967 6874  ht" if not right
+00014e10: 2065 6c73 6520 226c 6566 7422 293a 0a20   else "left"):. 
+00014e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e30: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
+00014e40: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00014e50: 696e 7075 7473 5b2d 315d 203d 3d20 7465  inputs[-1] == te
+00014e60: 726d 3a0a 2020 2020 2020 2020 2020 2020  rm:.            
+00014e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e80: 7265 7475 726e 2069 0a20 2020 2020 2020  return i.       
+00014e90: 2020 2020 2020 2020 2069 6620 7465 726d           if term
+00014ea0: 2e69 735f 636f 6e73 7461 6e74 5f73 7461  .is_constant_sta
+00014eb0: 7469 635f 6469 6d28 2920 616e 6420 6f74  tic_dim() and ot
+00014ec0: 6865 722e 6973 5f63 6f6e 7374 616e 745f  her.is_constant_
+00014ed0: 7374 6174 6963 5f64 696d 2829 3a0a 2020  static_dim():.  
+00014ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ef0: 2020 7265 7475 726e 2069 0a20 2020 2020    return i.     
+00014f00: 2020 2023 2046 6f72 2074 6865 206c 6173     # For the las
+00014f10: 742f 6669 7273 7420 7465 726d 2c20 6578  t/first term, ex
+00014f20: 7472 6120 6368 6563 6b73 2e0a 2020 2020  tra checks..    
+00014f30: 2020 2020 6920 3d20 6c65 6e28 7365 6c66      i = len(self
+00014f40: 2e74 6572 6d73 2920 2d20 3120 6966 2072  .terms) - 1 if r
+00014f50: 6967 6874 2065 6c73 6520 300a 2020 2020  ight else 0.    
+00014f60: 2020 2020 7465 726d 203d 2073 656c 662e      term = self.
+00014f70: 7465 726d 735b 695d 0a20 2020 2020 2020  terms[i].       
+00014f80: 2069 6620 6b69 6e64 2e65 6e64 7377 6974   if kind.endswit
+00014f90: 6828 2264 6976 2229 2061 6e64 206f 7468  h("div") and oth
+00014fa0: 6572 203d 3d20 7465 726d 3a0a 2020 2020  er == term:.    
+00014fb0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00014fc0: 0a20 2020 2020 2020 206f 705f 6b69 6e64  .        op_kind
+00014fd0: 203d 206b 696e 6420 2b20 225f 2220 2b20   = kind + "_" + 
+00014fe0: 2822 7269 6768 7422 2069 6620 7269 6768  ("right" if righ
+00014ff0: 7420 656c 7365 2022 6c65 6674 2229 0a20  t else "left"). 
+00015000: 2020 2020 2020 2069 6620 7465 726d 2e64         if term.d
+00015010: 6572 6976 6564 5f66 726f 6d5f 6f70 2061  erived_from_op a
+00015020: 6e64 2074 6572 6d2e 6465 7269 7665 645f  nd term.derived_
+00015030: 6672 6f6d 5f6f 702e 6b69 6e64 203d 3d20  from_op.kind == 
+00015040: 6f70 5f6b 696e 643a 0a20 2020 2020 2020  op_kind:.       
+00015050: 2020 2020 2072 6574 7572 6e20 690a 2020       return i.  
+00015060: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00015070: 650a 0a20 2020 2064 6566 2065 7874 656e  e..    def exten
+00015080: 645f 6d75 6c5f 6469 765f 2873 656c 662c  d_mul_div_(self,
+00015090: 206f 7468 6572 2c20 6b69 6e64 2c20 7269   other, kind, ri
+000150a0: 6768 7429 3a0a 2020 2020 2020 2020 2222  ght):.        ""
+000150b0: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+000150c0: 2044 696d 206f 7468 6572 3a0a 2020 2020   Dim other:.    
+000150d0: 2020 2020 3a70 6172 616d 2073 7472 206b      :param str k
+000150e0: 696e 643a 0a20 2020 2020 2020 203a 7061  ind:.        :pa
+000150f0: 7261 6d20 626f 6f6c 2072 6967 6874 3a0a  ram bool right:.
+00015100: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015110: 2020 2020 6173 7365 7274 206b 696e 6420      assert kind 
+00015120: 696e 207b 226d 756c 222c 2022 666c 6f6f  in {"mul", "floo
+00015130: 7264 6976 222c 2022 7472 7565 6469 7622  rdiv", "truediv"
+00015140: 2c20 2263 6569 6c64 6976 227d 0a20 2020  , "ceildiv"}.   
+00015150: 2020 2020 2069 6620 6f74 6865 722e 6973       if other.is
+00015160: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
+00015170: 5f64 696d 2829 2061 6e64 206f 7468 6572  _dim() and other
+00015180: 2e64 696d 656e 7369 6f6e 203d 3d20 313a  .dimension == 1:
+00015190: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000151a0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
+000151b0: 6f74 2073 656c 662e 7465 726d 733a 0a20  ot self.terms:. 
+000151c0: 2020 2020 2020 2020 2020 2069 6620 6b69             if ki
+000151d0: 6e64 203d 3d20 226d 756c 223a 0a20 2020  nd == "mul":.   
+000151e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000151f0: 662e 7465 726d 732e 6170 7065 6e64 286f  f.terms.append(o
+00015200: 7468 6572 290a 2020 2020 2020 2020 2020  ther).          
+00015210: 2020 656c 6966 206b 696e 642e 656e 6473    elif kind.ends
+00015220: 7769 7468 2822 6469 7622 293a 0a20 2020  with("div"):.   
+00015230: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015240: 662e 7465 726d 7320 3d20 5b5f 4f70 4d75  f.terms = [_OpMu
+00015250: 6c74 5465 726d 2e6e 6577 5f64 6976 5f64  ltTerm.new_div_d
+00015260: 696d 2873 656c 662e 6173 5f64 696d 2829  im(self.as_dim()
+00015270: 2c20 6f74 6865 722c 206b 696e 643d 6b69  , other, kind=ki
+00015280: 6e64 2c20 7269 6768 743d 7269 6768 7429  nd, right=right)
+00015290: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
+000152a0: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+000152b0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+000152c0: 6f6d 5f6f 7020 616e 6420 6f74 6865 722e  om_op and other.
+000152d0: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+000152e0: 6b69 6e64 203d 3d20 226d 756c 223a 0a20  kind == "mul":. 
+000152f0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+00015300: 6572 6d20 696e 206f 7468 6572 2e64 6572  erm in other.der
+00015310: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
+00015320: 7574 7320 6966 2072 6967 6874 2065 6c73  uts if right els
+00015330: 6520 7265 7665 7273 6564 286f 7468 6572  e reversed(other
+00015340: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015350: 2e69 6e70 7574 7329 3a0a 2020 2020 2020  .inputs):.      
+00015360: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+00015370: 7874 656e 645f 6d75 6c5f 6469 765f 2874  xtend_mul_div_(t
+00015380: 6572 6d2c 206b 696e 643d 6b69 6e64 2c20  erm, kind=kind, 
+00015390: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
+000153a0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000153b0: 2020 2020 2020 2020 6964 7820 3d20 7365          idx = se
+000153c0: 6c66 2e5f 7369 6d70 6c69 6679 5f74 6572  lf._simplify_ter
+000153d0: 6d5f 6964 7828 6f74 6865 722c 206b 696e  m_idx(other, kin
+000153e0: 643d 6b69 6e64 2c20 7269 6768 743d 7269  d=kind, right=ri
+000153f0: 6768 7429 0a20 2020 2020 2020 2069 6620  ght).        if 
+00015400: 6964 7820 6973 206e 6f74 204e 6f6e 653a  idx is not None:
+00015410: 0a20 2020 2020 2020 2020 2020 2074 6572  .            ter
+00015420: 6d20 3d20 7365 6c66 2e74 6572 6d73 5b69  m = self.terms[i
+00015430: 6478 5d0a 2020 2020 2020 2020 2020 2020  dx].            
+00015440: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+00015450: 6528 7465 726d 2c20 5f64 2e44 696d 290a  e(term, _d.Dim).
+00015460: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00015470: 696e 642e 656e 6473 7769 7468 2822 6469  ind.endswith("di
+00015480: 7622 2920 616e 6420 6f74 6865 7220 3d3d  v") and other ==
+00015490: 2074 6572 6d3a 0a20 2020 2020 2020 2020   term:.         
+000154a0: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
+000154b0: 732e 706f 7028 6964 7829 0a20 2020 2020  s.pop(idx).     
+000154c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000154d0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+000154e0: 206b 696e 6420 3d3d 2022 6d75 6c22 2061   kind == "mul" a
+000154f0: 6e64 2074 6572 6d2e 6465 7269 7665 645f  nd term.derived_
+00015500: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
+00015510: 2020 2020 2020 2020 2069 6620 7465 726d           if term
+00015520: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015530: 2e6b 696e 6420 3d3d 2022 7472 7565 6469  .kind == "truedi
+00015540: 765f 2220 2b20 2822 7269 6768 7422 2069  v_" + ("right" i
+00015550: 6620 7269 6768 7420 656c 7365 2022 6c65  f right else "le
+00015560: 6674 2229 3a0a 2020 2020 2020 2020 2020  ft"):.          
+00015570: 2020 2020 2020 2020 2020 6966 2074 6572            if ter
+00015580: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
+00015590: 702e 696e 7075 7473 5b2d 315d 203d 3d20  p.inputs[-1] == 
+000155a0: 6f74 6865 723a 0a20 2020 2020 2020 2020  other:.         
+000155b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000155c0: 656c 662e 7465 726d 735b 6964 785d 203d  elf.terms[idx] =
+000155d0: 2074 6572 6d2e 6465 7269 7665 645f 6672   term.derived_fr
+000155e0: 6f6d 5f6f 702e 696e 7075 7473 5b30 5d0a  om_op.inputs[0].
+000155f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015600: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00015610: 2020 2020 2020 2020 2020 2069 6620 6b69             if ki
+00015620: 6e64 203d 3d20 226d 756c 2220 616e 6420  nd == "mul" and 
+00015630: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00015640: 6f6d 5f6f 703a 0a20 2020 2020 2020 2020  om_op:.         
+00015650: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
+00015660: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00015670: 6b69 6e64 203d 3d20 2274 7275 6564 6976  kind == "truediv
+00015680: 5f22 202b 2028 2272 6967 6874 2220 6966  _" + ("right" if
+00015690: 206e 6f74 2072 6967 6874 2065 6c73 6520   not right else 
+000156a0: 226c 6566 7422 293a 0a20 2020 2020 2020  "left"):.       
+000156b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000156c0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+000156d0: 6f6d 5f6f 702e 696e 7075 7473 5b2d 315d  om_op.inputs[-1]
+000156e0: 203d 3d20 7465 726d 3a0a 2020 2020 2020   == term:.      
+000156f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015700: 2020 7365 6c66 2e74 6572 6d73 5b69 6478    self.terms[idx
+00015710: 5d20 3d20 6f74 6865 722e 6465 7269 7665  ] = other.derive
+00015720: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
+00015730: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00015740: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015750: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
+00015760: 6620 7465 726d 2e69 735f 636f 6e73 7461  f term.is_consta
+00015770: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
+00015780: 616e 6420 6f74 6865 722e 6973 5f63 6f6e  and other.is_con
+00015790: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
+000157a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000157b0: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
+000157c0: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
+000157d0: 2020 2020 2020 2020 2020 6966 2074 6572            if ter
+000157e0: 6d2e 6469 6d65 6e73 696f 6e20 2a20 6f74  m.dimension * ot
+000157f0: 6865 722e 6469 6d65 6e73 696f 6e20 3d3d  her.dimension ==
+00015800: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00015810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015820: 2e74 6572 6d73 2e70 6f70 2869 6478 290a  .terms.pop(idx).
+00015830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015840: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00015850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015860: 2020 2073 656c 662e 7465 726d 735b 6964     self.terms[id
+00015870: 785d 203d 205f 6d61 6b65 5f63 6f6e 7374  x] = _make_const
+00015880: 616e 745f 7374 6174 6963 5f64 696d 2874  ant_static_dim(t
+00015890: 6572 6d2e 6469 6d65 6e73 696f 6e20 2a20  erm.dimension * 
+000158a0: 6f74 6865 722e 6469 6d65 6e73 696f 6e2c  other.dimension,
+000158b0: 206b 696e 643d 7465 726d 2e6b 696e 6429   kind=term.kind)
+000158c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000158d0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+000158e0: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+000158f0: 696e 642e 656e 6473 7769 7468 2822 6469  ind.endswith("di
+00015900: 7622 2920 616e 6420 7465 726d 2e64 696d  v") and term.dim
+00015910: 656e 7369 6f6e 2025 206f 7468 6572 2e64  ension % other.d
+00015920: 696d 656e 7369 6f6e 203d 3d20 303a 0a20  imension == 0:. 
+00015930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015940: 2020 2073 656c 662e 7465 726d 735b 6964     self.terms[id
+00015950: 785d 203d 205f 6d61 6b65 5f63 6f6e 7374  x] = _make_const
+00015960: 616e 745f 7374 6174 6963 5f64 696d 2874  ant_static_dim(t
+00015970: 6572 6d2e 6469 6d65 6e73 696f 6e20 2f2f  erm.dimension //
+00015980: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
+00015990: 2c20 6b69 6e64 3d74 6572 6d2e 6b69 6e64  , kind=term.kind
+000159a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000159b0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000159c0: 2020 2020 2020 2020 2020 2020 2023 2046               # F
+000159d0: 616c 6c62 6163 6b20 7769 7468 2067 656e  allback with gen
+000159e0: 6572 6963 2068 616e 646c 696e 672e 0a20  eric handling.. 
+000159f0: 2020 2020 2020 2020 2020 206f 705f 6b69             op_ki
+00015a00: 6e64 203d 206b 696e 6420 2b20 225f 2220  nd = kind + "_" 
+00015a10: 2b20 2822 7269 6768 7422 2069 6620 7269  + ("right" if ri
+00015a20: 6768 7420 656c 7365 2022 6c65 6674 2229  ght else "left")
+00015a30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00015a40: 6b69 6e64 2e65 6e64 7377 6974 6828 2264  kind.endswith("d
+00015a50: 6976 2229 2061 6e64 2074 6572 6d2e 6465  iv") and term.de
+00015a60: 7269 7665 645f 6672 6f6d 5f6f 7020 616e  rived_from_op an
+00015a70: 6420 7465 726d 2e64 6572 6976 6564 5f66  d term.derived_f
+00015a80: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 206f  rom_op.kind == o
+00015a90: 705f 6b69 6e64 3a0a 2020 2020 2020 2020  p_kind:.        
+00015aa0: 2020 2020 2020 2020 6e75 6d65 7261 746f          numerato
+00015ab0: 7220 3d20 7465 726d 2e64 6572 6976 6564  r = term.derived
+00015ac0: 5f66 726f 6d5f 6f70 2e69 6e70 7574 735b  _from_op.inputs[
+00015ad0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+00015ae0: 2020 2064 656e 6f6d 696e 6174 6f72 203d     denominator =
+00015af0: 2074 6572 6d2e 6465 7269 7665 645f 6672   term.derived_fr
+00015b00: 6f6d 5f6f 702e 696e 7075 7473 5b31 5d0a  om_op.inputs[1].
+00015b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b20: 7365 6c66 2e74 6572 6d73 5b69 6478 5d20  self.terms[idx] 
+00015b30: 3d20 5f4f 704d 756c 7454 6572 6d2e 6e65  = _OpMultTerm.ne
+00015b40: 775f 6469 765f 6469 6d28 6e75 6d65 7261  w_div_dim(numera
+00015b50: 746f 722c 2064 656e 6f6d 696e 6174 6f72  tor, denominator
+00015b60: 202a 206f 7468 6572 2c20 6b69 6e64 3d6b   * other, kind=k
+00015b70: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
+00015b80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015b90: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00015ba0: 2069 6620 6b69 6e64 2e65 6e64 7377 6974   if kind.endswit
+00015bb0: 6828 2264 6976 2229 3a0a 2020 2020 2020  h("div"):.      
+00015bc0: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
+00015bd0: 203d 205b 5f4f 704d 756c 7454 6572 6d2e   = [_OpMultTerm.
+00015be0: 6e65 775f 6469 765f 6469 6d28 7365 6c66  new_div_dim(self
+00015bf0: 2e61 735f 6469 6d28 292c 206f 7468 6572  .as_dim(), other
+00015c00: 2c20 6b69 6e64 3d6b 696e 642c 2072 6967  , kind=kind, rig
+00015c10: 6874 3d72 6967 6874 295d 0a20 2020 2020  ht=right)].     
+00015c20: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00015c30: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
+00015c40: 2022 6d75 6c22 3a0a 2020 2020 2020 2020   "mul":.        
+00015c50: 2020 2020 6966 2072 6967 6874 3a0a 2020      if right:.  
+00015c60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015c70: 6c66 2e74 6572 6d73 2e61 7070 656e 6428  lf.terms.append(
+00015c80: 6f74 6865 7229 0a20 2020 2020 2020 2020  other).         
+00015c90: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00015ca0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00015cb0: 726d 732e 696e 7365 7274 2830 2c20 6f74  rms.insert(0, ot
+00015cc0: 6865 7229 0a20 2020 2020 2020 2020 2020  her).           
+00015cd0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00015ce0: 6173 7365 7274 2046 616c 7365 0a0a 2020  assert False..  
+00015cf0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00015d00: 2020 2064 6566 206e 6577 5f64 6976 5f64     def new_div_d
+00015d10: 696d 2863 6c73 2c20 6e75 6d65 7261 746f  im(cls, numerato
+00015d20: 722c 2064 656e 6f6d 696e 6174 6f72 2c20  r, denominator, 
+00015d30: 6b69 6e64 2c20 7269 6768 7429 3a0a 2020  kind, right):.  
+00015d40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015d50: 2020 3a70 6172 616d 2044 696d 206e 756d    :param Dim num
+00015d60: 6572 6174 6f72 3a0a 2020 2020 2020 2020  erator:.        
+00015d70: 3a70 6172 616d 2044 696d 2064 656e 6f6d  :param Dim denom
+00015d80: 696e 6174 6f72 3a0a 2020 2020 2020 2020  inator:.        
+00015d90: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
+00015da0: 2022 666c 6f6f 7264 6976 2220 6f72 2022   "floordiv" or "
+00015db0: 6365 696c 6469 7622 206f 7220 2274 7275  ceildiv" or "tru
+00015dc0: 6564 6976 220a 2020 2020 2020 2020 3a70  ediv".        :p
+00015dd0: 6172 616d 2062 6f6f 6c20 7269 6768 743a  aram bool right:
+00015de0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00015df0: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00015e00: 0a20 2020 2020 2020 2064 696d 5f76 616c  .        dim_val
+00015e10: 7565 203d 204e 6f6e 650a 2020 2020 2020  ue = None.      
+00015e20: 2020 6120 3d20 6e75 6d65 7261 746f 722e    a = numerator.
+00015e30: 6469 6d65 6e73 696f 6e0a 2020 2020 2020  dimension.      
+00015e40: 2020 6220 3d20 6465 6e6f 6d69 6e61 746f    b = denominato
+00015e50: 722e 6469 6d65 6e73 696f 6e0a 2020 2020  r.dimension.    
+00015e60: 2020 2020 6966 2061 2069 7320 6e6f 7420      if a is not 
+00015e70: 4e6f 6e65 2061 6e64 2062 2069 7320 6e6f  None and b is no
+00015e80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00015e90: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
+00015ea0: 666c 6f6f 7264 6976 223a 0a20 2020 2020  floordiv":.     
+00015eb0: 2020 2020 2020 2020 2020 2064 696d 5f76             dim_v
+00015ec0: 616c 7565 203d 2061 202f 2f20 620a 2020  alue = a // b.  
+00015ed0: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
+00015ee0: 696e 6420 3d3d 2022 6365 696c 6469 7622  ind == "ceildiv"
+00015ef0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015f00: 2020 6469 6d5f 7661 6c75 6520 3d20 2d28    dim_value = -(
+00015f10: 2d61 202f 2f20 6229 0a20 2020 2020 2020  -a // b).       
+00015f20: 2020 2020 2020 2020 2069 6620 6120 2520           if a % 
+00015f30: 6220 3d3d 2030 2061 6e64 2072 6967 6874  b == 0 and right
+00015f40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015f50: 2020 2020 2020 6b69 6e64 203d 2022 666c        kind = "fl
+00015f60: 6f6f 7264 6976 2220 2023 2066 6f72 206e  oordiv"  # for n
+00015f70: 6963 6572 2064 6573 6372 6970 7469 6f6e  icer description
+00015f80: 2c20 616e 6420 646f 6573 206e 6f74 206d  , and does not m
+00015f90: 6174 7465 720a 2020 2020 2020 2020 2020  atter.          
+00015fa0: 2020 656c 6966 206b 696e 6420 3d3d 2022    elif kind == "
+00015fb0: 7472 7565 6469 7622 3a0a 2020 2020 2020  truediv":.      
+00015fc0: 2020 2020 2020 2020 2020 6966 2061 2025            if a %
+00015fd0: 2062 2021 3d20 303a 0a20 2020 2020 2020   b != 0:.       
+00015fe0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00015ff0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00016000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016010: 2020 2020 2020 2022 2573 2074 7275 6564         "%s trued
+00016020: 6976 2025 7320 6f6e 6c79 2061 6c6c 6f77  iv %s only allow
+00016030: 6564 2069 6620 7468 6520 7265 7375 6c74  ed if the result
+00016040: 2069 7320 616e 2069 6e74 6567 6572 2220   is an integer" 
+00016050: 2520 286e 756d 6572 6174 6f72 2c20 6465  % (numerator, de
+00016060: 6e6f 6d69 6e61 746f 7229 0a20 2020 2020  nominator).     
+00016070: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00016080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016090: 2064 696d 5f76 616c 7565 203d 2061 202f   dim_value = a /
+000160a0: 2f20 620a 2020 2020 2020 2020 2020 2020  / b.            
+000160b0: 2020 2020 6966 2072 6967 6874 3a0a 2020      if right:.  
+000160c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160d0: 2020 6b69 6e64 203d 2022 666c 6f6f 7264    kind = "floord
+000160e0: 6976 2220 2023 2066 6f72 206e 6963 6572  iv"  # for nicer
+000160f0: 2064 6573 6372 6970 7469 6f6e 2c20 616e   description, an
+00016100: 6420 646f 6573 206e 6f74 206d 6174 7465  d does not matte
+00016110: 720a 2020 2020 2020 2020 2020 2020 656c  r.            el
+00016120: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00016130: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00016140: 7272 6f72 2822 696e 7661 6c69 6420 6b69  rror("invalid ki
+00016150: 6e64 2025 7222 2025 2028 6b69 6e64 2c29  nd %r" % (kind,)
+00016160: 290a 2020 2020 2020 2020 6966 206b 696e  ).        if kin
+00016170: 6420 3d3d 2022 666c 6f6f 7264 6976 2220  d == "floordiv" 
+00016180: 616e 6420 7269 6768 743a 0a20 2020 2020  and right:.     
+00016190: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+000161a0: 6f6e 203d 2022 2573 2f2f 2573 2220 2520  on = "%s//%s" % 
+000161b0: 285f 6765 745f 6465 7363 7269 7074 696f  (_get_descriptio
+000161c0: 6e28 6e75 6d65 7261 746f 7229 2c20 5f67  n(numerator), _g
+000161d0: 6574 5f64 6573 6372 6970 7469 6f6e 2864  et_description(d
+000161e0: 656e 6f6d 696e 6174 6f72 2929 0a20 2020  enominator)).   
+000161f0: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
+00016200: 3d20 2263 6569 6c64 6976 2220 616e 6420  = "ceildiv" and 
+00016210: 7269 6768 743a 0a20 2020 2020 2020 2020  right:.         
+00016220: 2020 2064 6573 6372 6970 7469 6f6e 203d     description =
+00016230: 2022 e28c 8825 732f 2573 e28c 8922 2025   "...%s/%s..." %
+00016240: 2028 5f67 6574 5f64 6573 6372 6970 7469   (_get_descripti
+00016250: 6f6e 286e 756d 6572 6174 6f72 292c 205f  on(numerator), _
+00016260: 6765 745f 6465 7363 7269 7074 696f 6e28  get_description(
+00016270: 6465 6e6f 6d69 6e61 746f 7229 290a 2020  denominator)).  
+00016280: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00016290: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+000162a0: 696f 6e20 3d20 2225 735f 2573 2825 732c  ion = "%s_%s(%s,
+000162b0: 2025 7329 2220 2520 280a 2020 2020 2020   %s)" % (.      
+000162c0: 2020 2020 2020 2020 2020 6b69 6e64 2c0a            kind,.
+000162d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162e0: 2272 6967 6874 2220 6966 2072 6967 6874  "right" if right
+000162f0: 2065 6c73 6520 226c 6566 7422 2c0a 2020   else "left",.  
+00016300: 2020 2020 2020 2020 2020 2020 2020 5f67                _g
+00016310: 6574 5f64 6573 6372 6970 7469 6f6e 286e  et_description(n
+00016320: 756d 6572 6174 6f72 2c20 6272 6163 6b65  umerator, bracke
+00016330: 7473 3d46 616c 7365 292c 0a20 2020 2020  ts=False),.     
+00016340: 2020 2020 2020 2020 2020 205f 6765 745f             _get_
+00016350: 6465 7363 7269 7074 696f 6e28 6465 6e6f  description(deno
+00016360: 6d69 6e61 746f 722c 2062 7261 636b 6574  minator, bracket
+00016370: 733d 4661 6c73 6529 2c0a 2020 2020 2020  s=False),.      
+00016380: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00016390: 6f70 5f6b 696e 6420 3d20 6b69 6e64 0a20  op_kind = kind. 
+000163a0: 2020 2020 2020 2069 6620 6120 6973 206e         if a is n
+000163b0: 6f74 204e 6f6e 6520 616e 6420 6220 6973  ot None and b is
+000163c0: 206e 6f74 204e 6f6e 6520 616e 6420 6120   not None and a 
+000163d0: 2520 6220 3d3d 2030 3a0a 2020 2020 2020  % b == 0:.      
+000163e0: 2020 2020 2020 6f70 5f6b 696e 6420 3d20        op_kind = 
+000163f0: 2274 7275 6564 6976 2220 2023 206d 616b  "truediv"  # mak
+00016400: 6573 2073 6f6d 6520 6f74 6865 7220 6368  es some other ch
+00016410: 6563 6b73 2073 696d 706c 6572 0a20 2020  ecks simpler.   
+00016420: 2020 2020 206f 705f 6b69 6e64 202b 3d20       op_kind += 
+00016430: 225f 2220 2b20 2822 7269 6768 7422 2069  "_" + ("right" i
+00016440: 6620 7269 6768 7420 656c 7365 2022 6c65  f right else "le
+00016450: 6674 2229 0a20 2020 2020 2020 2072 6574  ft").        ret
+00016460: 7572 6e20 5f64 2e44 696d 280a 2020 2020  urn _d.Dim(.    
+00016470: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00016480: 696f 6e3d 6465 7363 7269 7074 696f 6e2c  ion=description,
+00016490: 0a20 2020 2020 2020 2020 2020 206b 696e  .            kin
+000164a0: 643d 6e75 6d65 7261 746f 722e 6b69 6e64  d=numerator.kind
+000164b0: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+000164c0: 6d65 6e73 696f 6e3d 6469 6d5f 7661 6c75  mension=dim_valu
+000164d0: 652c 0a20 2020 2020 2020 2020 2020 2064  e,.            d
+000164e0: 6572 6976 6564 5f66 726f 6d5f 6f70 3d4f  erived_from_op=O
+000164f0: 7028 6b69 6e64 3d6f 705f 6b69 6e64 2c20  p(kind=op_kind, 
+00016500: 696e 7075 7473 3d5b 6e75 6d65 7261 746f  inputs=[numerato
+00016510: 722c 2064 656e 6f6d 696e 6174 6f72 5d29  r, denominator])
+00016520: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+00016530: 7269 7665 645f 6672 6f6d 5f74 6167 3d6e  rived_from_tag=n
+00016540: 756d 6572 6174 6f72 2c0a 2020 2020 2020  umerator,.      
+00016550: 2020 290a 0a20 2020 2064 6566 2061 735f    )..    def as_
+00016560: 6469 6d28 7365 6c66 293a 0a20 2020 2020  dim(self):.     
+00016570: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00016580: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
+00016590: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+000165a0: 6620 7365 6c66 2e69 735f 6f6e 6528 293a  f self.is_one():
+000165b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000165c0: 7572 6e20 5f6d 616b 655f 636f 6e73 7461  urn _make_consta
+000165d0: 6e74 5f73 7461 7469 635f 6469 6d28 3129  nt_static_dim(1)
+000165e0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+000165f0: 7365 6c66 2e74 6572 6d73 2920 3d3d 2031  self.terms) == 1
+00016600: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00016610: 7475 726e 2073 656c 662e 7465 726d 735b  turn self.terms[
+00016620: 305d 0a20 2020 2020 2020 2064 696d 5f6b  0].        dim_k
+00016630: 696e 6420 3d20 5f67 6574 5f6d 6572 6765  ind = _get_merge
+00016640: 645f 6469 6d5f 6b69 6e64 2873 656c 662e  d_dim_kind(self.
+00016650: 7465 726d 7329 0a20 2020 2020 2020 2072  terms).        r
+00016660: 6574 7572 6e20 5f64 2e44 696d 280a 2020  eturn _d.Dim(.  
+00016670: 2020 2020 2020 2020 2020 6b69 6e64 3d64            kind=d
+00016680: 696d 5f6b 696e 642c 0a20 2020 2020 2020  im_kind,.       
+00016690: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+000166a0: 3d22 2a22 2e6a 6f69 6e28 6d61 7028 5f67  ="*".join(map(_g
+000166b0: 6574 5f64 6573 6372 6970 7469 6f6e 2c20  et_description, 
+000166c0: 7365 6c66 2e74 6572 6d73 2929 2c0a 2020  self.terms)),.  
+000166d0: 2020 2020 2020 2020 2020 6469 6d65 6e73            dimens
+000166e0: 696f 6e3d 7365 6c66 2e64 696d 656e 7369  ion=self.dimensi
+000166f0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00016700: 6465 7269 7665 645f 6672 6f6d 5f6f 703d  derived_from_op=
+00016710: 4f70 286b 696e 643d 226d 756c 222c 2069  Op(kind="mul", i
+00016720: 6e70 7574 733d 6c69 7374 2873 656c 662e  nputs=list(self.
+00016730: 7465 726d 7329 292c 0a20 2020 2020 2020  terms)),.       
+00016740: 2020 2020 2064 6572 6976 6564 5f66 726f       derived_fro
+00016750: 6d5f 7461 673d 7365 6c66 2e72 6570 7265  m_tag=self.repre
+00016760: 7365 6e74 6174 6976 655f 7461 6728 292c  sentative_tag(),
+00016770: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00016780: 6465 6620 7265 7072 6573 656e 7461 7469  def representati
+00016790: 7665 5f74 6167 2873 656c 6629 3a0a 2020  ve_tag(self):.  
+000167a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000167b0: 2020 3a72 7479 7065 3a20 4469 6d7c 4e6f    :rtype: Dim|No
+000167c0: 6e65 0a20 2020 2020 2020 2022 2222 0a20  ne.        """. 
+000167d0: 2020 2020 2020 2023 2041 6c73 6f20 7365         # Also se
+000167e0: 6520 4469 6d2e 5f4f 704c 696e 6561 7254  e Dim._OpLinearT
+000167f0: 6572 6d2e 7265 7072 6573 656e 7461 7469  erm.representati
+00016800: 7665 5f74 6167 2829 2e0a 2020 2020 2020  ve_tag()..      
+00016810: 2020 2320 4669 7273 7420 6669 6e64 2061    # First find a
+00016820: 6e79 2064 796e 616d 6963 2e0a 2020 2020  ny dynamic..    
+00016830: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
+00016840: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
+00016850: 2020 2020 2020 2020 2069 6620 7465 726d           if term
+00016860: 5f2e 6973 5f64 796e 616d 6963 2829 3a0a  _.is_dynamic():.
+00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016880: 7265 7475 726e 2074 6572 6d5f 0a20 2020  return term_.   
+00016890: 2020 2020 2023 204e 6f77 2066 696e 6420       # Now find 
+000168a0: 6e6f 6e2d 756e 7370 6563 6966 6965 642e  non-unspecified.
+000168b0: 0a20 2020 2020 2020 2066 6f72 2074 6572  .        for ter
+000168c0: 6d5f 2069 6e20 7365 6c66 2e74 6572 6d73  m_ in self.terms
+000168d0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000168e0: 2074 6572 6d5f 2e6b 696e 6420 213d 2044   term_.kind != D
+000168f0: 696d 5479 7065 732e 556e 7370 6563 6966  imTypes.Unspecif
+00016900: 6965 643a 0a20 2020 2020 2020 2020 2020  ied:.           
+00016910: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
+00016920: 5f0a 2020 2020 2020 2020 2320 4e6f 7720  _.        # Now 
+00016930: 6669 6e64 2061 6e79 2e0a 2020 2020 2020  find any..      
+00016940: 2020 666f 7220 7465 726d 5f20 696e 2073    for term_ in s
+00016950: 656c 662e 7465 726d 733a 0a20 2020 2020  elf.terms:.     
+00016960: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
+00016970: 726d 5f0a 2020 2020 2020 2020 7265 7475  rm_.        retu
+00016980: 726e 204e 6f6e 650a 0a0a 636c 6173 7320  rn None...class 
+00016990: 5f4f 704c 696e 6561 7254 6572 6d3a 0a20  _OpLinearTerm:. 
+000169a0: 2020 2022 2222 0a20 2020 2072 6570 7265     """.    repre
+000169b0: 7365 6e74 7320 7374 6820 6c69 6b65 2061  sents sth like a
+000169c0: 202a 2062 202b 2063 0a20 2020 2022 2222   * b + c.    """
+000169d0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+000169e0: 6f64 0a20 2020 2064 6566 2066 726f 6d5f  od.    def from_
+000169f0: 6469 6d28 636c 732c 2064 696d 293a 0a20  dim(cls, dim):. 
+00016a00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016a10: 2020 203a 7061 7261 6d20 4469 6d20 6469     :param Dim di
+00016a20: 6d3a 0a20 2020 2020 2020 203a 7274 7970  m:.        :rtyp
+00016a30: 653a 2044 696d 2e5f 4f70 4c69 6e65 6172  e: Dim._OpLinear
+00016a40: 5465 726d 0a20 2020 2020 2020 2022 2222  Term.        """
+00016a50: 0a20 2020 2020 2020 2072 6573 203d 2063  .        res = c
+00016a60: 6c73 2e7a 6572 6f28 290a 2020 2020 2020  ls.zero().      
+00016a70: 2020 7265 732e 6578 7465 6e64 5f61 6464    res.extend_add
+00016a80: 5f73 7562 5f28 6469 6d2c 206b 696e 643d  _sub_(dim, kind=
+00016a90: 2261 6464 222c 2072 6967 6874 3d54 7275  "add", right=Tru
+00016aa0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+00016ab0: 6e20 7265 730a 0a20 2020 2040 636c 6173  n res..    @clas
+00016ac0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00016ad0: 7a65 726f 2863 6c73 293a 0a20 2020 2020  zero(cls):.     
+00016ae0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00016af0: 7274 7970 653a 2044 696d 2e5f 4f70 4c69  rtype: Dim._OpLi
+00016b00: 6e65 6172 5465 726d 0a20 2020 2020 2020  nearTerm.       
+00016b10: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00016b20: 7572 6e20 5f4f 704c 696e 6561 7254 6572  urn _OpLinearTer
+00016b30: 6d28 5b5d 290a 0a20 2020 2064 6566 205f  m([])..    def _
+00016b40: 5f69 6e69 745f 5f28 7365 6c66 2c20 7465  _init__(self, te
+00016b50: 726d 7329 3a0a 2020 2020 2020 2020 2222  rms):.        ""
+00016b60: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+00016b70: 206c 6973 745b 4469 6d2e 5f4f 704d 756c   list[Dim._OpMul
+00016b80: 7454 6572 6d5d 2074 6572 6d73 3a0a 2020  tTerm] terms:.  
+00016b90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00016ba0: 2020 7365 6c66 2e74 6572 6d73 203d 2074    self.terms = t
+00016bb0: 6572 6d73 0a0a 2020 2020 6465 6620 5f5f  erms..    def __
+00016bc0: 6861 7368 5f5f 2873 656c 6629 3a0a 2020  hash__(self):.  
+00016bd0: 2020 2020 2020 7265 7475 726e 2068 6173        return has
+00016be0: 6828 7475 706c 6528 7365 6c66 2e74 6572  h(tuple(self.ter
+00016bf0: 6d73 2929 0a0a 2020 2020 6465 6620 5f5f  ms))..    def __
+00016c00: 6571 5f5f 2873 656c 662c 206f 7468 6572  eq__(self, other
+00016c10: 293a 0a20 2020 2020 2020 2069 6620 6973  ):.        if is
+00016c20: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
+00016c30: 5f4f 704c 696e 6561 7254 6572 6d29 3a0a  _OpLinearTerm):.
+00016c40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00016c50: 726e 2073 656c 662e 7465 726d 7320 3d3d  rn self.terms ==
+00016c60: 206f 7468 6572 2e74 6572 6d73 0a20 2020   other.terms.   
+00016c70: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00016c80: 650a 0a20 2020 2064 6566 205f 5f6e 655f  e..    def __ne_
+00016c90: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+00016ca0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00016cb0: 6f74 2073 656c 662e 5f5f 6571 5f5f 286f  ot self.__eq__(o
+00016cc0: 7468 6572 290a 0a20 2020 2064 6566 2061  ther)..    def a
+00016cd0: 735f 6469 6d28 7365 6c66 293a 0a20 2020  s_dim(self):.   
+00016ce0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016cf0: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
+00016d00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016d10: 2069 6620 7365 6c66 2e69 735f 7a65 726f   if self.is_zero
+00016d20: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00016d30: 7265 7475 726e 205f 6d61 6b65 5f63 6f6e  return _make_con
+00016d40: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
+00016d50: 2830 290a 2020 2020 2020 2020 6966 206c  (0).        if l
+00016d60: 656e 2873 656c 662e 7465 726d 7329 203d  en(self.terms) =
+00016d70: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
+00016d80: 2072 6574 7572 6e20 7365 6c66 2e74 6572   return self.ter
+00016d90: 6d73 5b30 5d2e 6173 5f64 696d 2829 0a20  ms[0].as_dim(). 
+00016da0: 2020 2020 2020 2061 6464 5f70 6172 7473         add_parts
+00016db0: 203d 205b 5d0a 2020 2020 2020 2020 6465   = [].        de
+00016dc0: 7363 5f70 6172 7473 203d 205b 5d0a 2020  sc_parts = [].  
+00016dd0: 2020 2020 2020 6469 6d20 3d20 300a 2020        dim = 0.  
+00016de0: 2020 2020 2020 666f 7220 7465 726d 2069        for term i
+00016df0: 6e20 7365 6c66 2e74 6572 6d73 3a0a 2020  n self.terms:.  
+00016e00: 2020 2020 2020 2020 2020 7320 3d20 7465            s = te
+00016e10: 726d 2e61 735f 6469 6d28 290a 2020 2020  rm.as_dim().    
+00016e20: 2020 2020 2020 2020 6164 645f 7061 7274          add_part
+00016e30: 732e 6170 7065 6e64 2873 290a 2020 2020  s.append(s).    
+00016e40: 2020 2020 2020 2020 6465 7363 5f70 6172          desc_par
+00016e50: 7473 2e61 7070 656e 6428 5f67 6574 5f64  ts.append(_get_d
+00016e60: 6573 6372 6970 7469 6f6e 2873 2929 0a20  escription(s)). 
+00016e70: 2020 2020 2020 2020 2020 2069 6620 6469             if di
+00016e80: 6d20 6973 206e 6f74 204e 6f6e 6520 616e  m is not None an
+00016e90: 6420 732e 6469 6d65 6e73 696f 6e20 6973  d s.dimension is
+00016ea0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00016eb0: 2020 2020 2020 2020 2020 2064 696d 202b             dim +
+00016ec0: 3d20 732e 6469 6d65 6e73 696f 6e0a 2020  = s.dimension.  
+00016ed0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00016ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ef0: 6469 6d20 3d20 4e6f 6e65 0a20 2020 2020  dim = None.     
+00016f00: 2020 2069 6620 6c65 6e28 6164 645f 7061     if len(add_pa
+00016f10: 7274 7329 203d 3d20 313a 0a20 2020 2020  rts) == 1:.     
+00016f20: 2020 2020 2020 2072 6574 7572 6e20 6164         return ad
+00016f30: 645f 7061 7274 735b 305d 0a20 2020 2020  d_parts[0].     
+00016f40: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
+00016f50: 280a 2020 2020 2020 2020 2020 2020 6b69  (.            ki
+00016f60: 6e64 3d5f 6765 745f 6d65 7267 6564 5f64  nd=_get_merged_d
+00016f70: 696d 5f6b 696e 6428 6164 645f 7061 7274  im_kind(add_part
+00016f80: 7329 2c0a 2020 2020 2020 2020 2020 2020  s),.            
+00016f90: 6465 7363 7269 7074 696f 6e3d 222b 222e  description="+".
+00016fa0: 6a6f 696e 2864 6573 635f 7061 7274 7329  join(desc_parts)
+00016fb0: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+00016fc0: 6d65 6e73 696f 6e3d 6469 6d2c 0a20 2020  mension=dim,.   
+00016fd0: 2020 2020 2020 2020 2064 6572 6976 6564           derived
+00016fe0: 5f66 726f 6d5f 6f70 3d4f 7028 6b69 6e64  _from_op=Op(kind
+00016ff0: 3d22 6164 6422 2c20 696e 7075 7473 3d61  ="add", inputs=a
+00017000: 6464 5f70 6172 7473 292c 0a20 2020 2020  dd_parts),.     
+00017010: 2020 2020 2020 2064 6572 6976 6564 5f66         derived_f
+00017020: 726f 6d5f 7461 673d 7365 6c66 2e72 6570  rom_tag=self.rep
+00017030: 7265 7365 6e74 6174 6976 655f 7461 6728  resentative_tag(
+00017040: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00017050: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
+00017060: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00017070: 7475 726e 2022 4469 6d2e 5f4f 704c 696e  turn "Dim._OpLin
+00017080: 6561 7254 6572 6d28 2572 2922 2025 2028  earTerm(%r)" % (
+00017090: 7365 6c66 2e74 6572 6d73 2c29 0a0a 2020  self.terms,)..  
+000170a0: 2020 6465 6620 6973 5f7a 6572 6f28 7365    def is_zero(se
+000170b0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000170c0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000170d0: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
+000170e0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+000170f0: 206e 6f74 2073 656c 662e 7465 726d 730a   not self.terms.
+00017100: 0a20 2020 2064 6566 2065 7874 656e 645f  .    def extend_
+00017110: 6164 645f 7375 625f 2873 656c 662c 206f  add_sub_(self, o
+00017120: 7468 6572 2c20 6b69 6e64 2c20 7269 6768  ther, kind, righ
+00017130: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
+00017140: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
+00017150: 696d 7c69 6e74 206f 7468 6572 3a0a 2020  im|int other:.  
+00017160: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
+00017170: 206b 696e 643a 2022 6164 6422 206f 7220   kind: "add" or 
+00017180: 2273 7562 220a 2020 2020 2020 2020 3a70  "sub".        :p
+00017190: 6172 616d 2062 6f6f 6c20 7269 6768 743a  aram bool right:
+000171a0: 206f 7220 6c65 6674 2e20 7269 6768 7420   or left. right 
+000171b0: 6d65 616e 7320 7365 6c66 202b 206f 7468  means self + oth
+000171c0: 6572 2c20 6c65 6674 206d 6561 6e73 206f  er, left means o
+000171d0: 7468 6572 202b 2073 656c 660a 2020 2020  ther + self.    
+000171e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000171f0: 6173 7365 7274 206b 696e 6420 696e 207b  assert kind in {
+00017200: 2261 6464 222c 2022 7375 6222 7d0a 2020  "add", "sub"}.  
+00017210: 2020 2020 2020 6f74 6865 7220 3d20 7365        other = se
+00017220: 6c66 2e5f 6d61 6b65 5f64 696d 286f 7468  lf._make_dim(oth
+00017230: 6572 2c20 6b69 6e64 3d6b 696e 6429 0a20  er, kind=kind). 
+00017240: 2020 2020 2020 2069 6620 6f74 6865 722e         if other.
+00017250: 6973 5f63 6f6e 7374 616e 745f 7374 6174  is_constant_stat
+00017260: 6963 5f64 696d 2829 2061 6e64 206f 7468  ic_dim() and oth
+00017270: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
+00017280: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00017290: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+000172a0: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
+000172b0: 726f 6d5f 6f70 2061 6e64 206f 7468 6572  rom_op and other
+000172c0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+000172d0: 2e6b 696e 6420 3d3d 2022 6164 6422 3a0a  .kind == "add":.
+000172e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000172f0: 6f74 6865 725f 2069 6e20 6f74 6865 722e  other_ in other.
+00017300: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00017310: 696e 7075 7473 2069 6620 7269 6768 7420  inputs if right 
+00017320: 656c 7365 2072 6576 6572 7365 6428 6f74  else reversed(ot
+00017330: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
+00017340: 5f6f 702e 696e 7075 7473 293a 0a20 2020  _op.inputs):.   
+00017350: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017360: 662e 6578 7465 6e64 5f61 6464 5f73 7562  f.extend_add_sub
+00017370: 5f28 6f74 6865 725f 2c20 6b69 6e64 3d6b  _(other_, kind=k
+00017380: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
+00017390: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000173a0: 7475 726e 0a20 2020 2020 2020 2074 6572  turn.        ter
+000173b0: 6d20 3d20 5f4f 704d 756c 7454 6572 6d2e  m = _OpMultTerm.
+000173c0: 6672 6f6d 5f64 696d 286f 7468 6572 290a  from_dim(other).
+000173d0: 2020 2020 2020 2020 6e65 675f 7465 726d          neg_term
+000173e0: 203d 2074 6572 6d2e 6e65 6761 7469 7665   = term.negative
+000173f0: 2829 0a20 2020 2020 2020 2069 6620 6b69  ().        if ki
+00017400: 6e64 203d 3d20 2273 7562 223a 0a20 2020  nd == "sub":.   
+00017410: 2020 2020 2020 2020 2074 6572 6d2c 206e           term, n
+00017420: 6567 5f74 6572 6d20 3d20 6e65 675f 7465  eg_term = neg_te
+00017430: 726d 2c20 7465 726d 0a20 2020 2020 2020  rm, term.       
+00017440: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
+00017450: 6d20 3d20 7365 6c66 2e74 6572 6d73 5b2d  m = self.terms[-
+00017460: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
+00017470: 305d 2069 6620 7365 6c66 2e74 6572 6d73  0] if self.terms
+00017480: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+00017490: 2020 2069 6620 6d6f 7374 5f72 6563 656e     if most_recen
+000174a0: 745f 7465 726d 3a0a 2020 2020 2020 2020  t_term:.        
+000174b0: 2020 2020 6966 206d 6f73 745f 7265 6365      if most_rece
+000174c0: 6e74 5f74 6572 6d20 3d3d 206e 6567 5f74  nt_term == neg_t
+000174d0: 6572 6d3a 0a20 2020 2020 2020 2020 2020  erm:.           
+000174e0: 2020 2020 2073 656c 662e 7465 726d 732e       self.terms.
+000174f0: 706f 7028 2d31 2069 6620 7269 6768 7420  pop(-1 if right 
+00017500: 656c 7365 2030 290a 2020 2020 2020 2020  else 0).        
+00017510: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00017520: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+00017530: 7374 5f72 6563 656e 745f 7465 726d 2e69  st_recent_term.i
+00017540: 735f 636f 6e73 7461 6e74 5f73 7461 7469  s_constant_stati
+00017550: 635f 6469 6d28 2920 616e 6420 7465 726d  c_dim() and term
+00017560: 2e69 735f 636f 6e73 7461 6e74 5f73 7461  .is_constant_sta
+00017570: 7469 635f 6469 6d28 293a 0a20 2020 2020  tic_dim():.     
+00017580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017590: 7465 726d 735b 2d31 2069 6620 7269 6768  terms[-1 if righ
+000175a0: 7420 656c 7365 2030 5d20 3d20 5f4f 704d  t else 0] = _OpM
+000175b0: 756c 7454 6572 6d2e 6672 6f6d 5f64 696d  ultTerm.from_dim
+000175c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000175d0: 2020 2020 2020 5f6d 616b 655f 636f 6e73        _make_cons
+000175e0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
+000175f0: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
+00017600: 2e64 696d 656e 7369 6f6e 202b 2074 6572  .dimension + ter
+00017610: 6d2e 6469 6d65 6e73 696f 6e2c 206b 696e  m.dimension, kin
+00017620: 643d 6f74 6865 722e 6b69 6e64 290a 2020  d=other.kind).  
+00017630: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017650: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00017660: 2020 2069 6620 6d6f 7374 5f72 6563 656e     if most_recen
+00017670: 745f 7465 726d 2e74 6572 6d73 2061 6e64  t_term.terms and
+00017680: 2074 6572 6d2e 7465 726d 7320 616e 6420   term.terms and 
+00017690: 6d6f 7374 5f72 6563 656e 745f 7465 726d  most_recent_term
+000176a0: 2e74 6572 6d73 5b2d 315d 203d 3d20 7465  .terms[-1] == te
+000176b0: 726d 2e74 6572 6d73 5b2d 315d 3a0a 2020  rm.terms[-1]:.  
+000176c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000176d0: 4d65 7267 6520 7465 726d 730a 2020 2020  Merge terms.    
+000176e0: 2020 2020 2020 2020 2020 2020 6120 3d20              a = 
+000176f0: 5f4f 704d 756c 7454 6572 6d2e 6672 6f6d  _OpMultTerm.from
+00017700: 5f64 696d 5f66 6163 746f 7273 286d 6f73  _dim_factors(mos
+00017710: 745f 7265 6365 6e74 5f74 6572 6d2e 7465  t_recent_term.te
+00017720: 726d 735b 3a2d 315d 292e 6173 5f64 696d  rms[:-1]).as_dim
+00017730: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00017740: 2020 2062 203d 205f 4f70 4d75 6c74 5465     b = _OpMultTe
+00017750: 726d 2e66 726f 6d5f 6469 6d5f 6661 6374  rm.from_dim_fact
+00017760: 6f72 7328 7465 726d 2e74 6572 6d73 5b3a  ors(term.terms[:
+00017770: 2d31 5d29 2e61 735f 6469 6d28 290a 2020  -1]).as_dim().  
+00017780: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00017790: 7320 3d20 5f4f 704d 756c 7454 6572 6d2e  s = _OpMultTerm.
+000177a0: 6672 6f6d 5f64 696d 2828 6120 2b20 6229  from_dim((a + b)
+000177b0: 2069 6620 7269 6768 7420 656c 7365 2028   if right else (
+000177c0: 6220 2b20 6129 290a 2020 2020 2020 2020  b + a)).        
+000177d0: 2020 2020 2020 2020 7265 732e 6578 7465          res.exte
+000177e0: 6e64 5f6d 756c 5f64 6976 5f28 7465 726d  nd_mul_div_(term
+000177f0: 2e74 6572 6d73 5b2d 315d 2c20 6b69 6e64  .terms[-1], kind
+00017800: 3d22 6d75 6c22 2c20 7269 6768 743d 5472  ="mul", right=Tr
+00017810: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00017820: 2020 2020 7365 6c66 2e74 6572 6d73 5b2d      self.terms[-
+00017830: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
+00017840: 305d 203d 2072 6573 0a20 2020 2020 2020  0] = res.       
+00017850: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00017860: 2020 2020 2020 2020 6966 2072 6967 6874          if right
+00017870: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00017880: 6c66 2e74 6572 6d73 2e61 7070 656e 6428  lf.terms.append(
+00017890: 7465 726d 290a 2020 2020 2020 2020 656c  term).        el
+000178a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000178b0: 7365 6c66 2e74 6572 6d73 2e69 6e73 6572  self.terms.inser
+000178c0: 7428 302c 2074 6572 6d29 0a0a 2020 2020  t(0, term)..    
+000178d0: 6465 6620 6578 7465 6e64 5f6d 756c 5f64  def extend_mul_d
+000178e0: 6976 5f28 7365 6c66 2c20 6f74 6865 722c  iv_(self, other,
+000178f0: 206b 696e 642c 2072 6967 6874 293a 0a20   kind, right):. 
+00017900: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00017910: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
+00017920: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
+00017930: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
+00017940: 3a20 226d 756c 2220 6f72 2022 6365 696c  : "mul" or "ceil
+00017950: 6469 7622 0a20 2020 2020 2020 203a 7061  div".        :pa
+00017960: 7261 6d20 626f 6f6c 2072 6967 6874 3a20  ram bool right: 
+00017970: 6f72 206c 6566 742e 2072 6967 6874 206d  or left. right m
+00017980: 6561 6e73 2073 656c 6620 2a20 6f74 6865  eans self * othe
+00017990: 722c 206c 6566 7420 6d65 616e 7320 6f74  r, left means ot
+000179a0: 6865 7220 2a20 7365 6c66 0a20 2020 2020  her * self.     
+000179b0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+000179c0: 7373 6572 7420 6b69 6e64 2069 6e20 7b22  ssert kind in {"
+000179d0: 6d75 6c22 2c20 2266 6c6f 6f72 6469 7622  mul", "floordiv"
+000179e0: 2c20 2274 7275 6564 6976 222c 2022 6365  , "truediv", "ce
+000179f0: 696c 6469 7622 7d0a 2020 2020 2020 2020  ildiv"}.        
+00017a00: 6f74 6865 7220 3d20 7365 6c66 2e5f 6d61  other = self._ma
+00017a10: 6b65 5f64 696d 286f 7468 6572 2c20 6b69  ke_dim(other, ki
+00017a20: 6e64 3d6b 696e 6429 0a20 2020 2020 2020  nd=kind).       
+00017a30: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
+00017a40: 2220 616e 6420 7269 6768 743a 0a20 2020  " and right:.   
+00017a50: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00017a60: 616c 6c28 7465 726d 2e63 616e 5f73 696d  all(term.can_sim
+00017a70: 706c 6966 7928 6f74 6865 722c 206b 696e  plify(other, kin
+00017a80: 643d 6b69 6e64 2c20 7269 6768 743d 7269  d=kind, right=ri
+00017a90: 6768 7429 2066 6f72 2074 6572 6d20 696e  ght) for term in
+00017aa0: 2073 656c 662e 7465 726d 7329 3a0a 2020   self.terms):.  
+00017ab0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00017ac0: 446f 2069 7420 7468 6520 6f74 6865 7220  Do it the other 
+00017ad0: 7761 7920 6172 6f75 6e64 0a20 2020 2020  way around.     
+00017ae0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017af0: 7465 726d 732c 206f 7468 6572 203d 205f  terms, other = _
+00017b00: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
+00017b10: 6d5f 6469 6d28 6f74 6865 7229 2e74 6572  m_dim(other).ter
+00017b20: 6d73 2c20 7365 6c66 2e61 735f 6469 6d28  ms, self.as_dim(
+00017b30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017b40: 2020 7269 6768 7420 3d20 4661 6c73 650a    right = False.
+00017b50: 2020 2020 2020 2020 6966 206f 7468 6572          if other
+00017b60: 2e69 735f 636f 6e73 7461 6e74 5f73 7461  .is_constant_sta
+00017b70: 7469 635f 6469 6d28 2920 616e 6420 6f74  tic_dim() and ot
+00017b80: 6865 722e 6469 6d65 6e73 696f 6e20 3d3d  her.dimension ==
+00017b90: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00017ba0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+00017bb0: 6620 6b69 6e64 2e65 6e64 7377 6974 6828  f kind.endswith(
+00017bc0: 2264 6976 2229 2061 6e64 206c 656e 2873  "div") and len(s
+00017bd0: 656c 662e 7465 726d 7329 203e 3d20 323a  elf.terms) >= 2:
+00017be0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017bf0: 616e 7928 6e6f 7420 7465 726d 2e64 6976  any(not term.div
+00017c00: 6973 6962 6c65 286f 7468 6572 2c20 7269  isible(other, ri
+00017c10: 6768 743d 7269 6768 7429 2066 6f72 2074  ght=right) for t
+00017c20: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
+00017c30: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00017c40: 2020 2020 7365 6c66 2e74 6572 6d73 203d      self.terms =
+00017c50: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00017c60: 2020 2020 2020 205f 4f70 4d75 6c74 5465         _OpMultTe
+00017c70: 726d 2e66 726f 6d5f 6469 6d28 5f4f 704d  rm.from_dim(_OpM
+00017c80: 756c 7454 6572 6d2e 6e65 775f 6469 765f  ultTerm.new_div_
+00017c90: 6469 6d28 7365 6c66 2e61 735f 6469 6d28  dim(self.as_dim(
+00017ca0: 292c 206f 7468 6572 2c20 6b69 6e64 3d6b  ), other, kind=k
 00017cb0: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
-00017cc0: 290a 0a20 2020 2064 6566 205f 6d61 6b65  )..    def _make
-00017cd0: 5f64 696d 2873 656c 662c 206f 7468 6572  _dim(self, other
-00017ce0: 2c20 6b69 6e64 293a 0a20 2020 2020 2020  , kind):.       
-00017cf0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00017d00: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-00017d10: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
-00017d20: 6d20 7374 7220 6b69 6e64 3a0a 2020 2020  m str kind:.    
-00017d30: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-00017d40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00017d50: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00017d60: 6528 6f74 6865 722c 2069 6e74 293a 0a20  e(other, int):. 
-00017d70: 2020 2020 2020 2020 2020 2062 6173 655f             base_
-00017d80: 7461 6720 3d20 7365 6c66 2e72 6570 7265  tag = self.repre
-00017d90: 7365 6e74 6174 6976 655f 7461 6728 290a  sentative_tag().
-00017da0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00017db0: 726e 205f 6d61 6b65 5f63 6f6e 7374 616e  rn _make_constan
-00017dc0: 745f 7374 6174 6963 5f64 696d 286f 7468  t_static_dim(oth
-00017dd0: 6572 2c20 6b69 6e64 3d62 6173 655f 7461  er, kind=base_ta
-00017de0: 672e 6b69 6e64 2069 6620 6261 7365 5f74  g.kind if base_t
-00017df0: 6167 2065 6c73 6520 4e6f 6e65 290a 2020  ag else None).  
-00017e00: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00017e10: 7461 6e63 6528 6f74 6865 722c 205f 642e  tance(other, _d.
-00017e20: 4469 6d29 3a0a 2020 2020 2020 2020 2020  Dim):.          
-00017e30: 2020 7265 7475 726e 206f 7468 6572 2e67    return other.g
-00017e40: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
-00017e50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00017e60: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00017e70: 7970 6545 7272 6f72 2822 2573 2025 7320  ypeError("%s %s 
-00017e80: 2573 2069 6e76 616c 6964 2066 6f72 2074  %s invalid for t
-00017e90: 7970 6520 2573 2220 2520 2873 656c 662c  ype %s" % (self,
-00017ea0: 206b 696e 642c 206f 7468 6572 2c20 7479   kind, other, ty
-00017eb0: 7065 286f 7468 6572 2929 290a 0a20 2020  pe(other)))..   
-00017ec0: 2064 6566 2072 6570 7265 7365 6e74 6174   def representat
-00017ed0: 6976 655f 7461 6728 7365 6c66 293a 0a20  ive_tag(self):. 
-00017ee0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00017ef0: 2020 203a 7274 7970 653a 2044 696d 7c4e     :rtype: Dim|N
-00017f00: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
-00017f10: 2020 2020 2020 2020 2320 4669 7273 7420          # First 
-00017f20: 6669 6e64 2061 6e79 2064 796e 616d 6963  find any dynamic
-00017f30: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
-00017f40: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
-00017f50: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-00017f60: 7220 7465 726d 5f20 696e 2074 6572 6d2e  r term_ in term.
-00017f70: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
-00017f80: 2020 2020 2020 2069 6620 7465 726d 5f2e         if term_.
-00017f90: 6973 5f64 796e 616d 6963 2829 3a0a 2020  is_dynamic():.  
-00017fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fb0: 2020 7265 7475 726e 2074 6572 6d5f 0a20    return term_. 
-00017fc0: 2020 2020 2020 2023 204e 6f77 2066 696e         # Now fin
-00017fd0: 6420 6e6f 6e2d 756e 7370 6563 6966 6965  d non-unspecifie
-00017fe0: 642e 0a20 2020 2020 2020 2066 6f72 2074  d..        for t
-00017ff0: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
-00018000: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00018010: 6f72 2074 6572 6d5f 2069 6e20 7465 726d  or term_ in term
-00018020: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00018030: 2020 2020 2020 2020 6966 2074 6572 6d5f          if term_
-00018040: 2e6b 696e 6420 213d 2044 696d 5479 7065  .kind != DimType
-00018050: 732e 556e 7370 6563 6966 6965 643a 0a20  s.Unspecified:. 
-00018060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018070: 2020 2072 6574 7572 6e20 7465 726d 5f0a     return term_.
-00018080: 2020 2020 2020 2020 2320 4e6f 7720 6669          # Now fi
-00018090: 6e64 2061 6e79 2e0a 2020 2020 2020 2020  nd any..        
-000180a0: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
-000180b0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-000180c0: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
-000180d0: 2074 6572 6d2e 7465 726d 733a 0a20 2020   term.terms:.   
-000180e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000180f0: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
-00018100: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
-00018110: 6465 6620 5f67 6574 5f6d 6572 6765 645f  def _get_merged_
-00018120: 6469 6d5f 6b69 6e64 2864 696d 5f74 6167  dim_kind(dim_tag
-00018130: 7329 3a0a 2020 2020 2222 220a 2020 2020  s):.    """.    
-00018140: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
-00018150: 7c74 7570 6c65 5b44 696d 5d20 6469 6d5f  |tuple[Dim] dim_
-00018160: 7461 6773 3a0a 2020 2020 3a72 6574 7572  tags:.    :retur
-00018170: 6e3a 2064 696d 206b 696e 640a 2020 2020  n: dim kind.    
-00018180: 3a72 7479 7065 3a20 456e 7469 7479 0a20  :rtype: Entity. 
-00018190: 2020 2022 2222 0a20 2020 2069 6620 616e     """.    if an
-000181a0: 7928 7461 672e 6973 5f62 6174 6368 5f64  y(tag.is_batch_d
-000181b0: 696d 2829 2066 6f72 2074 6167 2069 6e20  im() for tag in 
-000181c0: 6469 6d5f 7461 6773 293a 0a20 2020 2020  dim_tags):.     
-000181d0: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
-000181e0: 6573 2e42 6174 6368 0a20 2020 2065 6c69  es.Batch.    eli
-000181f0: 6620 616e 7928 7461 672e 6973 5f66 6561  f any(tag.is_fea
-00018200: 7475 7265 5f64 696d 2829 2066 6f72 2074  ture_dim() for t
-00018210: 6167 2069 6e20 6469 6d5f 7461 6773 293a  ag in dim_tags):
-00018220: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00018230: 4469 6d54 7970 6573 2e46 6561 7475 7265  DimTypes.Feature
-00018240: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00018250: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
-00018260: 6573 2e53 7061 7469 616c 0a0a 0a64 6566  es.Spatial...def
-00018270: 2064 696d 5f63 6d70 5f76 616c 7565 286f   dim_cmp_value(o
-00018280: 626a 293a 0a20 2020 2022 2222 0a20 2020  bj):.    """.   
-00018290: 203a 7061 7261 6d20 4469 6d7c 5f4d 6172   :param Dim|_Mar
-000182a0: 6b65 6444 696d 206f 626a 3a0a 2020 2020  kedDim obj:.    
-000182b0: 3a72 6574 7572 6e3a 2061 6e79 7468 696e  :return: anythin
-000182c0: 6720 7768 6963 6820 6361 6e20 6265 2063  g which can be c
-000182d0: 6f6d 7061 7265 640a 2020 2020 2222 220a  ompared.    """.
-000182e0: 2020 2020 2320 4d61 6b65 2044 696d 2061      # Make Dim a
-000182f0: 6e64 205f 4d61 726b 6564 4469 6d20 636f  nd _MarkedDim co
-00018300: 6d70 6172 6162 6c65 2074 6f20 6561 6368  mparable to each
-00018310: 206f 7468 6572 2e0a 2020 2020 2320 4e6f   other..    # No
-00018320: 7465 2074 6861 7420 7468 6520 6f72 6465  te that the orde
-00018330: 7220 6973 2072 6561 6c6c 7920 6172 6269  r is really arbi
-00018340: 7472 6172 7920 616e 6420 646f 6573 206e  trary and does n
-00018350: 6f74 206d 6174 7465 722e 0a20 2020 2069  ot matter..    i
-00018360: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
-00018370: 2c20 5f64 2e44 696d 293a 0a20 2020 2020  , _d.Dim):.     
-00018380: 2020 206f 626a 203d 206f 626a 2e67 6574     obj = obj.get
-00018390: 5f73 616d 655f 6261 7365 2829 0a20 2020  _same_base().   
-000183a0: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
-000183b0: 2020 2020 2020 2020 2020 2222 2c0a 2020            "",.  
-000183c0: 2020 2020 2020 2020 2020 6f62 6a2e 6465            obj.de
-000183d0: 7363 7269 7074 696f 6e2c 0a20 2020 2020  scription,.     
-000183e0: 2020 2020 2020 206f 626a 2e6b 696e 642c         obj.kind,
-000183f0: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
-00018400: 2e64 696d 656e 7369 6f6e 2c0a 2020 2020  .dimension,.    
-00018410: 2020 2020 2020 2020 6f62 6a2e 6479 6e5f          obj.dyn_
-00018420: 7369 7a65 5f65 7874 2e64 696d 7320 6966  size_ext.dims if
-00018430: 206f 626a 2e64 796e 5f73 697a 655f 6578   obj.dyn_size_ex
-00018440: 7420 6973 206e 6f74 204e 6f6e 6520 656c  t is not None el
-00018450: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
-00018460: 2029 0a20 2020 2069 6620 6973 696e 7374   ).    if isinst
-00018470: 616e 6365 286f 626a 2c20 5f6d 2e4d 6172  ance(obj, _m.Mar
-00018480: 6b65 6444 696d 293a 0a20 2020 2020 2020  kedDim):.       
-00018490: 2072 6574 7572 6e20 6f62 6a2e 5f5f 636c   return obj.__cl
-000184a0: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20  ass__.__name__, 
-000184b0: 6f62 6a2e 7461 670a 2020 2020 7265 7475  obj.tag.    retu
-000184c0: 726e 206f 626a 0a                        rn obj.
+00017cc0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00017cd0: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00017ce0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00017cf0: 2020 2020 666f 7220 7465 726d 2069 6e20      for term in 
+00017d00: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
+00017d10: 2020 2020 2020 2020 7465 726d 2e65 7874          term.ext
+00017d20: 656e 645f 6d75 6c5f 6469 765f 286f 7468  end_mul_div_(oth
+00017d30: 6572 2c20 6b69 6e64 3d6b 696e 642c 2072  er, kind=kind, r
+00017d40: 6967 6874 3d72 6967 6874 290a 0a20 2020  ight=right)..   
+00017d50: 2064 6566 205f 6d61 6b65 5f64 696d 2873   def _make_dim(s
+00017d60: 656c 662c 206f 7468 6572 2c20 6b69 6e64  elf, other, kind
+00017d70: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00017d80: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+00017d90: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
+00017da0: 2020 2020 203a 7061 7261 6d20 7374 7220       :param str 
+00017db0: 6b69 6e64 3a0a 2020 2020 2020 2020 3a72  kind:.        :r
+00017dc0: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
+00017dd0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00017de0: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+00017df0: 722c 2069 6e74 293a 0a20 2020 2020 2020  r, int):.       
+00017e00: 2020 2020 2062 6173 655f 7461 6720 3d20       base_tag = 
+00017e10: 7365 6c66 2e72 6570 7265 7365 6e74 6174  self.representat
+00017e20: 6976 655f 7461 6728 290a 2020 2020 2020  ive_tag().      
+00017e30: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00017e40: 6b65 5f63 6f6e 7374 616e 745f 7374 6174  ke_constant_stat
+00017e50: 6963 5f64 696d 286f 7468 6572 2c20 6b69  ic_dim(other, ki
+00017e60: 6e64 3d62 6173 655f 7461 672e 6b69 6e64  nd=base_tag.kind
+00017e70: 2069 6620 6261 7365 5f74 6167 2065 6c73   if base_tag els
+00017e80: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
+00017e90: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00017ea0: 6f74 6865 722c 205f 642e 4469 6d29 3a0a  other, _d.Dim):.
+00017eb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017ec0: 726e 206f 7468 6572 2e67 6574 5f73 616d  rn other.get_sam
+00017ed0: 655f 6261 7365 2829 0a20 2020 2020 2020  e_base().       
+00017ee0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00017ef0: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00017f00: 6f72 2822 2573 2025 7320 2573 2069 6e76  or("%s %s %s inv
+00017f10: 616c 6964 2066 6f72 2074 7970 6520 2573  alid for type %s
+00017f20: 2220 2520 2873 656c 662c 206b 696e 642c  " % (self, kind,
+00017f30: 206f 7468 6572 2c20 7479 7065 286f 7468   other, type(oth
+00017f40: 6572 2929 290a 0a20 2020 2064 6566 2072  er)))..    def r
+00017f50: 6570 7265 7365 6e74 6174 6976 655f 7461  epresentative_ta
+00017f60: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+00017f70: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+00017f80: 7970 653a 2044 696d 7c4e 6f6e 650a 2020  ype: Dim|None.  
+00017f90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00017fa0: 2020 2320 4669 7273 7420 6669 6e64 2061    # First find a
+00017fb0: 6e79 2064 796e 616d 6963 2e0a 2020 2020  ny dynamic..    
+00017fc0: 2020 2020 666f 7220 7465 726d 2069 6e20      for term in 
+00017fd0: 7365 6c66 2e74 6572 6d73 3a0a 2020 2020  self.terms:.    
+00017fe0: 2020 2020 2020 2020 666f 7220 7465 726d          for term
+00017ff0: 5f20 696e 2074 6572 6d2e 7465 726d 733a  _ in term.terms:
+00018000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018010: 2069 6620 7465 726d 5f2e 6973 5f64 796e   if term_.is_dyn
+00018020: 616d 6963 2829 3a0a 2020 2020 2020 2020  amic():.        
+00018030: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00018040: 726e 2074 6572 6d5f 0a20 2020 2020 2020  rn term_.       
+00018050: 2023 204e 6f77 2066 696e 6420 6e6f 6e2d   # Now find non-
+00018060: 756e 7370 6563 6966 6965 642e 0a20 2020  unspecified..   
+00018070: 2020 2020 2066 6f72 2074 6572 6d20 696e       for term in
+00018080: 2073 656c 662e 7465 726d 733a 0a20 2020   self.terms:.   
+00018090: 2020 2020 2020 2020 2066 6f72 2074 6572           for ter
+000180a0: 6d5f 2069 6e20 7465 726d 2e74 6572 6d73  m_ in term.terms
+000180b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000180c0: 2020 6966 2074 6572 6d5f 2e6b 696e 6420    if term_.kind 
+000180d0: 213d 2044 696d 5479 7065 732e 556e 7370  != DimTypes.Unsp
+000180e0: 6563 6966 6965 643a 0a20 2020 2020 2020  ecified:.       
+000180f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00018100: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
+00018110: 2020 2320 4e6f 7720 6669 6e64 2061 6e79    # Now find any
+00018120: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
+00018130: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
+00018140: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00018150: 7220 7465 726d 5f20 696e 2074 6572 6d2e  r term_ in term.
+00018160: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
+00018170: 2020 2020 2020 2072 6574 7572 6e20 7465         return te
+00018180: 726d 5f0a 2020 2020 2020 2020 7265 7475  rm_.        retu
+00018190: 726e 204e 6f6e 650a 0a0a 6465 6620 5f67  rn None...def _g
+000181a0: 6574 5f6d 6572 6765 645f 6469 6d5f 6b69  et_merged_dim_ki
+000181b0: 6e64 2864 696d 5f74 6167 7329 3a0a 2020  nd(dim_tags):.  
+000181c0: 2020 2222 220a 2020 2020 3a70 6172 616d    """.    :param
+000181d0: 206c 6973 745b 4469 6d5d 7c74 7570 6c65   list[Dim]|tuple
+000181e0: 5b44 696d 5d20 6469 6d5f 7461 6773 3a0a  [Dim] dim_tags:.
+000181f0: 2020 2020 3a72 6574 7572 6e3a 2064 696d      :return: dim
+00018200: 206b 696e 640a 2020 2020 3a72 7479 7065   kind.    :rtype
+00018210: 3a20 456e 7469 7479 0a20 2020 2022 2222  : Entity.    """
+00018220: 0a20 2020 2069 6620 616e 7928 7461 672e  .    if any(tag.
+00018230: 6973 5f62 6174 6368 5f64 696d 2829 2066  is_batch_dim() f
+00018240: 6f72 2074 6167 2069 6e20 6469 6d5f 7461  or tag in dim_ta
+00018250: 6773 293a 0a20 2020 2020 2020 2072 6574  gs):.        ret
+00018260: 7572 6e20 4469 6d54 7970 6573 2e42 6174  urn DimTypes.Bat
+00018270: 6368 0a20 2020 2065 6c69 6620 616e 7928  ch.    elif any(
+00018280: 7461 672e 6973 5f66 6561 7475 7265 5f64  tag.is_feature_d
+00018290: 696d 2829 2066 6f72 2074 6167 2069 6e20  im() for tag in 
+000182a0: 6469 6d5f 7461 6773 293a 0a20 2020 2020  dim_tags):.     
+000182b0: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
+000182c0: 6573 2e46 6561 7475 7265 0a20 2020 2065  es.Feature.    e
+000182d0: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
+000182e0: 7572 6e20 4469 6d54 7970 6573 2e53 7061  urn DimTypes.Spa
+000182f0: 7469 616c 0a0a 0a64 6566 2064 696d 5f63  tial...def dim_c
+00018300: 6d70 5f76 616c 7565 286f 626a 293a 0a20  mp_value(obj):. 
+00018310: 2020 2022 2222 0a20 2020 203a 7061 7261     """.    :para
+00018320: 6d20 4469 6d7c 5f4d 6172 6b65 6444 696d  m Dim|_MarkedDim
+00018330: 206f 626a 3a0a 2020 2020 3a72 6574 7572   obj:.    :retur
+00018340: 6e3a 2061 6e79 7468 696e 6720 7768 6963  n: anything whic
+00018350: 6820 6361 6e20 6265 2063 6f6d 7061 7265  h can be compare
+00018360: 640a 2020 2020 2222 220a 2020 2020 2320  d.    """.    # 
+00018370: 4d61 6b65 2044 696d 2061 6e64 205f 4d61  Make Dim and _Ma
+00018380: 726b 6564 4469 6d20 636f 6d70 6172 6162  rkedDim comparab
+00018390: 6c65 2074 6f20 6561 6368 206f 7468 6572  le to each other
+000183a0: 2e0a 2020 2020 2320 4e6f 7465 2074 6861  ..    # Note tha
+000183b0: 7420 7468 6520 6f72 6465 7220 6973 2072  t the order is r
+000183c0: 6561 6c6c 7920 6172 6269 7472 6172 7920  eally arbitrary 
+000183d0: 616e 6420 646f 6573 206e 6f74 206d 6174  and does not mat
+000183e0: 7465 722e 0a20 2020 2069 6620 6973 696e  ter..    if isin
+000183f0: 7374 616e 6365 286f 626a 2c20 5f64 2e44  stance(obj, _d.D
+00018400: 696d 293a 0a20 2020 2020 2020 206f 626a  im):.        obj
+00018410: 203d 206f 626a 2e67 6574 5f73 616d 655f   = obj.get_same_
+00018420: 6261 7365 2829 0a20 2020 2020 2020 2072  base().        r
+00018430: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
+00018440: 2020 2020 2222 2c0a 2020 2020 2020 2020      "",.        
+00018450: 2020 2020 6f62 6a2e 6465 7363 7269 7074      obj.descript
+00018460: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00018470: 206f 626a 2e6b 696e 642c 0a20 2020 2020   obj.kind,.     
+00018480: 2020 2020 2020 206f 626a 2e64 696d 656e         obj.dimen
+00018490: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+000184a0: 2020 6f62 6a2e 6479 6e5f 7369 7a65 5f65    obj.dyn_size_e
+000184b0: 7874 2e64 696d 7320 6966 206f 626a 2e64  xt.dims if obj.d
+000184c0: 796e 5f73 697a 655f 6578 7420 6973 206e  yn_size_ext is n
+000184d0: 6f74 204e 6f6e 6520 656c 7365 204e 6f6e  ot None else Non
+000184e0: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
+000184f0: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
+00018500: 626a 2c20 5f6d 2e4d 6172 6b65 6444 696d  bj, _m.MarkedDim
+00018510: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00018520: 6e20 6f62 6a2e 5f5f 636c 6173 735f 5f2e  n obj.__class__.
+00018530: 5f5f 6e61 6d65 5f5f 2c20 6f62 6a2e 7461  __name__, obj.ta
+00018540: 670a 2020 2020 7265 7475 726e 206f 626a  g.    return obj
+00018550: 0a                                       .
```

### Comparing `returnn-1.20230609.82609/returnn/tensor/_tensor_extra.py` & `returnn-1.20230614.134509/returnn/tensor/_tensor_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1542,15 +1542,20 @@
                 new_batch_dim_tag = None
                 for virtual_dim in batch.virtual_dims:
                     if isinstance(virtual_dim, BatchInfo.PackedDim):
                         dim_tags.append(virtual_dim.dim_tag)
                         batch = batch.copy_remove_dim(virtual_dim)
                     elif isinstance(virtual_dim, BatchInfo.GlobalBatchDim):
                         assert not new_batch_dim_tag
-                        new_batch_dim_tag = Dim(kind=Dim.Types.Batch, description=dim_tag.description, dimension=None)
+                        if batch is None or batch.is_global_batch():
+                            new_batch_dim_tag = batch_dim  # reuse global batch dim
+                        else:
+                            new_batch_dim_tag = Dim(
+                                kind=Dim.Types.Batch, description=dim_tag.description, dimension=None
+                            )
                         dim_tags.append(new_batch_dim_tag)
                 assert new_batch_dim_tag, "%s: batch info %r invalid" % (self, batch)
                 new_batch_dim_tag.batch = batch
                 kwargs["batch"] = batch
             else:
                 dim_tags.append(dim_tag)
 
@@ -3570,15 +3575,19 @@
         )
     elif feature_dim_axis is not None:
         if feature_dim_axis < 0:
             feature_dim_axis += len(batch_shape)
         assert 0 <= feature_dim_axis < len(batch_shape)
     dim_tags = {}
     if batch_dim_axis is not None and batch_dim_axis not in dim_tags:
-        dim_tags[batch_dim_axis] = Dim(kind=Dim.Types.Batch, description="batch:%s" % name, dimension=None)
+        if batch is None or batch.is_global_batch():
+            batch_dim_ = batch_dim  # global batch dim
+        else:
+            batch_dim_ = Dim(kind=Dim.Types.Batch, description="batch:%s" % name, batch=batch, dimension=None)
+        dim_tags[batch_dim_axis] = batch_dim_
     # Note: Consistent to Tensor.get_dim_tag,
     # prefer interpretation as spatial axis if there is a dynamic size or this is marked as time axis.
     if size_placeholder:
         for axis_wo_b, size in size_placeholder.items():
             axis = _get_axis_wb(axis_wo_b, batch_dim_axis=batch_dim_axis)
             if axis in dim_tags:
                 continue
```

### Comparing `returnn-1.20230609.82609/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230614.134509/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230614.134509/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230614.134509/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tensor/dim.py` & `returnn-1.20230614.134509/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tensor/marked_dim.py` & `returnn-1.20230614.134509/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tensor/tensor.py` & `returnn-1.20230614.134509/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tensor/tensor_dict.py` & `returnn-1.20230614.134509/returnn/tensor/tensor_dict.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 describing the data coming from the dataset (after batch preparation).
 
 We also might have model_outputs in the user config.
 (https://github.com/rwth-i6/returnn/issues/1166)
 """
 
 from __future__ import annotations
-from typing import Optional, Union, Any, Dict, Sequence
+from typing import Optional, Union, Any, Type, Dict, Sequence
 from .tensor import Tensor
 
 
 _TensorT = Union[Tensor, Dict[str, Any]]
 _DataAutoConvertT = Union[Dict[str, _TensorT], Sequence[_TensorT]]
 _DataStrictT = Union[Dict[str, Tensor], Sequence[Tensor]]
 
@@ -69,31 +69,47 @@
             if dim.dyn_size_ext:
                 dim.dyn_size_ext.reset()
 
     def copy_template(self) -> TensorDict:
         """copy template"""
         return TensorDict({k: v.copy_template() for k, v in self.data.items()})
 
-    def as_raw_tensor_dict(self, *, include_const_sizes: bool = False) -> Dict[str, Any]:
+    def as_raw_tensor_dict(
+        self, *, include_const_sizes: bool = False, expected_type: Union[Type, Sequence[Type]] = object
+    ) -> Dict[str, Any]:
         """
         :return: dict of raw tensors, including any sequence lengths / dynamic sizes
         """
         out = {}
         for key, value in self.data.items():
             assert key not in out
+            assert isinstance(
+                value.raw_tensor, expected_type
+            ), f"key {key} {value}: unexpected {type(value.raw_tensor)}, expected {expected_type}"
             out[key] = value.raw_tensor
             for i, dim in enumerate(value.dims):
                 key_ = f"{key}:size{i}"
                 assert key_ not in out
                 if dim.is_batch_dim() and (not dim.dyn_size_ext or dim.dyn_size_ext.raw_tensor is None):
-                    out[key_] = dim.get_dim_value()
+                    dim_value = dim.get_dim_value()
+                    assert isinstance(
+                        dim_value, expected_type
+                    ), f"key {key_} {dim}: unexpected {type(dim_value)}, expected {expected_type}"
+                    out[key_] = dim_value
                 elif dim.dyn_size_ext:
+                    assert isinstance(dim.dyn_size_ext.raw_tensor, expected_type), (
+                        f"key {key_} {dim} {dim.dyn_size_ext}:"
+                        f" unexpected {type(dim.dyn_size_ext.raw_tensor)}, expected {expected_type}"
+                    )
                     out[key_] = dim.dyn_size_ext.raw_tensor
                 elif dim.size is not None:
                     if include_const_sizes:
+                        assert isinstance(
+                            dim.size, expected_type
+                        ), f"key {key_} {dim}: unexpected {type(dim.size)}, expected {expected_type}"
                         out[key_] = dim.size
                 else:
                     raise Exception(f"cannot handle dim: {dim}")
         return out
 
     def assign_from_raw_tensor_dict_(self, raw_tensor_dict: Dict[str, Any]):
         """
```

### Comparing `returnn-1.20230609.82609/returnn/tensor/utils.py` & `returnn-1.20230614.134509/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/compat.py` & `returnn-1.20230614.134509/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/data_pipeline.py` & `returnn-1.20230614.134509/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/distributed.py` & `returnn-1.20230614.134509/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/engine.py` & `returnn-1.20230614.134509/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 https://github.com/rwth-i6/returnn/issues/1120
 """
 
 from __future__ import annotations
 from typing import Any, Dict, Tuple
 from tensorflow.python.util import nest
 from returnn.util.basic import BehaviorVersion
-from returnn.tensor import TensorDict, Tensor, Dim
+from returnn.tensor import TensorDict, Tensor, Dim, batch_dim
 from returnn.config import get_global_config
 import returnn.frontend as rf
 from .. import frontend_layers as rfl
 from . import _utils
 
 
 __all__ = ["get_net_dict"]
@@ -105,9 +105,14 @@
             # Dim dyn_size_ext might be Tensor[rfl.Layer],
             # but now the TF engine actually wants to have Tensor[tf.Tensor].
             # Reset it now. The TF engine should redefine it again.
             if elem.dyn_size_ext:
                 elem.dyn_size_ext.raw_tensor = None
         return elem
 
-    net_dict = nest.map_structure(_cleanup_net_dict_value, net_dict)
+    # Do some cleanup.
+    nest.map_structure(_cleanup_net_dict_value, net_dict)
+    _cleanup_net_dict_value(batch_dim)
+    for data in extern_data.data.values():
+        for dim in data.dims:
+            _cleanup_net_dict_value(dim)
     return net_dict, model
```

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230614.134509/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230614.134509/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/horovod.py` & `returnn-1.20230614.134509/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230614.134509/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/layers/base.py` & `returnn-1.20230614.134509/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/layers/basic.py` & `returnn-1.20230614.134509/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/layers/rec.py` & `returnn-1.20230614.134509/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/layers/segmental_model.py` & `returnn-1.20230614.134509/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/layers/signal_processing.py` & `returnn-1.20230614.134509/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/layers/variable.py` & `returnn-1.20230614.134509/returnn/tf/layers/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,17 +150,17 @@
                 raise TypeError("Layer %r: invalid type %s in shape %r" % (name, type(d), shape))
             dim_tags.append(d)
         if add_time_axis:
             dim_tags.insert(
                 0, Dim(kind=Dim.Types.Time, description="%s:dummy-time" % name, dimension=1, auto_generated=True)
             )
         if add_batch_axis:
-            dim_tags.insert(
-                0, Dim(kind=Dim.Types.Batch, description="batch", batch=network.get_global_batch_info(), dimension=None)
-            )
+            from returnn.tensor.dim import batch_dim
+
+            dim_tags.insert(0, batch_dim)
         return Tensor(
             name="%s_output" % name,
             dim_tags=dim_tags,
             dtype=dtype,
             batch=network.get_global_batch_info() if add_batch_axis else None,
         )
```

### Comparing `returnn-1.20230609.82609/returnn/tf/native_op.py` & `returnn-1.20230614.134509/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/network.py` & `returnn-1.20230614.134509/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/sprint.py` & `returnn-1.20230614.134509/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/updater.py` & `returnn-1.20230614.134509/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/util/basic.py` & `returnn-1.20230614.134509/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/util/data.py` & `returnn-1.20230614.134509/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/util/ken_lm.py` & `returnn-1.20230614.134509/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/tf/util/open_fst.py` & `returnn-1.20230614.134509/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/torch/data/pipeline.py` & `returnn-1.20230614.134509/returnn/torch/data/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,14 +104,18 @@
         """
         chunking_data_keys = list(self._chunk_size.keys())
 
         for data_dict in self._dataset:
 
             if not chunking_data_keys:
                 chunking_data_keys = list(data_dict.keys())  # use all if not configured separately
+                chunking_data_key_black_list = ["seq_tag"]
+                for key in chunking_data_key_black_list:
+                    if key in chunking_data_keys:
+                        chunking_data_keys.remove(key)
                 assert chunking_data_keys, "Dataset produced sequence without any data."
 
             data_chunks = {}
             num_chunks = None
 
             for data_key in chunking_data_keys:
                 chunk_size = self._chunk_size[data_key]
```

### Comparing `returnn-1.20230609.82609/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230614.134509/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/torch/data/tensor_utils.py` & `returnn-1.20230614.134509/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/torch/engine.py` & `returnn-1.20230614.134509/returnn/torch/engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from __future__ import annotations
 from typing import Optional, Union, Callable, Dict
 from contextlib import nullcontext
 
 import os
 import numpy
 import torch
+import time
+from torch.distributed import init_process_group
+from torch.nn.parallel import DistributedDataParallel
 import torch.utils.data.datapipes as dp
 from torch import autocast
 from torch.cuda import amp
 from torchdata.dataloader2 import DataLoader2
 from random import random
 
 from returnn.config import Config
 from returnn.log import log
 from returnn.engine.base import EngineBase
 import returnn.frontend as rf
 from returnn.tensor import TensorDict, Tensor, Dim
 from returnn.datasets.basic import init_dataset, Dataset
 from returnn.util import basic as util
 from returnn.util import NumbersDict
-from returnn.util.basic import NotSpecified
+from returnn.util.basic import hms, NotSpecified
 from returnn.forward_iface import ForwardCallbackIface
 
 from .updater import Updater
 from .data import pipeline as data_pipeline
 from .data import returnn_dataset_wrapper
 from .frontend.bridge import rf_module_to_pt_module
 
@@ -68,14 +71,26 @@
         self._use_autocast = False
         self._autocast_dtype = None  # type: Optional[str]
         self._grad_scaler = None  # type: Optional[amp.GradScaler]
 
         self._device = _get_device_from_config(config)
         print("Using device:", self._device, file=log.v2)
 
+        self._use_torch_distributed = False
+        self._torch_distributed_class = None  # type: Optional[Callable]
+        self._torch_distributed_options = None  # type: Optional[dict]
+        self._ddp_pt_model = None  # type: Optional[torch.nn.Module]
+        self._accum_grad_multiple_step = config.int("accum_grad_multiple_step", 1)
+
+        torch_distributed = config.typed_value("torch_distributed")
+        if torch_distributed is not None:
+            self._use_torch_distributed = True
+            self._torch_distributed_class = torch_distributed.get("class", None)
+            self._torch_distributed_options = torch_distributed.get("options", None)
+
         amp_options = self.config.typed_value("torch_amp")
         grad_scaler_opts = self.config.typed_value("grad_scaler", NotSpecified)
         if amp_options is not None:
             self._use_autocast = True
             if isinstance(amp_options, dict):
                 amp_options = util.CollectionReadCheckCovered(amp_options)
                 dtype = amp_options.get("dtype", None)
@@ -126,14 +141,22 @@
         :param train_data:
         :param dev_data:
         :param eval_data:
         """
         assert config is self.config or not config
         super().init_train_from_config(config=config)
 
+        if self._use_torch_distributed:
+            import returnn.torch.distributed
+
+            torch_distributed = returnn.torch.distributed.get_ctx(config=config)
+            local_rank = torch_distributed.local_rank()
+            print(f"Start running torch distributed training on local rank {local_rank}.", file=log.v2)
+            self._device = f"cuda:{local_rank}"
+
         self.train_dataset = train_data
         self.eval_datasets.clear()
         if dev_data:
             self.eval_datasets["dev"] = dev_data
         if eval_data:
             self.eval_datasets["eval"] = eval_data
         if config.has("eval_datasets"):
@@ -147,14 +170,21 @@
         self._start_epoch = self.get_train_start_epoch(self.config)
         self._final_epoch = self.config_get_final_epoch(self.config)
 
         self.init_network_from_config(config=config)
 
         self._save_model_epoch_interval = config.int("save_interval", 1)
 
+        if self._use_torch_distributed:
+            from returnn.torch.distributed import get_device_ids
+
+            # wrap the model use torch distributed class
+            self._ddp_pt_model = self._torch_distributed_class(
+                self._pt_model, device_ids=get_device_ids(), **self._torch_distributed_options
+            )
         self._updater = Updater(self.config, self._pt_model, self.learning_rate)
         self._updater.create_optimizer()
         if self._start_epoch > 1:
             self._load_optimizer()
 
         self._train_step_func = self.config.typed_value("train_step")
         assert self._train_step_func, "train_step not defined"
@@ -198,67 +228,114 @@
         print("start", self.get_epoch_str(), "with learning rate", self.learning_rate, "...", file=log.v4)
 
         self._pt_model.train()
 
         accumulated_losses_dict = NumbersDict()
         accumulated_inv_norm_factors_dict = NumbersDict()
         step_idx = 0
-        for extern_data_raw in self._train_dataloader:
-            self._updater.get_optimizer().zero_grad()
+        epoch_start_time = time.time()
+
+        data_iter = iter(self._train_dataloader)
+        elapsed_computation_time = 0
+
+        while True:
+            extern_data_raw = next(data_iter, None)
+            # WARNING: torch.distributed works only for the registered device,
+            # as it uses only one mechanism for communication, like NCCL.
+            # This is suboptimal here as we have the roundtrip CPU -> GPU -> NCCL -> GPU -> CPU.
+            # TODO: Use more direct CPU -> Ethernet -> CPU communication.
+            _has_data = torch.tensor([extern_data_raw is not None], dtype=torch.int8).to(self._device)
+
+            if self._use_torch_distributed:
+                # use all reduce to check if all workers have data, if at least one worker does not have data,
+                # all workers finish this epoch
+                torch.distributed.all_reduce(_has_data, op=torch.distributed.ReduceOp.MIN)
+            if not _has_data[0]:
+                break
+
+            # clear the gradients when every gradient accumulation loop starts
+            if step_idx % self._accum_grad_multiple_step == 0:
+                self._updater.get_optimizer().zero_grad()
+
+            step_begin_time = time.time()
+
             extern_data = _raw_dict_to_extern_data(
                 extern_data_raw, extern_data_template=self.extern_data, device=self._device
             )
-            self._run_step(extern_data, train_func=True, train_flag=True)
+            self._run_step(extern_data, train_flag=True, train_func=True)
 
             train_ctx = rf.get_run_ctx()
+
+            # scale the loss to account for gradient accumulation
+            if self._accum_grad_multiple_step > 1:
+                for loss_name in train_ctx.losses.keys():
+                    train_ctx.losses[loss_name].loss /= self._accum_grad_multiple_step
+
             total_loss = train_ctx.total_loss()
             losses_dict = NumbersDict(
                 {
                     name: float(loss.get_summed_loss().raw_tensor.detach().cpu().numpy())
                     for name, loss in train_ctx.losses.items()
                 }
             )
             inv_norm_factors_dict = NumbersDict(
                 {name: float(_to_raw(loss.get_inv_norm_factor())) for name, loss in train_ctx.losses.items()}
             )
 
-            if self._grad_scaler is not None:
-                self._grad_scaler.scale(total_loss).backward()
-                self._grad_scaler.step(self._updater.get_optimizer())
-                self._grad_scaler.update()
-            else:
-                total_loss.raw_tensor.backward()
-                self._updater.get_optimizer().step()
+            with self._ddp_pt_model.no_sync() if self._use_torch_distributed and (
+                step_idx % self._accum_grad_multiple_step
+            ) != (self._accum_grad_multiple_step - 1) else nullcontext():
+                if self._grad_scaler is not None:
+                    self._grad_scaler.scale(total_loss).backward()
+                else:
+                    total_loss.raw_tensor.backward()
+
+            # only update the weights when every gradient accumulation loop ends
+            if (step_idx % self._accum_grad_multiple_step) == (self._accum_grad_multiple_step - 1):
+                if self._grad_scaler is not None:
+                    self._grad_scaler.step(self._updater.get_optimizer())
+                    self._grad_scaler.update()
+                else:
+                    self._updater.get_optimizer().step()
+
+            elapsed_computation_time += time.time() - step_begin_time
 
             accumulated_losses_dict += losses_dict
             accumulated_inv_norm_factors_dict += inv_norm_factors_dict
             _print_process(
                 f"ep {self.epoch} train",
                 step=step_idx,
                 eval_info=dict(losses_dict / inv_norm_factors_dict),
             )
 
             step_idx += 1
             self.global_train_step += 1
 
-        print("Trained %i steps" % step_idx)
-
-        accumulated_losses_dict = accumulated_losses_dict / accumulated_inv_norm_factors_dict
-        self.learning_rate_control.set_epoch_error(
-            self.epoch, {f"train_loss_{k}": v for k, v in accumulated_losses_dict.items()}
+        elapsed = time.time() - epoch_start_time
+        elapsed_computation_percentage = elapsed_computation_time / elapsed
+        print(
+            "Trained %i steps, %s elapsed (%.1f%% computing time)"
+            % (step_idx, hms(elapsed), (elapsed_computation_percentage * 100.0)),
+            file=log.v3,
         )
-        self.learning_rate_control.save()
 
-        print(f"Total train loss:", _format_score(dict(accumulated_losses_dict)), file=log.v3)
+        if (not self._use_torch_distributed) or (self._use_torch_distributed and torch.distributed.get_rank() == 0):
+            accumulated_losses_dict = accumulated_losses_dict / accumulated_inv_norm_factors_dict
+            self.learning_rate_control.set_epoch_error(
+                self.epoch, {f"train_loss_{k}": v for k, v in accumulated_losses_dict.items()}
+            )
+            self.learning_rate_control.save()
+
+            print(f"Total train loss:", _format_score(dict(accumulated_losses_dict)), file=log.v3)
 
-        if self.epoch % self._save_model_epoch_interval == 0 or self.epoch == self._final_epoch:
-            self._save_model()
-            self._save_optimizer()
+            if self.epoch % self._save_model_epoch_interval == 0 or self.epoch == self._final_epoch:
+                self._save_model()
+                self._save_optimizer()
 
-        self.eval_model()
+            self.eval_model()
 
     def eval_model(self):
         """
         Runs model on all eval datasets and calculates the loss.
         """
         self._pt_model.eval()
 
@@ -366,15 +443,21 @@
         if train_func:
             assert self._train_step_func is not None
             rf.init_train_step_run_ctx(train_flag=train_flag)
         else:
             assert self._forward_step_func is not None, "define forward_step in the config"
             rf.init_forward_step_run_ctx(expected_outputs=self._forward_step_expected_outputs)
 
-        with autocast(device_type=self._device, dtype=self._autocast_dtype) if self._use_autocast else nullcontext():
+        from returnn.torch.distributed import ddp_train_forward_ctx
+
+        with autocast(
+            device_type=self._device, dtype=self._autocast_dtype
+        ) if self._use_autocast else nullcontext(), ddp_train_forward_ctx(pt_model=self._ddp_pt_model) if isinstance(
+            self._ddp_pt_model, DistributedDataParallel
+        ) else nullcontext():
             sentinel_kw = {"__fwd_compatible_random_arg_%i" % int(random() * 100): None}
             if train_func:
                 self._train_step_func(model=self._orig_model, extern_data=extern_data, **sentinel_kw)
             else:
                 self._forward_step_func(model=self._orig_model, extern_data=extern_data, **sentinel_kw)
 
     def _load_model(self):
```

### Comparing `returnn-1.20230609.82609/returnn/torch/frontend/_backend.py` & `returnn-1.20230614.134509/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/torch/frontend/_rand.py` & `returnn-1.20230614.134509/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/torch/frontend/bridge.py` & `returnn-1.20230614.134509/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/torch/updater.py` & `returnn-1.20230614.134509/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/basic.py` & `returnn-1.20230614.134509/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/better_exchook.py` & `returnn-1.20230614.134509/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/bpe.py` & `returnn-1.20230614.134509/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/debug.py` & `returnn-1.20230614.134509/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/debug_helpers.py` & `returnn-1.20230614.134509/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/fsa.py` & `returnn-1.20230614.134509/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230614.134509/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/pprint.py` & `returnn-1.20230614.134509/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/py-to-pickle.cpp` & `returnn-1.20230614.134509/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/sig_proc.py` & `returnn-1.20230614.134509/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn/util/task_system.py` & `returnn-1.20230614.134509/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/returnn.egg-info/PKG-INFO` & `returnn-1.20230614.134509/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230609.82609
+Version: 1.20230614.134509
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230609.82609/returnn.egg-info/SOURCES.txt` & `returnn-1.20230614.134509/returnn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -243,14 +243,15 @@
 returnn/tf/util/__init__.py
 returnn/tf/util/basic.py
 returnn/tf/util/data.py
 returnn/tf/util/ken_lm.py
 returnn/tf/util/open_fst.py
 returnn/torch/README.md
 returnn/torch/__init__.py
+returnn/torch/distributed.py
 returnn/torch/engine.py
 returnn/torch/updater.py
 returnn/torch/data/__init__.py
 returnn/torch/data/pipeline.py
 returnn/torch/data/returnn_dataset_wrapper.py
 returnn/torch/data/tensor_utils.py
 returnn/torch/frontend/__init__.py
```

### Comparing `returnn-1.20230609.82609/setup.py` & `returnn-1.20230614.134509/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/DummySprintExec.py` & `returnn-1.20230614.134509/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230614.134509/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230614.134509/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230614.134509/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/_set_num_threads1.py` & `returnn-1.20230614.134509/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/_setup_test_env.py` & `returnn-1.20230614.134509/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/bpe-unicode-demo.codes` & `returnn-1.20230614.134509/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/bpe-unicode-demo.vocab` & `returnn-1.20230614.134509/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/lexicon_opt.isyms` & `returnn-1.20230614.134509/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/lexicon_opt.jpg` & `returnn-1.20230614.134509/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/lint_common.py` & `returnn-1.20230614.134509/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/pycharm-inspect.py` & `returnn-1.20230614.134509/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/pylint.py` & `returnn-1.20230614.134509/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/returnn-as-framework.py` & `returnn-1.20230614.134509/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/rf_utils.py` & `returnn-1.20230614.134509/tests/rf_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from __future__ import annotations
 from typing import Optional, Union, Dict
 import contextlib
 import re
 import numpy
 import numpy.testing
+import tensorflow as tf
 
 from returnn.config import Config, global_config_ctx
 from returnn.util.pprint import pprint
 import returnn.frontend as rf
 from returnn.tensor import Tensor, Dim, TensorDict
 from returnn.tensor.utils import tensor_dict_fill_random_numpy_
 import returnn.tf.compat as tf_compat
@@ -84,15 +85,15 @@
         v_tf = out_tf_raw[k]
         numpy.testing.assert_allclose(v_pt, v_tf, atol=1e-5, rtol=1e-5, err_msg=f"output {k!r} differs")
     return out_pt
 
 
 def run_model_torch(extern_data: TensorDict, get_model: rf.GetModelFunc, forward_step: rf.StepFunc) -> TensorDict:
     """run"""
-    extern_data_raw = extern_data.as_raw_tensor_dict()
+    extern_data_raw = extern_data.as_raw_tensor_dict(expected_type=numpy.ndarray)
     rf.select_backend_torch()
     rf.set_random_seed(42)
 
     # Inplace replace Numpy by Torch.
     # Inplace because dim tags cannot easily be copied (then they are not the same).
     # We recover extern_data in the end.
     tensor_dict_numpy_to_torch_(extern_data)
@@ -106,15 +107,15 @@
 
     extern_data.assign_from_raw_tensor_dict_(extern_data_raw)
     return outputs
 
 
 def run_model_net_dict_tf(extern_data: TensorDict, get_model: rf.GetModelFunc, forward_step: rf.StepFunc) -> TensorDict:
     """run"""
-    extern_data_raw = extern_data.as_raw_tensor_dict()
+    extern_data_raw = extern_data.as_raw_tensor_dict(expected_type=numpy.ndarray)
     extern_data.reset_content()
     rf.select_backend_returnn_layers_tf()
     rf.set_random_seed(42)
 
     from returnn.tf.frontend_layers.config_entry_points import get_net_dict
 
     config = Config(
@@ -154,17 +155,17 @@
         for k, v in outputs_layers.data.items():
             v: Tensor[rfl.Layer]
             assert isinstance(v.raw_tensor, rfl.Layer)
             layer_name = v.raw_tensor.get_abs_name()
             layer = net.get_layer(layer_name)
             outputs_tf.data[k] = layer.output.copy()
 
-        fetches = outputs_tf.as_raw_tensor_dict()
+        fetches = outputs_tf.as_raw_tensor_dict(expected_type=tf.Tensor)
         assert set(extern_data.data.keys()) == set(net.extern_data.data.keys())
-        extern_data_tf_placeholders = net.extern_data.as_raw_tensor_dict()
+        extern_data_tf_placeholders = net.extern_data.as_raw_tensor_dict(expected_type=tf.Tensor)
         assert set(extern_data_tf_placeholders.keys()) == set(extern_data_raw.keys())
         feed_dict = {extern_data_tf_placeholders[k]: v for k, v in extern_data_raw.items()}
 
         outputs_numpy_raw = session.run(fetches, feed_dict=feed_dict)
 
         # Scalars are not Numpy arrays, but our code below assumes that we only have Numpy arrays.
         # So we convert them here.
```

### Comparing `returnn-1.20230609.82609/tests/spelling.dic` & `returnn-1.20230614.134509/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_Config.py` & `returnn-1.20230614.134509/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_Dataset.py` & `returnn-1.20230614.134509/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_Fsa.py` & `returnn-1.20230614.134509/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_GeneratingDataset.py` & `returnn-1.20230614.134509/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_HDFDataset.py` & `returnn-1.20230614.134509/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_LearningRateControl.py` & `returnn-1.20230614.134509/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_Log.py` & `returnn-1.20230614.134509/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_MultiProcDataset.py` & `returnn-1.20230614.134509/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_PTDataset.py` & `returnn-1.20230614.134509/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_Pretrain.py` & `returnn-1.20230614.134509/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_ResNet.py` & `returnn-1.20230614.134509/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_SprintDataset.py` & `returnn-1.20230614.134509/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_SprintInterface.py` & `returnn-1.20230614.134509/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TFEngine.py` & `returnn-1.20230614.134509/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TFNativeOp.py` & `returnn-1.20230614.134509/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TFNetworkLayer.py` & `returnn-1.20230614.134509/tests/test_TFNetworkLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -7819,14 +7819,16 @@
     rnd = numpy.random.RandomState(42)
     seqs = rnd.randint(1, 100, (n_batch, n_time, n_dim)).astype("float32")  # all != 0
     seq_lens = numpy.array([n_time, n_time - 2, n_time - 3, n_time - 1, n_time - 4], dtype="int32")
     starts = numpy.array([2, 1, 3, n_time + 1, -1], dtype="int32")
     size = 5
     with make_scope() as session:
         net = TFNetwork(extern_data=ExternData())
+        batch = BatchInfo.make_global_batch_info(tf.constant(n_batch))
+        net.extern_data.set_batch_info(batch)
         src = InternalLayer(name="src", network=net, output=Data(name="src", dim=n_dim))
         src.output.placeholder = tf.constant(seqs)
         src.output.size_placeholder = {0: tf.constant(seq_lens)}
         src.output.sanity_check()
         start = InternalLayer(
             name="start",
             network=net,
@@ -9291,14 +9293,15 @@
 
 def test_PostfixInTimeLayer():
     with make_scope() as session:
         import numpy as np
 
         net = TFNetwork(extern_data=ExternData())
         batch = BatchInfo.make_global_batch_info(tf.constant(2))
+        net.extern_data.set_batch_info(batch)
         src = InternalLayer(name="src", network=net, output=Data(name="src", dim=2, dtype="int32", batch=batch))
         src_seqs = np.array([[[1, 1], [2, 2], [3, 3], [4, 4], [5, 5]], [[6, 6], [7, 7], [8, 8], [0, 0], [0, 0]]])
         src_seq_lens = [5, 3]
         src.output.placeholder = tf.constant(src_seqs, dtype=tf.int32)
         src.output.size_placeholder = {0: tf.constant(src_seq_lens, dtype=tf.int32)}
 
         static_postfix = -7
```

### Comparing `returnn-1.20230609.82609/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230614.134509/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230614.134509/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TFUpdater.py` & `returnn-1.20230614.134509/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TFUtil.py` & `returnn-1.20230614.134509/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TF_determinism.py` & `returnn-1.20230614.134509/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TaskSystem.py` & `returnn-1.20230614.134509/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230614.134509/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_TranslationDataset.py` & `returnn-1.20230614.134509/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_Util.py` & `returnn-1.20230614.134509/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_demos.py` & `returnn-1.20230614.134509/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_fork_exec.py` & `returnn-1.20230614.134509/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_hdf_dump.py` & `returnn-1.20230614.134509/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_array.py` & `returnn-1.20230614.134509/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_attention.py` & `returnn-1.20230614.134509/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_base.py` & `returnn-1.20230614.134509/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_cond.py` & `returnn-1.20230614.134509/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_container.py` & `returnn-1.20230614.134509/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_conv.py` & `returnn-1.20230614.134509/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_encoder_conformer.py` & `returnn-1.20230614.134509/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_loop.py` & `returnn-1.20230614.134509/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_math.py` & `returnn-1.20230614.134509/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_normalization.py` & `returnn-1.20230614.134509/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_rec.py` & `returnn-1.20230614.134509/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_reduce.py` & `returnn-1.20230614.134509/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_rf_signal.py` & `returnn-1.20230614.134509/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_tensor.py` & `returnn-1.20230614.134509/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_tools.py` & `returnn-1.20230614.134509/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_torch_engine.py` & `returnn-1.20230614.134509/tests/test_torch_engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_torch_frontend.py` & `returnn-1.20230614.134509/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tests/test_torch_internal_frontend.py` & `returnn-1.20230614.134509/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/analyze-dataset-batches.py` & `returnn-1.20230614.134509/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/bliss-collect-seq-lens.py` & `returnn-1.20230614.134509/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/bliss-dump-text.py` & `returnn-1.20230614.134509/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/bliss-get-segment-names.py` & `returnn-1.20230614.134509/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/bliss-to-ogg-zip.py` & `returnn-1.20230614.134509/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/bpe-create-lexicon.py` & `returnn-1.20230614.134509/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/calculate-word-error-rate.py` & `returnn-1.20230614.134509/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/cleanup-old-models.py` & `returnn-1.20230614.134509/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/collect-orth-symbols.py` & `returnn-1.20230614.134509/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/collect-words.py` & `returnn-1.20230614.134509/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/compile_native_op.py` & `returnn-1.20230614.134509/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/compile_tf_graph.py` & `returnn-1.20230614.134509/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/debug-dump-search-scores.py` & `returnn-1.20230614.134509/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/debug-plot-search-scores.py` & `returnn-1.20230614.134509/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/dump-dataset-raw-strings.py` & `returnn-1.20230614.134509/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/dump-dataset.py` & `returnn-1.20230614.134509/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/dump-forward-stats.py` & `returnn-1.20230614.134509/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/dump-forward.py` & `returnn-1.20230614.134509/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/dump-network-json.py` & `returnn-1.20230614.134509/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/dump-pickle.py` & `returnn-1.20230614.134509/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230614.134509/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/get-attention-weights.py` & `returnn-1.20230614.134509/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/get-best-model-epoch.py` & `returnn-1.20230614.134509/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/hdf_dump.py` & `returnn-1.20230614.134509/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230614.134509/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/import-blocks-mt-model.py` & `returnn-1.20230614.134509/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/import-t2t-mt-model.py` & `returnn-1.20230614.134509/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/Makefile` & `returnn-1.20230614.134509/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/README.md` & `returnn-1.20230614.134509/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/example/README.md` & `returnn-1.20230614.134509/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230614.134509/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230614.134509/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/file.h` & `returnn-1.20230614.134509/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230614.134509/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230614.134509/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/main.cc` & `returnn-1.20230614.134509/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230614.134509/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230614.134509/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230614.134509/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/tf_avg_checkpoints.py` & `returnn-1.20230614.134509/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/tf_inspect_checkpoint.py` & `returnn-1.20230614.134509/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/tf_inspect_summary_log.py` & `returnn-1.20230614.134509/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230609.82609/tools/torch_export_to_onnx.py` & `returnn-1.20230614.134509/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

