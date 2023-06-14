# Comparing `tmp/weaver-core-0.4.2.tar.gz` & `tmp/weaver-core-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaver-core-0.4.2.tar", last modified: Wed Jan 25 16:16:56 2023, max compression
+gzip compressed data, was "weaver-core-0.4.3.tar", last modified: Wed Jun 14 15:23:18 2023, max compression
```

## Comparing `weaver-core-0.4.2.tar` & `weaver-core-0.4.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.188616 weaver-core-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-25 16:16:09.000000 weaver-core-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-01-25 16:16:56.188616 weaver-core-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-01-25 16:16:09.000000 weaver-core-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 16:16:56.188616 weaver-core-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-25 16:16:09.000000 weaver-core-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.184616 weaver-core-0.4.2/weaver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.184616 weaver-core-0.4.2/weaver/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.184616 weaver-core-0.4.2/weaver/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/nn/loss/focal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.184616 weaver-core-0.4.2/weaver/nn/model/
--rw-r--r--   0 runner    (1001) docker     (123)    35306 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/nn/model/ParticleNeXt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/nn/model/ParticleNet.py
--rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/nn/model/ParticleTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/nn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44214 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.184616 weaver-core-0.4.2/weaver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.184616 weaver-core-0.4.2/weaver/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/data/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/data/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/data/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    17840 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/import_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/lr_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.184616 weaver-core-0.4.2/weaver/utils/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/nn/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.184616 weaver-core-0.4.2/weaver/utils/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/nn/optimizer/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/nn/optimizer/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/nn/optimizer/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-01-25 16:16:09.000000 weaver-core-0.4.2/weaver/utils/nn/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 16:16:56.184616 weaver-core-0.4.2/weaver_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-01-25 16:16:56.000000 weaver-core-0.4.2/weaver_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-25 16:16:56.000000 weaver-core-0.4.2/weaver_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 16:16:56.000000 weaver-core-0.4.2/weaver_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-25 16:16:56.000000 weaver-core-0.4.2/weaver_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 16:16:56.000000 weaver-core-0.4.2/weaver_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-25 16:16:56.000000 weaver-core-0.4.2/weaver_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-25 16:16:56.000000 weaver-core-0.4.2/weaver_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.529950 weaver-core-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 15:22:35.000000 weaver-core-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-14 15:23:18.529950 weaver-core-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-06-14 15:22:35.000000 weaver-core-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:23:18.529950 weaver-core-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-14 15:22:35.000000 weaver-core-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/loss/focal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/nn/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    35306 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/model/ParticleNeXt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/model/ParticleNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/model/ParticleTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45296 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/import_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/lr_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/utils/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/utils/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/optimizer/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/optimizer/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/optimizer/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/top_level.txt
```

### Comparing `weaver-core-0.4.2/LICENSE` & `weaver-core-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/PKG-INFO` & `weaver-core-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaver-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: A streamlined deep-learning framework for high energy physics
 Home-page: https://github.com/hqucms/weaver-core
 Author: H. Qu, C. Li
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `weaver-core-0.4.2/README.md` & `weaver-core-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/setup.py` & `weaver-core-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         if not line:
             continue
         if line.startswith('#'):
             continue
         install_requires.append(line)
 
 setup(name="weaver-core",
-      version='0.4.2',
+      version='0.4.3',
       description="A streamlined deep-learning framework for high energy physics",
       long_description_content_type="text/markdown",
       author="H. Qu, C. Li",
       url="https://github.com/hqucms/weaver-core",
       long_description=long_desc,
       entry_points={'console_scripts':
                     ['weaver = weaver.train:main']},
```

### Comparing `weaver-core-0.4.2/weaver/nn/loss/focal.py` & `weaver-core-0.4.3/weaver/nn/loss/focal.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/nn/model/ParticleNeXt.py` & `weaver-core-0.4.3/weaver/nn/model/ParticleNeXt.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/nn/model/ParticleNet.py` & `weaver-core-0.4.3/weaver/nn/model/ParticleNet.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/nn/model/ParticleTransformer.py` & `weaver-core-0.4.3/weaver/nn/model/ParticleTransformer.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/train.py` & `weaver-core-0.4.3/weaver/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,16 @@
                          'will saved to `{model_prefix}_epoch-%d_state.pt` after each epoch, and the one with the best '
                          'validation metric to `{model_prefix}_best_epoch_state.pt`; for testing, this should be the full path '
                          'including the suffix, otherwise the one with the best validation metric will be used; '
                          'for training, `{auto}` can be used as part of the path to auto-generate a name, '
                          'based on the timestamp and network configuration')
 parser.add_argument('--load-model-weights', type=str, default=None,
                     help='initialize model with pre-trained weights')
+parser.add_argument('--exclude-model-weights', type=str, default=None,
+                    help='comma-separated regex to exclude matched weights from being loaded, e.g., `a.fc..+,b.fc..+`')
 parser.add_argument('--num-epochs', type=int, default=20,
                     help='number of epochs')
 parser.add_argument('--steps-per-epoch', type=int, default=None,
                     help='number of steps (iterations) per epochs; '
                          'if neither of `--steps-per-epoch` or `--samples-per-epoch` is set, each epoch will run over all loaded samples')
 parser.add_argument('--steps-per-epoch-val', type=int, default=None,
                     help='number of steps (iterations) per epochs for validation; '
@@ -117,14 +119,16 @@
 parser.add_argument('--predict', action='store_true', default=False,
                     help='run prediction instead of training')
 parser.add_argument('--predict-output', type=str,
                     help='path to save the prediction output, support `.root` and `.parquet` format')
 parser.add_argument('--export-onnx', type=str, default=None,
                     help='export the PyTorch model to ONNX model and save it at the given path (path must ends w/ .onnx); '
                          'needs to set `--data-config`, `--network-config`, and `--model-prefix` (requires the full model path)')
+parser.add_argument('--onnx-opset', type=int, default=15,
+                    help='ONNX opset version.')
 parser.add_argument('--io-test', action='store_true', default=False,
                     help='test throughput of the dataloader')
 parser.add_argument('--copy-inputs', action='store_true', default=False,
                     help='copy input files to the current dir (can help to speed up dataloading when running over remote files, e.g., from EOS)')
 parser.add_argument('--log', type=str, default='',
                     help='path to the log file; `{auto}` can be used as part of the path to auto-generate a name, based on the timestamp and network configuration')
 parser.add_argument('--print', action='store_true', default=False,
@@ -332,15 +336,15 @@
     os.makedirs(os.path.dirname(args.export_onnx), exist_ok=True)
     inputs = tuple(
         torch.ones(model_info['input_shapes'][k], dtype=torch.float32) for k in model_info['input_names'])
     torch.onnx.export(model, inputs, args.export_onnx,
                       input_names=model_info['input_names'],
                       output_names=model_info['output_names'],
                       dynamic_axes=model_info.get('dynamic_axes', None),
-                      opset_version=13)
+                      opset_version=args.onnx_opset)
     _logger.info('ONNX model saved to %s', args.export_onnx)
 
     preprocessing_json = os.path.join(os.path.dirname(args.export_onnx), 'preprocess.json')
     data_config.export_json(preprocessing_json)
     _logger.info('Preprocessing parameters saved to %s', preprocessing_json)
 
 
@@ -555,14 +559,26 @@
     if args.export_onnx:
         network_options['for_inference'] = True
     if args.use_amp:
         network_options['use_amp'] = True
     model, model_info = network_module.get_model(data_config, **network_options)
     if args.load_model_weights:
         model_state = torch.load(args.load_model_weights, map_location='cpu')
+        if args.exclude_model_weights:
+            import re
+            exclude_patterns = args.exclude_model_weights.split(',')
+            _logger.info('The following weights will not be loaded: %s' % str(exclude_patterns))
+            key_state = {}
+            for k in model_state.keys():
+                key_state[k] = True
+                for pattern in exclude_patterns:
+                    if re.match(pattern, k):
+                        key_state[k] = False
+                        break
+            model_state = {k: v for k, v in model_state.items() if key_state[k]}
         missing_keys, unexpected_keys = model.load_state_dict(model_state, strict=False)
         _logger.info('Model initialized with weights from %s\n ... Missing: %s\n ... Unexpected: %s' %
                      (args.load_model_weights, missing_keys, unexpected_keys))
     # _logger.info(model)
     flops(model, model_info)
     # loss function
     try:
@@ -888,21 +904,25 @@
         args.log += '.%03d' % args.local_rank
         if args.local_rank != 0:
             stdout = None
     _configLogger('weaver', stdout=stdout, filename=args.log)
 
     if args.cross_validation:
         model_dir, model_fn = os.path.split(args.model_prefix)
+        load_model = args.load_model_weights or None
         var_name, kfold = args.cross_validation.split('%')
         kfold = int(kfold)
         for i in range(kfold):
             _logger.info(f'\n=== Running cross validation, fold {i} of {kfold} ===')
             args.model_prefix = os.path.join(f'{model_dir}_fold{i}', model_fn)
             args.extra_selection = f'{var_name}%{kfold}!={i}'
             args.extra_test_selection = f'{var_name}%{kfold}=={i}'
+            if load_model and '{fold}' in load_model:
+                args.load_model_weights = load_model.replace('{fold}', f'fold{i}')
+
             _main(args)
     else:
         _main(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `weaver-core-0.4.2/weaver/utils/data/config.py` & `weaver-core-0.4.3/weaver/utils/data/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     r"""Data loading configuration.
     """
 
     def __init__(self, print_info=True, **kwargs):
 
         opts = {
             'treename': None,
+            'branch_magic': None,
             'selection': None,
             'test_time_selection': None,
             'preprocess': {'method': 'manual', 'data_fraction': 0.1, 'params': None},
             'new_variables': {},
             'inputs': {},
             'labels': {},
             'observers': [],
```

### Comparing `weaver-core-0.4.2/weaver/utils/data/fileio.py` & `weaver-core-0.4.3/weaver/utils/data/fileio.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,32 +16,45 @@
     start = math.trunc(load_range[0] * len(outputs[branches[0]]))
     stop = max(start + 1, math.trunc(load_range[1] * len(outputs[branches[0]])))
     for k, v in outputs.items():
         outputs[k] = v[start:stop]
     return ak.Array(outputs)
 
 
-def _read_root(filepath, branches, load_range=None, treename=None):
+def _read_root(filepath, branches, load_range=None, treename=None, branch_magic=None):
     import uproot
     with uproot.open(filepath) as f:
         if treename is None:
             treenames = set([k.split(';')[0] for k, v in f.items() if getattr(v, 'classname', '') == 'TTree'])
             if len(treenames) == 1:
                 treename = treenames.pop()
             else:
                 raise RuntimeError(
                     'Need to specify `treename` as more than one trees are found in file %s: %s' %
-                    (filepath, str(branches)))
+                    (filepath, str(treenames)))
         tree = f[treename]
         if load_range is not None:
             start = math.trunc(load_range[0] * tree.num_entries)
             stop = max(start + 1, math.trunc(load_range[1] * tree.num_entries))
         else:
             start, stop = None, None
-        outputs = tree.arrays(filter_name=branches, entry_start=start, entry_stop=stop)
+        if branch_magic is not None:
+            branch_dict = {}
+            for name in branches:
+                decoded_name = name
+                for src, tgt in branch_magic.items():
+                    if src in decoded_name:
+                        decoded_name = decoded_name.replace(src, tgt)
+                branch_dict[name] = decoded_name
+            outputs = tree.arrays(filter_name=list(branch_dict.values()), entry_start=start, entry_stop=stop)
+            for name, decoded_name in branch_dict.items():
+                if name != decoded_name:
+                    outputs[name] = outputs[decoded_name]
+        else:
+            outputs = tree.arrays(filter_name=branches, entry_start=start, entry_stop=stop)
     return outputs
 
 
 def _read_awkd(filepath, branches, load_range=None):
     import awkward0
     with awkward0.load(filepath) as f:
         outputs = {k: f[k] for k in branches}
@@ -73,15 +86,17 @@
         ext = os.path.splitext(filepath)[1]
         if ext not in ('.h5', '.root', '.awkd', '.parquet'):
             raise RuntimeError('File %s of type `%s` is not supported!' % (filepath, ext))
         try:
             if ext == '.h5':
                 a = _read_hdf5(filepath, branches, load_range=load_range)
             elif ext == '.root':
-                a = _read_root(filepath, branches, load_range=load_range, treename=kwargs.get('treename', None))
+                a = _read_root(filepath, branches, load_range=load_range,
+                               treename=kwargs.get('treename', None),
+                               branch_magic=kwargs.get('branch_magic', None))
             elif ext == '.awkd':
                 a = _read_awkd(filepath, branches, load_range=load_range)
             elif ext == '.parquet':
                 a = _read_parquet(filepath, branches, load_range=load_range)
         except Exception as e:
             a = None
             _logger.error('When reading file %s:', filepath)
```

### Comparing `weaver-core-0.4.2/weaver/utils/data/preprocess.py` & `weaver-core-0.4.3/weaver/utils/data/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,16 @@
                     self.load_branches.update(_get_variable_names(expr))
                 else:
                     self.load_branches.add(k)
         if self._data_config.selection:
             self.load_branches.update(_get_variable_names(self._data_config.selection))
         _logger.debug('[AutoStandardizer] keep_branches:\n  %s', ','.join(self.keep_branches))
         _logger.debug('[AutoStandardizer] load_branches:\n  %s', ','.join(self.load_branches))
-        table = _read_files(filelist, self.load_branches, self.load_range,
-                            show_progressbar=True, treename=self._data_config.treename)
+        table = _read_files(filelist, self.load_branches, self.load_range, show_progressbar=True,
+                            treename=self._data_config.treename, branch_magic=self._data_config.branch_magic)
         table = _apply_selection(table, self._data_config.selection)
         table = _build_new_variables(
             table, {k: v for k, v in self._data_config.var_funcs.items() if k in self.keep_branches})
         table = _clean_up(table, self.load_branches - self.keep_branches)
         return table
 
     def make_preprocess_params(self, table):
@@ -174,15 +174,16 @@
                 self.load_branches.update(_get_variable_names(expr))
             else:
                 self.load_branches.add(k)
         if self._data_config.selection:
             self.load_branches.update(_get_variable_names(self._data_config.selection))
         _logger.debug('[WeightMaker] keep_branches:\n  %s', ','.join(self.keep_branches))
         _logger.debug('[WeightMaker] load_branches:\n  %s', ','.join(self.load_branches))
-        table = _read_files(filelist, self.load_branches, show_progressbar=True, treename=self._data_config.treename)
+        table = _read_files(filelist, self.load_branches, show_progressbar=True,
+                            treename=self._data_config.treename, branch_magic=self._data_config.branch_magic)
         table = _apply_selection(table, self._data_config.selection)
         table = _build_new_variables(
             table, {k: v for k, v in self._data_config.var_funcs.items() if k in self.keep_branches})
         table = _clean_up(table, self.load_branches - self.keep_branches)
         return table
 
     def make_weights(self, table):
```

### Comparing `weaver-core-0.4.2/weaver/utils/data/tools.py` & `weaver-core-0.4.3/weaver/utils/data/tools.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/utils/dataset.py` & `weaver-core-0.4.3/weaver/utils/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,16 @@
         np.random.shuffle(indices)
     # perform input variable standardization, clipping, padding and stacking
     table = _finalize_inputs(table, data_config)
     return table, indices
 
 
 def _load_next(data_config, filelist, load_range, options):
-    table = _read_files(filelist, data_config.load_branches, load_range, treename=data_config.treename)
+    table = _read_files(filelist, data_config.load_branches, load_range,
+                        treename=data_config.treename, branch_magic=data_config.branch_magic)
     table, indices = _preprocess(table, data_config, options)
     return table, indices
 
 
 class _SimpleIter(object):
     r"""_SimpleIter
 
@@ -138,15 +139,15 @@
             self._name += '_worker%d' % worker_info.id
             self._seed = worker_info.seed & 0xFFFFFFFF
             np.random.seed(self._seed)
             # split workload by files
             new_file_dict = {}
             for name, files in file_dict.items():
                 new_files = files[worker_info.id::worker_info.num_workers]
-                assert(len(new_files) > 0)
+                assert (len(new_files) > 0)
                 new_file_dict[name] = new_files
             file_dict = new_file_dict
         self.worker_file_dict = file_dict
         self.worker_filelist = sum(file_dict.values(), [])
         self.worker_info = worker_info
         self.restart()
```

### Comparing `weaver-core-0.4.2/weaver/utils/flops_counter.py` & `weaver-core-0.4.3/weaver/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/utils/logger.py` & `weaver-core-0.4.3/weaver/utils/logger.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/utils/lr_finder.py` & `weaver-core-0.4.3/weaver/utils/lr_finder.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/utils/nn/metrics.py` & `weaver-core-0.4.3/weaver/utils/nn/metrics.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/utils/nn/optimizer/lookahead.py` & `weaver-core-0.4.3/weaver/utils/nn/optimizer/lookahead.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/utils/nn/optimizer/radam.py` & `weaver-core-0.4.3/weaver/utils/nn/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver/utils/nn/tools.py` & `weaver-core-0.4.3/weaver/utils/nn/tools.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.2/weaver_core.egg-info/PKG-INFO` & `weaver-core-0.4.3/weaver_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaver-core
-Version: 0.4.2
+Version: 0.4.3
 Summary: A streamlined deep-learning framework for high energy physics
 Home-page: https://github.com/hqucms/weaver-core
 Author: H. Qu, C. Li
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `weaver-core-0.4.2/weaver_core.egg-info/SOURCES.txt` & `weaver-core-0.4.3/weaver_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

