# Comparing `tmp/opengsl-0.0.1.tar.gz` & `tmp/opengsl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengsl-0.0.1.tar", last modified: Wed Jun 14 06:20:52 2023, max compression
+gzip compressed data, was "opengsl-0.0.2.tar", last modified: Wed Jun 14 08:12:25 2023, max compression
```

## Comparing `opengsl-0.0.1.tar` & `opengsl-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 06:20:52.929229 opengsl-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-06-14 05:42:30.000000 opengsl-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6599 2023-06-14 06:20:52.928229 opengsl-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5833 2023-06-14 06:13:18.000000 opengsl-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 06:20:52.903230 opengsl-0.0.1/opengsl/
--rw-rw-rw-   0        0        0     4090 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/ExpManager.py
--rw-rw-rw-   0        0        0      103 2023-06-14 06:13:18.000000 opengsl-0.0.1/opengsl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:20:52.911227 opengsl-0.0.1/opengsl/data/
--rw-rw-rw-   0        0        0       28 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/data/__init__.py
--rw-rw-rw-   0        0        0     6844 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/data/dataset.py
--rw-rw-rw-   0        0        0     1209 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/data/hetero_load.py
--rw-rw-rw-   0        0        0     1242 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/data/homophily_control.py
--rw-rw-rw-   0        0        0     1612 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/data/pyg_load.py
--rw-rw-rw-   0        0        0     3116 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/data/split.py
--rw-rw-rw-   0        0        0     3181 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/load_conf.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:20:52.913226 opengsl-0.0.1/opengsl/method/
--rw-rw-rw-   0        0        0      985 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/__init__.py
--rw-rw-rw-   0        0        0     9235 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/gnnsolver.py
--rw-rw-rw-   0        0        0    90850 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/gslsolver.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:20:52.925228 opengsl-0.0.1/opengsl/method/models/
--rw-rw-rw-   0        0        0        0 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/__init__.py
--rw-rw-rw-   0        0        0    13055 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/cogsl.py
--rw-rw-rw-   0        0        0     5535 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/gaug.py
--rw-rw-rw-   0        0        0     4584 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/gcn.py
--rw-rw-rw-   0        0        0     3470 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/gcn_idgl.py
--rw-rw-rw-   0        0        0     5153 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/gen.py
--rw-rw-rw-   0        0        0     9332 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/gnn_modules.py
--rw-rw-rw-   0        0        0     5704 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/grcn.py
--rw-rw-rw-   0        0        0    11587 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/gt.py
--rw-rw-rw-   0        0        0    10579 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/idgl.py
--rw-rw-rw-   0        0        0     4696 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/jknet.py
--rw-rw-rw-   0        0        0    14225 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/nodeformer.py
--rw-rw-rw-   0        0        0     6836 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/prognn.py
--rw-rw-rw-   0        0        0    31469 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/segsl.py
--rw-rw-rw-   0        0        0    11028 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/slaps.py
--rw-rw-rw-   0        0        0     6613 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/stable.py
--rw-rw-rw-   0        0        0    15908 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/models/sublime.py
--rw-rw-rw-   0        0        0     6184 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/method/solver.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:20:52.927230 opengsl-0.0.1/opengsl/utils/
--rw-rw-rw-   0        0        0       20 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/utils/__init__.py
--rw-rw-rw-   0        0        0     1392 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/utils/logger.py
--rw-rw-rw-   0        0        0     1107 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/utils/recorder.py
--rw-rw-rw-   0        0        0     6901 2023-06-14 05:42:30.000000 opengsl-0.0.1/opengsl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 06:20:52.907228 opengsl-0.0.1/opengsl.egg-info/
--rw-rw-rw-   0        0        0     6599 2023-06-14 06:20:52.000000 opengsl-0.0.1/opengsl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1146 2023-06-14 06:20:52.000000 opengsl-0.0.1/opengsl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 06:20:52.000000 opengsl-0.0.1/opengsl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-06-14 06:20:52.000000 opengsl-0.0.1/opengsl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 06:20:52.000000 opengsl-0.0.1/opengsl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 06:20:52.929229 opengsl-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-06-14 06:10:55.000000 opengsl-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:12:25.739477 opengsl-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-06-14 05:42:30.000000 opengsl-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6556 2023-06-14 08:12:25.738475 opengsl-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5790 2023-06-14 07:15:00.000000 opengsl-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 08:12:25.710850 opengsl-0.0.2/opengsl/
+-rw-rw-rw-   0        0        0     4090 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/ExpManager.py
+-rw-rw-rw-   0        0        0      163 2023-06-14 07:15:00.000000 opengsl-0.0.2/opengsl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:12:25.726493 opengsl-0.0.2/opengsl/data/
+-rw-rw-rw-   0        0        0       28 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/data/__init__.py
+-rw-rw-rw-   0        0        0     7559 2023-06-14 07:36:43.000000 opengsl-0.0.2/opengsl/data/dataset.py
+-rw-rw-rw-   0        0        0     1845 2023-06-14 07:15:01.000000 opengsl-0.0.2/opengsl/data/hetero_load.py
+-rw-rw-rw-   0        0        0     1242 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/data/homophily_control.py
+-rw-rw-rw-   0        0        0     1743 2023-06-14 07:38:00.000000 opengsl-0.0.2/opengsl/data/pyg_load.py
+-rw-rw-rw-   0        0        0     3116 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/data/split.py
+-rw-rw-rw-   0        0        0     3181 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/load_conf.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:12:25.728493 opengsl-0.0.2/opengsl/method/
+-rw-rw-rw-   0        0        0      985 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/__init__.py
+-rw-rw-rw-   0        0        0     9235 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/gnnsolver.py
+-rw-rw-rw-   0        0        0    90850 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/gslsolver.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:12:25.736500 opengsl-0.0.2/opengsl/method/models/
+-rw-rw-rw-   0        0        0        0 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/__init__.py
+-rw-rw-rw-   0        0        0    13055 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/cogsl.py
+-rw-rw-rw-   0        0        0     5535 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/gaug.py
+-rw-rw-rw-   0        0        0     4584 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/gcn.py
+-rw-rw-rw-   0        0        0     3470 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/gcn_idgl.py
+-rw-rw-rw-   0        0        0     5153 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/gen.py
+-rw-rw-rw-   0        0        0     9332 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/gnn_modules.py
+-rw-rw-rw-   0        0        0     5704 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/grcn.py
+-rw-rw-rw-   0        0        0    11587 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/gt.py
+-rw-rw-rw-   0        0        0    10579 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/idgl.py
+-rw-rw-rw-   0        0        0     4696 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/jknet.py
+-rw-rw-rw-   0        0        0    14225 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/nodeformer.py
+-rw-rw-rw-   0        0        0     6836 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/prognn.py
+-rw-rw-rw-   0        0        0    31469 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/segsl.py
+-rw-rw-rw-   0        0        0    11028 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/slaps.py
+-rw-rw-rw-   0        0        0     6613 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/stable.py
+-rw-rw-rw-   0        0        0    15908 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/models/sublime.py
+-rw-rw-rw-   0        0        0     6184 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/method/solver.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:12:25.738475 opengsl-0.0.2/opengsl/utils/
+-rw-rw-rw-   0        0        0       20 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/utils/__init__.py
+-rw-rw-rw-   0        0        0     1392 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/utils/logger.py
+-rw-rw-rw-   0        0        0     1107 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/utils/recorder.py
+-rw-rw-rw-   0        0        0     6901 2023-06-14 05:42:30.000000 opengsl-0.0.2/opengsl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:12:25.723477 opengsl-0.0.2/opengsl.egg-info/
+-rw-rw-rw-   0        0        0     6556 2023-06-14 08:12:25.000000 opengsl-0.0.2/opengsl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1146 2023-06-14 08:12:25.000000 opengsl-0.0.2/opengsl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:12:25.000000 opengsl-0.0.2/opengsl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-06-14 08:12:25.000000 opengsl-0.0.2/opengsl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 08:12:25.000000 opengsl-0.0.2/opengsl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:12:25.739477 opengsl-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1363 2023-06-14 08:11:52.000000 opengsl-0.0.2/setup.py
```

### Comparing `opengsl-0.0.1/LICENSE` & `opengsl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/PKG-INFO` & `opengsl-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengsl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A comprehensive benchmark for Graph Structure Learning.
 Home-page: https://github.com/OpenGSL/OpenGSL
 Author: Zhiyao Zhou, Sheng Zhou, Bochao Mao, Xuanyi Zhou
 Keywords: AI,GNN,graph structure learning
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -46,33 +46,35 @@
 ``` python
 import opengsl
 conf = opengsl.load_conf(method="gcn", dataset="cora")
 ```
 
 #### Step 2: Load data
 ``` python
-import opengsl.data
 dataset = opengsl.data.Dataset("cora", n_splits=1, feat_norm=conf.dataset['feat_norm'])
 ```
 
 #### Step 3: Build Model
 ``` python
-import opengsl.method
 solver = opengsl.method.gcn(conf,dataset)
 ```
 
 #### Step 4: Training and Evaluation
 ``` python
 exp = opengsl.ExpManager(solver, n_runs = 10)
 exp.run()
 ```
 
+## Add method
+if you want to use your own method, see `example.py` for detail.
+
+
 ## Node Classification Results
 | **Model**      | **Cora**     | **Citeseer** | **Pubmed**   | **Questions** | **Minesweeper** |
-|--------------|:------------:|:------------:|:------------:|:-------------:|:---------------:|
+|----------------|:------------:|:------------:|:------------:|:-------------:|:---------------:|
 | **GCN**        | 81.95 卤 0.62 | 71.34 卤 0.48 | 78.98 卤 0.35 | 75.80 卤 0.51  | 78.28 卤 0.44    |
 | **ProGNN**     | 80.27 卤 0.48 | 71.35 卤 0.42 | 79.39 卤 0.29 | --            | 51.43 卤 2.22    |
 | **IDGL**       | 84.19 卤 0.61 | 73.26 卤 0.53 | 82.78 卤 0.44 | 50.00 卤 0.00  | 50.00 卤 0.00    |
 | **GRCN**       | 84.61 卤 0.34 | 72.34 卤 0.73 | 79.30 卤 0.34 | 74.50 卤 0.84  | 72.57 卤 0.49    |
 | **GAug(O)**    | 83.43 卤 0.53 | 72.79 卤 0.86 | 78.73 卤 0.77 | --            | 77.93 卤 0.64    |
 | **SLAPS**      | 72.29 卤 1.01 | 70.00 卤 1.29 | 70.96 卤 0.99 | --            | 50.89 卤 1.72    |
 | **GT**         | 80.79 卤 1.14 | 68.50 卤 2.07 | 77.91 卤 0.58 | 75.36 卤 0.92  | 89.70 卤 0.28    |
@@ -81,37 +83,29 @@
 | **CoGSL**      | 81.46 卤 0.88 | 72.94 卤 0.71 | --           | --            | --              |
 | **SEGSL**      | 81.04 卤 1.07 | 71.57 卤 0.40 | 79.26 卤 0.67 | --            | --              |
 | **SUBLIME**    | 83.33 卤 0.73 | 72.44 卤 0.89 | 80.56 卤 1.32 | 67.21 卤 0.99  | 49.93 卤 1.36    |
 | **STABLE**     | 83.25 卤 0.86 | 70.99 卤 1.19 | 81.46 卤 0.78 | --            | 70.78 卤 0.27    |
 
 
 | **Model**      | **BlogCatalog** | **Flickr**   | **Amazon-ratings** | **Roman-empire** | **Wiki-cooc**  |
-|--------------|:---------------:|:------------:|:------------------:|:----------------:|:--------------:|
+|----------------|:---------------:|:------------:|:------------------:|:----------------:|:--------------:|
 | **GCN**        | 76.12 卤 0.42    | 61.60 卤 0.49 | 45.24 卤 0.29       | 70.41 卤 0.47     | 92.03 卤 0.19   |
 | **ProGNN**     | 73.38 卤 0.30    | 52.88 卤 0.76 | --                 | 56.21 卤 0.58     | 89.07 卤 5.59   |
 | **IDGL**       | 89.68 卤 0.24    | 86.03 卤 0.25 |  45.87 卤 0.58      | 47.10 卤 0.65     |  90.18 卤 0.27  |
 | **GRCN**       | 76.08 卤 0.27    | 59.31 卤 0.46 | 50.06 卤 0.38       | 44.41 卤 0.41     | 90.59 卤 0.37   |
 | **GAug(O)**    | 76.92 卤 0.34    | 61.98 卤 0.67 | 48.42 卤 0.39       | 52.74 卤 0.48     | 91.30 卤 0.23   |
 | **SLAPS**      | 91.73 卤 0.40    | 83.92 卤 0.63 | 40.97 卤 0.45       | 65.35 卤 0.45     | 89.09 卤 0.54   |
 | **GT**         | 70.70 卤 5.62    | 43.19 卤 6.53 | 48.55 卤 0.34       | 76.49 卤 0.80     | 90.26 卤 1.24   |
 | **Nodeformer** | 44.53 卤 22.62   | 67.14 卤 6.77 | 41.33 卤 1.25       | 56.54 卤 3.73     | 54.83 卤 4.43   |
 | **GEN**        | 90.48 卤 0.99    | 84.84 卤 0.81 | 49.17 卤 0.68       | --               | 91.15 卤 0.49   |
 | **CoGSL**      | --              | --           | --                 | --               | --             |
 | **SEGSL**      | 75.03 卤 0.28    | 60.59 卤 0.54 | --                 | --               | --             |
 | **SUBLIME**    | 95.29 卤 0.26    | 88.74 卤 0.29 | 44.49 卤 0.30       | 63.93 卤 0.27     | 76.10 卤 1.12   |
 | **STABLE**     | 71.84 卤 0.56    | 51.36 卤 1.24 | 48.36 卤 0.21       | 41.00 卤 1.18     | 80.46 卤 2.44   |
 
-## Add method
-
-There is an example of use your own GSL method.
-
-```python
-
-```
-
 ## How to Contribute
 As an active research topic, we are witenessing the rapid development of GSL methods.
 Hence, this project will be frequently updated and we welcome everyone interested in this topic to contribute! 
 
 Please feel free to send PR or issue!
 
 ## Citation
```

### Comparing `opengsl-0.0.1/README.md` & `opengsl-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,33 +29,35 @@
 ``` python
 import opengsl
 conf = opengsl.load_conf(method="gcn", dataset="cora")
 ```
 
 #### Step 2: Load data
 ``` python
-import opengsl.data
 dataset = opengsl.data.Dataset("cora", n_splits=1, feat_norm=conf.dataset['feat_norm'])
 ```
 
 #### Step 3: Build Model
 ``` python
-import opengsl.method
 solver = opengsl.method.gcn(conf,dataset)
 ```
 
 #### Step 4: Training and Evaluation
 ``` python
 exp = opengsl.ExpManager(solver, n_runs = 10)
 exp.run()
 ```
 
+## Add method
+if you want to use your own method, see `example.py` for detail.
+
+
 ## Node Classification Results
 | **Model**      | **Cora**     | **Citeseer** | **Pubmed**   | **Questions** | **Minesweeper** |
-|--------------|:------------:|:------------:|:------------:|:-------------:|:---------------:|
+|----------------|:------------:|:------------:|:------------:|:-------------:|:---------------:|
 | **GCN**        | 81.95 ± 0.62 | 71.34 ± 0.48 | 78.98 ± 0.35 | 75.80 ± 0.51  | 78.28 ± 0.44    |
 | **ProGNN**     | 80.27 ± 0.48 | 71.35 ± 0.42 | 79.39 ± 0.29 | --            | 51.43 ± 2.22    |
 | **IDGL**       | 84.19 ± 0.61 | 73.26 ± 0.53 | 82.78 ± 0.44 | 50.00 ± 0.00  | 50.00 ± 0.00    |
 | **GRCN**       | 84.61 ± 0.34 | 72.34 ± 0.73 | 79.30 ± 0.34 | 74.50 ± 0.84  | 72.57 ± 0.49    |
 | **GAug(O)**    | 83.43 ± 0.53 | 72.79 ± 0.86 | 78.73 ± 0.77 | --            | 77.93 ± 0.64    |
 | **SLAPS**      | 72.29 ± 1.01 | 70.00 ± 1.29 | 70.96 ± 0.99 | --            | 50.89 ± 1.72    |
 | **GT**         | 80.79 ± 1.14 | 68.50 ± 2.07 | 77.91 ± 0.58 | 75.36 ± 0.92  | 89.70 ± 0.28    |
@@ -64,37 +66,29 @@
 | **CoGSL**      | 81.46 ± 0.88 | 72.94 ± 0.71 | --           | --            | --              |
 | **SEGSL**      | 81.04 ± 1.07 | 71.57 ± 0.40 | 79.26 ± 0.67 | --            | --              |
 | **SUBLIME**    | 83.33 ± 0.73 | 72.44 ± 0.89 | 80.56 ± 1.32 | 67.21 ± 0.99  | 49.93 ± 1.36    |
 | **STABLE**     | 83.25 ± 0.86 | 70.99 ± 1.19 | 81.46 ± 0.78 | --            | 70.78 ± 0.27    |
 
 
 | **Model**      | **BlogCatalog** | **Flickr**   | **Amazon-ratings** | **Roman-empire** | **Wiki-cooc**  |
-|--------------|:---------------:|:------------:|:------------------:|:----------------:|:--------------:|
+|----------------|:---------------:|:------------:|:------------------:|:----------------:|:--------------:|
 | **GCN**        | 76.12 ± 0.42    | 61.60 ± 0.49 | 45.24 ± 0.29       | 70.41 ± 0.47     | 92.03 ± 0.19   |
 | **ProGNN**     | 73.38 ± 0.30    | 52.88 ± 0.76 | --                 | 56.21 ± 0.58     | 89.07 ± 5.59   |
 | **IDGL**       | 89.68 ± 0.24    | 86.03 ± 0.25 |  45.87 ± 0.58      | 47.10 ± 0.65     |  90.18 ± 0.27  |
 | **GRCN**       | 76.08 ± 0.27    | 59.31 ± 0.46 | 50.06 ± 0.38       | 44.41 ± 0.41     | 90.59 ± 0.37   |
 | **GAug(O)**    | 76.92 ± 0.34    | 61.98 ± 0.67 | 48.42 ± 0.39       | 52.74 ± 0.48     | 91.30 ± 0.23   |
 | **SLAPS**      | 91.73 ± 0.40    | 83.92 ± 0.63 | 40.97 ± 0.45       | 65.35 ± 0.45     | 89.09 ± 0.54   |
 | **GT**         | 70.70 ± 5.62    | 43.19 ± 6.53 | 48.55 ± 0.34       | 76.49 ± 0.80     | 90.26 ± 1.24   |
 | **Nodeformer** | 44.53 ± 22.62   | 67.14 ± 6.77 | 41.33 ± 1.25       | 56.54 ± 3.73     | 54.83 ± 4.43   |
 | **GEN**        | 90.48 ± 0.99    | 84.84 ± 0.81 | 49.17 ± 0.68       | --               | 91.15 ± 0.49   |
 | **CoGSL**      | --              | --           | --                 | --               | --             |
 | **SEGSL**      | 75.03 ± 0.28    | 60.59 ± 0.54 | --                 | --               | --             |
 | **SUBLIME**    | 95.29 ± 0.26    | 88.74 ± 0.29 | 44.49 ± 0.30       | 63.93 ± 0.27     | 76.10 ± 1.12   |
 | **STABLE**     | 71.84 ± 0.56    | 51.36 ± 1.24 | 48.36 ± 0.21       | 41.00 ± 1.18     | 80.46 ± 2.44   |
 
-## Add method
-
-There is an example of use your own GSL method.
-
-```python
-
-```
-
 ## How to Contribute
 As an active research topic, we are witenessing the rapid development of GSL methods.
 Hence, this project will be frequently updated and we welcome everyone interested in this topic to contribute! 
 
 Please feel free to send PR or issue!
 
 ## Citation
```

### Comparing `opengsl-0.0.1/opengsl/ExpManager.py` & `opengsl-0.0.2/opengsl/ExpManager.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/data/dataset.py` & `opengsl-0.0.2/opengsl/data/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from .pyg_load import pyg_load_dataset
 from .hetero_load import hetero_load
 from .split import get_split
 from ..utils.utils import normalize_feats
 import numpy as np
 from .homophily_control import get_new_adj
 import pickle
+import os
+import urllib.request
 
 
 class Dataset:
 
     def __init__(self, data, feat_norm=False, verbose=True, n_splits=1, homophily_control=None, path='./data/'):
         '''
         This class loads, preprocessed and splits data. The results are saved as "self.feats, self.adj, self.labels, self.train_masks, self.val_masks, self.test_masks".
@@ -63,15 +65,15 @@
             self.labels = self.labels.to(self.device)
             self.adj = self.adj.to(self.device)
             # normalize features
             if feat_norm:
                 self.feats = normalize_feats(self.feats)
 
         elif ds_name in ['amazon-ratings', 'questions', 'chameleon-filtered', 'squirrel-filtered', 'minesweeper', 'roman-empire', 'wiki-cooc']:
-            self.feats, self.adj, self.labels, self.splits = hetero_load(ds_name)
+            self.feats, self.adj, self.labels, self.splits = hetero_load(ds_name, path=self.path)
 
             self.feats = self.feats.to(self.device)
             self.labels = self.labels.to(self.device)
             self.adj = self.adj.to(self.device)
             self.n_nodes = self.feats.shape[0]
             self.dim_feats = self.feats.shape[1]
             self.n_edges = len(self.adj.coalesce().values())/2
@@ -108,16 +110,28 @@
         self.train_masks = []
         self.val_masks = []
         self.test_masks = []
         if self.name in ['blogcatalog', 'flickr']:
             def load_obj(file_name):
                 with open(file_name, 'rb') as f:
                     return pickle.load(f)
-
-            train_indices, val_indices, test_indices = load_obj('data/' + self.name + '_tvt_nids.pkl')
+            def download(name):
+                url = 'https://github.com/zhao-tong/GAug/raw/master/data/graphs/'
+                try:
+                    print('Downloading', url + name)
+                    urllib.request.urlretrieve(url + name, os.path.join(self.path, name))
+                    print('Done!')
+                except:
+                    raise Exception(
+                        '''Download failed! Make sure you have stable Internet connection and enter the right name''')
+
+            split_file = self.name + '_tvt_nids.pkl'
+            if not os.path.exists(os.path.join(self.path, split_file)):
+                download(split_file)
+            train_indices, val_indices, test_indices = load_obj(os.path.join(self.path, split_file))
             for i in range(n_splits):
                 self.train_masks.append(train_indices)
                 self.val_masks.append(val_indices)
                 self.test_masks.append(test_indices)
 
         elif self.name in ['coauthorcs', 'coauthorph', 'amazoncom', 'amazonpho']:
             for i in range(n_splits):
```

### Comparing `opengsl-0.0.1/opengsl/data/homophily_control.py` & `opengsl-0.0.2/opengsl/data/homophily_control.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/data/split.py` & `opengsl-0.0.2/opengsl/data/split.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/load_conf.py` & `opengsl-0.0.2/opengsl/load_conf.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/__init__.py` & `opengsl-0.0.2/opengsl/method/__init__.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/gnnsolver.py` & `opengsl-0.0.2/opengsl/method/gnnsolver.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/gslsolver.py` & `opengsl-0.0.2/opengsl/method/gslsolver.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/cogsl.py` & `opengsl-0.0.2/opengsl/method/models/cogsl.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/gaug.py` & `opengsl-0.0.2/opengsl/method/models/gaug.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/gcn.py` & `opengsl-0.0.2/opengsl/method/models/gcn.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/gcn_idgl.py` & `opengsl-0.0.2/opengsl/method/models/gcn_idgl.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/gen.py` & `opengsl-0.0.2/opengsl/method/models/gen.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/gnn_modules.py` & `opengsl-0.0.2/opengsl/method/models/gnn_modules.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/grcn.py` & `opengsl-0.0.2/opengsl/method/models/grcn.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/gt.py` & `opengsl-0.0.2/opengsl/method/models/gt.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/idgl.py` & `opengsl-0.0.2/opengsl/method/models/idgl.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/jknet.py` & `opengsl-0.0.2/opengsl/method/models/jknet.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/nodeformer.py` & `opengsl-0.0.2/opengsl/method/models/nodeformer.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/prognn.py` & `opengsl-0.0.2/opengsl/method/models/prognn.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/segsl.py` & `opengsl-0.0.2/opengsl/method/models/segsl.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/slaps.py` & `opengsl-0.0.2/opengsl/method/models/slaps.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/stable.py` & `opengsl-0.0.2/opengsl/method/models/stable.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/models/sublime.py` & `opengsl-0.0.2/opengsl/method/models/sublime.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/method/solver.py` & `opengsl-0.0.2/opengsl/method/solver.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/utils/logger.py` & `opengsl-0.0.2/opengsl/utils/logger.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/utils/recorder.py` & `opengsl-0.0.2/opengsl/utils/recorder.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl/utils/utils.py` & `opengsl-0.0.2/opengsl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/opengsl.egg-info/PKG-INFO` & `opengsl-0.0.2/opengsl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengsl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A comprehensive benchmark for Graph Structure Learning.
 Home-page: https://github.com/OpenGSL/OpenGSL
 Author: Zhiyao Zhou, Sheng Zhou, Bochao Mao, Xuanyi Zhou
 Keywords: AI,GNN,graph structure learning
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -46,33 +46,35 @@
 ``` python
 import opengsl
 conf = opengsl.load_conf(method="gcn", dataset="cora")
 ```
 
 #### Step 2: Load data
 ``` python
-import opengsl.data
 dataset = opengsl.data.Dataset("cora", n_splits=1, feat_norm=conf.dataset['feat_norm'])
 ```
 
 #### Step 3: Build Model
 ``` python
-import opengsl.method
 solver = opengsl.method.gcn(conf,dataset)
 ```
 
 #### Step 4: Training and Evaluation
 ``` python
 exp = opengsl.ExpManager(solver, n_runs = 10)
 exp.run()
 ```
 
+## Add method
+if you want to use your own method, see `example.py` for detail.
+
+
 ## Node Classification Results
 | **Model**      | **Cora**     | **Citeseer** | **Pubmed**   | **Questions** | **Minesweeper** |
-|--------------|:------------:|:------------:|:------------:|:-------------:|:---------------:|
+|----------------|:------------:|:------------:|:------------:|:-------------:|:---------------:|
 | **GCN**        | 81.95 卤 0.62 | 71.34 卤 0.48 | 78.98 卤 0.35 | 75.80 卤 0.51  | 78.28 卤 0.44    |
 | **ProGNN**     | 80.27 卤 0.48 | 71.35 卤 0.42 | 79.39 卤 0.29 | --            | 51.43 卤 2.22    |
 | **IDGL**       | 84.19 卤 0.61 | 73.26 卤 0.53 | 82.78 卤 0.44 | 50.00 卤 0.00  | 50.00 卤 0.00    |
 | **GRCN**       | 84.61 卤 0.34 | 72.34 卤 0.73 | 79.30 卤 0.34 | 74.50 卤 0.84  | 72.57 卤 0.49    |
 | **GAug(O)**    | 83.43 卤 0.53 | 72.79 卤 0.86 | 78.73 卤 0.77 | --            | 77.93 卤 0.64    |
 | **SLAPS**      | 72.29 卤 1.01 | 70.00 卤 1.29 | 70.96 卤 0.99 | --            | 50.89 卤 1.72    |
 | **GT**         | 80.79 卤 1.14 | 68.50 卤 2.07 | 77.91 卤 0.58 | 75.36 卤 0.92  | 89.70 卤 0.28    |
@@ -81,37 +83,29 @@
 | **CoGSL**      | 81.46 卤 0.88 | 72.94 卤 0.71 | --           | --            | --              |
 | **SEGSL**      | 81.04 卤 1.07 | 71.57 卤 0.40 | 79.26 卤 0.67 | --            | --              |
 | **SUBLIME**    | 83.33 卤 0.73 | 72.44 卤 0.89 | 80.56 卤 1.32 | 67.21 卤 0.99  | 49.93 卤 1.36    |
 | **STABLE**     | 83.25 卤 0.86 | 70.99 卤 1.19 | 81.46 卤 0.78 | --            | 70.78 卤 0.27    |
 
 
 | **Model**      | **BlogCatalog** | **Flickr**   | **Amazon-ratings** | **Roman-empire** | **Wiki-cooc**  |
-|--------------|:---------------:|:------------:|:------------------:|:----------------:|:--------------:|
+|----------------|:---------------:|:------------:|:------------------:|:----------------:|:--------------:|
 | **GCN**        | 76.12 卤 0.42    | 61.60 卤 0.49 | 45.24 卤 0.29       | 70.41 卤 0.47     | 92.03 卤 0.19   |
 | **ProGNN**     | 73.38 卤 0.30    | 52.88 卤 0.76 | --                 | 56.21 卤 0.58     | 89.07 卤 5.59   |
 | **IDGL**       | 89.68 卤 0.24    | 86.03 卤 0.25 |  45.87 卤 0.58      | 47.10 卤 0.65     |  90.18 卤 0.27  |
 | **GRCN**       | 76.08 卤 0.27    | 59.31 卤 0.46 | 50.06 卤 0.38       | 44.41 卤 0.41     | 90.59 卤 0.37   |
 | **GAug(O)**    | 76.92 卤 0.34    | 61.98 卤 0.67 | 48.42 卤 0.39       | 52.74 卤 0.48     | 91.30 卤 0.23   |
 | **SLAPS**      | 91.73 卤 0.40    | 83.92 卤 0.63 | 40.97 卤 0.45       | 65.35 卤 0.45     | 89.09 卤 0.54   |
 | **GT**         | 70.70 卤 5.62    | 43.19 卤 6.53 | 48.55 卤 0.34       | 76.49 卤 0.80     | 90.26 卤 1.24   |
 | **Nodeformer** | 44.53 卤 22.62   | 67.14 卤 6.77 | 41.33 卤 1.25       | 56.54 卤 3.73     | 54.83 卤 4.43   |
 | **GEN**        | 90.48 卤 0.99    | 84.84 卤 0.81 | 49.17 卤 0.68       | --               | 91.15 卤 0.49   |
 | **CoGSL**      | --              | --           | --                 | --               | --             |
 | **SEGSL**      | 75.03 卤 0.28    | 60.59 卤 0.54 | --                 | --               | --             |
 | **SUBLIME**    | 95.29 卤 0.26    | 88.74 卤 0.29 | 44.49 卤 0.30       | 63.93 卤 0.27     | 76.10 卤 1.12   |
 | **STABLE**     | 71.84 卤 0.56    | 51.36 卤 1.24 | 48.36 卤 0.21       | 41.00 卤 1.18     | 80.46 卤 2.44   |
 
-## Add method
-
-There is an example of use your own GSL method.
-
-```python
-
-```
-
 ## How to Contribute
 As an active research topic, we are witenessing the rapid development of GSL methods.
 Hence, this project will be frequently updated and we welcome everyone interested in this topic to contribute! 
 
 Please feel free to send PR or issue!
 
 ## Citation
```

### Comparing `opengsl-0.0.1/opengsl.egg-info/SOURCES.txt` & `opengsl-0.0.2/opengsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.1/setup.py` & `opengsl-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,28 +12,27 @@
 numba
 torch
 torch_geometric
 torch_sparse
 dgl-cu115
 """
 
-
 def get_install_requires():
     reqs = [req for req in REQUIRES.split("\n") if len(req) > 0]
     return reqs
 
 
 with open("README.md") as f:
     readme = f.read()
 
 
 def do_setup():
     setup(
         name="opengsl",
-        version="0.0.1",
+        version="0.0.2",
         description="A comprehensive benchmark for Graph Structure Learning.",
         url="https://github.com/OpenGSL/OpenGSL",
         author='Zhiyao Zhou, Sheng Zhou, Bochao Mao, Xuanyi Zhou',
         long_description=readme,
         long_description_content_type="text/markdown",
         install_requires=get_install_requires(),
         python_requires=">=3.7.0",
```

