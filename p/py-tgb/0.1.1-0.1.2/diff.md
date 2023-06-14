# Comparing `tmp/py_tgb-0.1.1.tar.gz` & `tmp/py_tgb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tgb-0.1.1.tar", max compression
+gzip compressed data, was "py_tgb-0.1.2.tar", max compression
```

## Comparing `py_tgb-0.1.1.tar` & `py_tgb-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1905 2023-06-12 18:33:10.179693 py_tgb-0.1.1/README.md
--rw-r--r--   0        0        0      703 2023-06-12 19:25:39.195693 py_tgb-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      177 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/MAG/mag.py
--rw-r--r--   0        0        0      820 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/MAG/old/plot_stats.py
--rw-r--r--   0        0        0     4777 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/amazonreview/amazonreview.py
--rw-r--r--   0        0        0     2499 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/amazonreview/amazonreview_neg_generator.py
--rw-r--r--   0        0        0     7781 2023-06-12 18:33:10.199693 py_tgb-0.1.1/tgb/datasets/flight_raw/opensky.py
--rw-r--r--   0        0        0    19780 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/lastfmGenre/lastfm.py
--rw-r--r--   0        0        0     2518 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/opensky/opensky_neg_generator.py
--rw-r--r--   0        0        0     6912 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/redditcomments/redditcomments.py
--rw-r--r--   0        0        0     2501 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/redditcomments/redditcomments_neg_generator.py
--rw-r--r--   0        0        0     4740 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/stablecoin/stablecoin.py
--rw-r--r--   0        0        0     2497 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/stablecoin/stablecoin_neg_generator.py
--rw-r--r--   0        0        0    11859 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/subreddits/subreddits.py
--rw-r--r--   0        0        0     5927 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/datasets/un_trade/un_trade.py
--rw-r--r--   0        0        0    14106 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/edgeregression/dataset.py
--rw-r--r--   0        0        0     3992 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/edgeregression/dataset_pyg.py
--rw-r--r--   0        0        0     5087 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/edgeregression/evaluate.py
--rw-r--r--   0        0        0    13856 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/linkproppred/dataset.py
--rw-r--r--   0        0        0     7293 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/linkproppred/dataset_pyg.py
--rw-r--r--   0        0        0     4664 2023-06-12 18:33:10.203693 py_tgb-0.1.1/tgb/linkproppred/evaluate.py
--rw-r--r--   0        0        0    10770 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/linkproppred/negative_generator.py
--rw-r--r--   0        0        0     3903 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/linkproppred/negative_sampler.py
--rw-r--r--   0        0        0    16249 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/nodeproppred/dataset.py
--rw-r--r--   0        0        0     7205 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/nodeproppred/dataset_pyg.py
--rw-r--r--   0        0        0     5334 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/nodeproppred/evaluate.py
--rw-r--r--   0        0        0     1683 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/utils/info.py
--rw-r--r--   0        0        0    27787 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/utils/pre_process.py
--rw-r--r--   0        0        0     2905 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/utils/stats.py
--rw-r--r--   0        0        0     2974 2023-06-12 18:33:10.207693 py_tgb-0.1.1/tgb/utils/utils.py
--rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 py_tgb-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2218 2023-06-14 13:49:29.647098 py_tgb-0.1.2/README.md
+-rw-r--r--   0        0        0      748 2023-06-14 13:49:29.647098 py_tgb-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-06-14 13:49:29.647098 py_tgb-0.1.2/tgb/datasets/MAG/mag.py
+-rw-r--r--   0        0        0      820 2023-06-14 13:49:29.647098 py_tgb-0.1.2/tgb/datasets/MAG/old/plot_stats.py
+-rw-r--r--   0        0        0     4777 2023-06-14 13:49:29.647098 py_tgb-0.1.2/tgb/datasets/amazonreview/amazonreview.py
+-rw-r--r--   0        0        0     2499 2023-06-14 13:49:29.647098 py_tgb-0.1.2/tgb/datasets/amazonreview/amazonreview_neg_generator.py
+-rw-r--r--   0        0        0     7781 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/datasets/flight_raw/opensky.py
+-rw-r--r--   0        0        0    19780 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/datasets/lastfmgenre/lastfm.py
+-rw-r--r--   0        0        0     2518 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/datasets/opensky/opensky_neg_generator.py
+-rw-r--r--   0        0        0     6912 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/datasets/redditcomments/redditcomments.py
+-rw-r--r--   0        0        0     2501 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/datasets/redditcomments/redditcomments_neg_generator.py
+-rw-r--r--   0        0        0     4740 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/datasets/stablecoin/stablecoin.py
+-rw-r--r--   0        0        0     2497 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/datasets/stablecoin/stablecoin_neg_generator.py
+-rw-r--r--   0        0        0    11859 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/datasets/subreddits/subreddits.py
+-rw-r--r--   0        0        0     5927 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/datasets/un_trade/un_trade.py
+-rw-r--r--   0        0        0    14106 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/edgeregression/dataset.py
+-rw-r--r--   0        0        0     3992 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/edgeregression/dataset_pyg.py
+-rw-r--r--   0        0        0     5087 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/edgeregression/evaluate.py
+-rw-r--r--   0        0        0    13856 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/linkproppred/dataset.py
+-rw-r--r--   0        0        0     7293 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/linkproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     4664 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/linkproppred/evaluate.py
+-rw-r--r--   0        0        0    10770 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/linkproppred/negative_generator.py
+-rw-r--r--   0        0        0     3903 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/linkproppred/negative_sampler.py
+-rw-r--r--   0        0        0    16249 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/nodeproppred/dataset.py
+-rw-r--r--   0        0        0     7205 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/nodeproppred/dataset_pyg.py
+-rw-r--r--   0        0        0     5334 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/nodeproppred/evaluate.py
+-rw-r--r--   0        0        0     8689 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/utils/dataset_stats.py
+-rw-r--r--   0        0        0     1683 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/utils/info.py
+-rw-r--r--   0        0        0    27787 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/utils/pre_process.py
+-rw-r--r--   0        0        0     2970 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/utils/stats.py
+-rw-r--r--   0        0        0     2974 2023-06-14 13:49:29.651098 py_tgb-0.1.2/tgb/utils/utils.py
+-rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 py_tgb-0.1.2/PKG-INFO
```

### Comparing `py_tgb-0.1.1/README.md` & `py_tgb-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 # TGB
 Temporal Graph Benchmark project repo 
 
+### Pypi Install
+
+You can install TGB via [pip](https://pypi.org/project/py-tgb/)
+```
+pip install py-tgb
+```
+
+### Dataset Download
+
+all dataset download links can be found at [info.py](https://github.com/shenyangHuang/TGB/blob/main/tgb/utils/info.py)
+
+TGB dataloader will also automatically download the dataset
+
 ### Install dependency
 Our implementation works with python >= 3.9 and can be installed as follows
 
 1. set up virtual environment (conda should work as well)
 ```
 python -m venv ~/tgb_env/
 source ~/tgb_env/bin/activate
```

### Comparing `py_tgb-0.1.1/pyproject.toml` & `py_tgb-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "py-tgb"
-version = "0.1.1"
+version = "0.1.2"
 description = "Temporal Graph Benchmark project repo"
 authors = ["shenyang Huang <shenyang.huang@mail.mcgill.ca>", "Farimah Poursafaei", "Emanuele Rossi <emanuele.rossi1909@gmail.com>", "Jacob Danovitch <jacob.danovitch@mila.quebec>"]
 readme = "README.md"
 packages = [{include = "tgb"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 torch-geometric = "^2.3.0"
 tqdm = "^4.65.0"
 clint = "^0.5.1"
 requests = "^2.28.2"
+pandas = "^1.5.3"
 scikit-learn = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.15"
 mkdocstrings-python = "^1.1.2"
+mkdocs-jupyter = "^0.24.1"
 poetry = "^1.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py_tgb-0.1.1/tgb/datasets/MAG/old/plot_stats.py` & `py_tgb-0.1.2/tgb/datasets/MAG/old/plot_stats.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/amazonreview/amazonreview.py` & `py_tgb-0.1.2/tgb/datasets/amazonreview/amazonreview.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/amazonreview/amazonreview_neg_generator.py` & `py_tgb-0.1.2/tgb/datasets/amazonreview/amazonreview_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/flight_raw/opensky.py` & `py_tgb-0.1.2/tgb/datasets/flight_raw/opensky.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/lastfmGenre/lastfm.py` & `py_tgb-0.1.2/tgb/datasets/lastfmgenre/lastfm.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/opensky/opensky_neg_generator.py` & `py_tgb-0.1.2/tgb/datasets/opensky/opensky_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/redditcomments/redditcomments.py` & `py_tgb-0.1.2/tgb/datasets/redditcomments/redditcomments.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/redditcomments/redditcomments_neg_generator.py` & `py_tgb-0.1.2/tgb/datasets/redditcomments/redditcomments_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/stablecoin/stablecoin.py` & `py_tgb-0.1.2/tgb/datasets/stablecoin/stablecoin.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/stablecoin/stablecoin_neg_generator.py` & `py_tgb-0.1.2/tgb/datasets/stablecoin/stablecoin_neg_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/subreddits/subreddits.py` & `py_tgb-0.1.2/tgb/datasets/subreddits/subreddits.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/datasets/un_trade/un_trade.py` & `py_tgb-0.1.2/tgb/datasets/un_trade/un_trade.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/edgeregression/dataset.py` & `py_tgb-0.1.2/tgb/edgeregression/dataset.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/edgeregression/dataset_pyg.py` & `py_tgb-0.1.2/tgb/edgeregression/dataset_pyg.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/edgeregression/evaluate.py` & `py_tgb-0.1.2/tgb/edgeregression/evaluate.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/linkproppred/dataset.py` & `py_tgb-0.1.2/tgb/linkproppred/dataset.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/linkproppred/dataset_pyg.py` & `py_tgb-0.1.2/tgb/linkproppred/dataset_pyg.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/linkproppred/evaluate.py` & `py_tgb-0.1.2/tgb/linkproppred/evaluate.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/linkproppred/negative_generator.py` & `py_tgb-0.1.2/tgb/linkproppred/negative_generator.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/linkproppred/negative_sampler.py` & `py_tgb-0.1.2/tgb/linkproppred/negative_sampler.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/nodeproppred/dataset.py` & `py_tgb-0.1.2/tgb/nodeproppred/dataset.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/nodeproppred/dataset_pyg.py` & `py_tgb-0.1.2/tgb/nodeproppred/dataset_pyg.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/nodeproppred/evaluate.py` & `py_tgb-0.1.2/tgb/nodeproppred/evaluate.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/utils/info.py` & `py_tgb-0.1.2/tgb/utils/info.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/utils/pre_process.py` & `py_tgb-0.1.2/tgb/utils/pre_process.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/tgb/utils/stats.py` & `py_tgb-0.1.2/tgb/utils/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 script for generating statistics from the dataset
 """
 import csv
 import numpy as np
-import matplotlib.pyplot as plt
+# import matplotlib.pyplot as plt
 
 
 """
 #! analyze statistics from the dataset
 #* 1). # of unique nodes, 2). # of edges. 3). # of unique edges, 4). # of timestamps 5). recurrence of nodes
 """
 
@@ -88,13 +88,14 @@
     plt.savefig(outname + ".pdf")
     plt.close()
 
 
 def main():
     # fname = "../datasets/flight_raw/opensky/opensky_edgelist.csv"
     # fname = "../datasets/lastfmgenre/lastfmgenre_raw/lastfmgenre_edgelist.csv"
-    fname = "../datasets/redditcomments/redditcomments_edgelist.csv"
+    # fname = "../datasets/redditcomments/redditcomments_edgelist.csv"
+    fname = "tgb/datasets/wikipedia/wikipedia_edgelist.csv"
     analyze_csv(fname)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `py_tgb-0.1.1/tgb/utils/utils.py` & `py_tgb-0.1.2/tgb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `py_tgb-0.1.1/PKG-INFO` & `py_tgb-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 Metadata-Version: 2.1
 Name: py-tgb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Temporal Graph Benchmark project repo
 Author: shenyang Huang
 Author-email: shenyang.huang@mail.mcgill.ca
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clint (>=0.5.1,<0.6.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: torch-geometric (>=2.3.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # TGB
 Temporal Graph Benchmark project repo 
 
+### Pypi Install
+
+You can install TGB via [pip](https://pypi.org/project/py-tgb/)
+```
+pip install py-tgb
+```
+
+### Dataset Download
+
+all dataset download links can be found at [info.py](https://github.com/shenyangHuang/TGB/blob/main/tgb/utils/info.py)
+
+TGB dataloader will also automatically download the dataset
+
 ### Install dependency
 Our implementation works with python >= 3.9 and can be installed as follows
 
 1. set up virtual environment (conda should work as well)
 ```
 python -m venv ~/tgb_env/
 source ~/tgb_env/bin/activate
```

