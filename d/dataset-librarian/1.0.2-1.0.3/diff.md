# Comparing `tmp/dataset_librarian-1.0.2.tar.gz` & `tmp/dataset_librarian-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_librarian-1.0.2.tar", last modified: Mon Jun  5 19:36:02 2023, max compression
+gzip compressed data, was "dataset_librarian-1.0.3.tar", last modified: Tue Jun 13 22:19:36 2023, max compression
```

## Comparing `dataset_librarian-1.0.2.tar` & `dataset_librarian-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3975 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3424 2023-06-05 18:22:53.000000 dataset_librarian-1.0.2/README.md
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      805 2023-06-05 19:35:51.000000 dataset_librarian-1.0.2/pyproject.toml
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/setup.cfg
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.224434 dataset_librarian-1.0.2/src/
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.224434 dataset_librarian-1.0.2/src/dataset_librarian/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3944 2023-05-23 13:31:26.000000 dataset_librarian-1.0.2/src/dataset_librarian/dataset.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.224434 dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2302 2023-05-18 18:37:10.000000 dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/download.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3484 2023-05-18 18:37:04.000000 dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/preprocess.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2425 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/datasets_urls.json
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/src/dataset_librarian/scripts/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/__init__.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     7804 2023-06-05 18:23:21.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/create_data_split.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     8135 2023-06-01 04:54:09.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/prepare_nlp_data.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)    10700 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/prepare_vision_data.py
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.228434 dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/__init__.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2746 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/csv_generator_mvtec.py
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     1928 2023-05-18 18:00:22.000000 dataset_librarian-1.0.2/src/dataset_librarian/terms_and_conditions.txt
-drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-05 19:36:02.224434 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3975 2023-06-05 19:36:01.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/PKG-INFO
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      939 2023-06-05 19:36:02.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/SOURCES.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-06-05 19:36:01.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/dependency_links.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       77 2023-06-05 19:36:01.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/requires.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       18 2023-06-05 19:36:01.000000 dataset_librarian-1.0.2/src/dataset_librarian.egg-info/top_level.txt
--rw-r--r--   0 mapineda (12146662) mlp_labs (21495)   102383 2023-06-05 18:22:53.000000 dataset_librarian-1.0.2/third-party-programs.txt
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-13 22:19:36.543260 dataset_librarian-1.0.3/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     4069 2023-06-13 22:19:36.543260 dataset_librarian-1.0.3/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3518 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/README.md
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      805 2023-06-13 22:17:46.000000 dataset_librarian-1.0.3/pyproject.toml
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       38 2023-06-13 22:19:36.543260 dataset_librarian-1.0.3/setup.cfg
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-13 22:19:36.539260 dataset_librarian-1.0.3/src/
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-13 22:19:36.539260 dataset_librarian-1.0.3/src/dataset_librarian/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     4065 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/dataset.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-13 22:19:36.543260 dataset_librarian-1.0.3/src/dataset_librarian/dataset_api/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/dataset_api/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2302 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/dataset_api/download.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     3870 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/dataset_api/preprocess.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2425 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/datasets_urls.json
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-13 22:19:36.543260 dataset_librarian-1.0.3/src/dataset_librarian/scripts/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/scripts/__init__.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-13 22:19:36.543260 dataset_librarian-1.0.3/src/dataset_librarian/scripts/brca/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/scripts/brca/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     7744 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/scripts/brca/create_data_split.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     8134 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/scripts/brca/prepare_nlp_data.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)    10652 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/scripts/brca/prepare_vision_data.py
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-13 22:19:36.543260 dataset_librarian-1.0.3/src/dataset_librarian/scripts/mvtec-ad/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      617 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/scripts/mvtec-ad/__init__.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     2746 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/scripts/mvtec-ad/csv_generator_mvtec.py
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     1928 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/src/dataset_librarian/terms_and_conditions.txt
+drwxr-sr-x   0 mapineda (12146662) mlp_labs (21495)        0 2023-06-13 22:19:36.539260 dataset_librarian-1.0.3/src/dataset_librarian.egg-info/
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)     4069 2023-06-13 22:19:35.000000 dataset_librarian-1.0.3/src/dataset_librarian.egg-info/PKG-INFO
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)      939 2023-06-13 22:19:36.000000 dataset_librarian-1.0.3/src/dataset_librarian.egg-info/SOURCES.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)        1 2023-06-13 22:19:35.000000 dataset_librarian-1.0.3/src/dataset_librarian.egg-info/dependency_links.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       77 2023-06-13 22:19:35.000000 dataset_librarian-1.0.3/src/dataset_librarian.egg-info/requires.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)       18 2023-06-13 22:19:35.000000 dataset_librarian-1.0.3/src/dataset_librarian.egg-info/top_level.txt
+-rw-r--r--   0 mapineda (12146662) mlp_labs (21495)   102383 2023-06-13 22:07:46.000000 dataset_librarian-1.0.3/third-party-programs.txt
```

### Comparing `dataset_librarian-1.0.2/PKG-INFO` & `dataset_librarian-1.0.3/src/dataset_librarian.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dataset_librarian
-Version: 1.0.2
+Name: dataset-librarian
+Version: 1.0.3
 Summary: Dataset librarian is a tool to download and apply the preprocessing needed for the list of supported datasets
 Author-email: IntelAI <IntelAI@intel.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
@@ -18,29 +18,30 @@
 python -m pip install dataset-librarian
 ```
 For more information check the [dataset-librarian PyPI package](https://pypi.org/project/dataset-librarian/)
 
 ## Datasets
 | Dataset name | Description | Download | Preprocessing | command |
 | ------------ | ----------- | -------- | --------------| ------- |
-| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory>` |
+| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory> --split_ratio 0.1` |
 | `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python -m dataset_librarian.dataset -n tabformer --download` |
 | `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python -m dataset_librarian.dataset -n dureader-vis --download` |
 | `msmarco` | [MS MARCO](https://microsoft.github.io/msmarco/)  is a collection of datasets focused on deep learning in search | supported | not supported | `python -m dataset_librarian.dataset -n msmarco --download` |
 | `mvtec-ad` | [MVTEC Anomaly Detection DATASET](https://www.mvtec.com/company/research/datasets/mvtec-ad) for industrial inspection. It contains over 5000 high-resolution images divided into fifteen different object and texture categories. | supported | supported  | `python -m dataset_librarian.dataset -n mvtec-ad --download --preprocess -d <path to the dataset directory>` |
 
 ## Command-line Interface
 
 | Input Arguments | Description |
 | --------------- | ----------- |
 | --list (-l) | list the supported datasets. |
 | --name (-n) | dataset name |
 | --directory (-d) | directory location where the raw dataset will be saved on your system. It's also where the preprocessed dataset files will be written. If not set, a directory with the dataset name will be created. |
 | --download | download the dataset specified. |
 | --preprocess | preprocess the dataset if supported. |
+| --split_ratio | split ratio of the test data, the default value is 0.1. |
 
 
 ## Python API
 ```
 from dataset_librarian.dataset_api.download import download_dataset
 from dataset_librarian.dataset_api.preprocess import preprocess_dataset
```

### Comparing `dataset_librarian-1.0.2/README.md` & `dataset_librarian-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 python -m pip install dataset-librarian
 ```
 For more information check the [dataset-librarian PyPI package](https://pypi.org/project/dataset-librarian/)
 
 ## Datasets
 | Dataset name | Description | Download | Preprocessing | command |
 | ------------ | ----------- | -------- | --------------| ------- |
-| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory>` |
+| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory> --split_ratio 0.1` |
 | `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python -m dataset_librarian.dataset -n tabformer --download` |
 | `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python -m dataset_librarian.dataset -n dureader-vis --download` |
 | `msmarco` | [MS MARCO](https://microsoft.github.io/msmarco/)  is a collection of datasets focused on deep learning in search | supported | not supported | `python -m dataset_librarian.dataset -n msmarco --download` |
 | `mvtec-ad` | [MVTEC Anomaly Detection DATASET](https://www.mvtec.com/company/research/datasets/mvtec-ad) for industrial inspection. It contains over 5000 high-resolution images divided into fifteen different object and texture categories. | supported | supported  | `python -m dataset_librarian.dataset -n mvtec-ad --download --preprocess -d <path to the dataset directory>` |
 
 ## Command-line Interface
 
 | Input Arguments | Description |
 | --------------- | ----------- |
 | --list (-l) | list the supported datasets. |
 | --name (-n) | dataset name |
 | --directory (-d) | directory location where the raw dataset will be saved on your system. It's also where the preprocessed dataset files will be written. If not set, a directory with the dataset name will be created. |
 | --download | download the dataset specified. |
 | --preprocess | preprocess the dataset if supported. |
+| --split_ratio | split ratio of the test data, the default value is 0.1. |
 
 
 ## Python API
 ```
 from dataset_librarian.dataset_api.download import download_dataset
 from dataset_librarian.dataset_api.preprocess import preprocess_dataset
```

### Comparing `dataset_librarian-1.0.2/pyproject.toml` & `dataset_librarian-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset_librarian"
-version = "1.0.2"
+version = "1.0.3"
 requires-python = ">=3.9,<3.11"
 authors = [
     { name="IntelAI", email="IntelAI@intel.com"}
 ]
 description = "Dataset librarian is a tool to download and apply the preprocessing needed for the list of supported datasets"
 readme = "README.md"
 classifiers = [
```

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/__init__.py` & `dataset_librarian-1.0.3/src/dataset_librarian/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/dataset.py` & `dataset_librarian-1.0.3/src/dataset_librarian/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,25 +65,26 @@
     # Create the parser for the CLI
     parser = argparse.ArgumentParser(description='Download and preprocess datasets')
     parser.add_argument('-n', '--name', type=str, help='name of the dataset to download')
     parser.add_argument('-l', '--list', action='store_true', help='list the supported datasets')
     parser.add_argument('-d', '--directory', type=str, help='the desired dataset directory location')
     parser.add_argument('--download', action='store_true', help='download the raw dataset')
     parser.add_argument('--preprocess', action='store_true', help='preprocess the dataset')
+    parser.add_argument('--split_ratio', type=float, help="split ratio of the test data", default=0.1)
 
     # Parse the command-line arguments
     args = parser.parse_args()
 
     # Download the dataset if the --download flag is true
     if args.download:
         download_dataset(args.name, args.directory)
 
     # Preprocess the dataset if the --preprocess flag is true
     if args.preprocess:
-        preprocess_dataset(args.name, args.directory)
+        preprocess_dataset(args.name, args.directory, args.split_ratio)
 
     # List the supported datasets if the --list flag is true
     if args.list:
         datasets = pkg_resources.resource_filename('dataset_librarian', 'datasets_urls.json')
         with open(datasets) as f: 
             datasets = json.load(f)
         # Get the list of keys
```

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/__init__.py` & `dataset_librarian-1.0.3/src/dataset_librarian/dataset_api/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/download.py` & `dataset_librarian-1.0.3/src/dataset_librarian/dataset_api/download.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/dataset_api/preprocess.py` & `dataset_librarian-1.0.3/src/dataset_librarian/dataset_api/preprocess.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import json
 import os
 import sys
 import signal
 import subprocess
 import pkg_resources
 
-def preprocess_dataset(dataset_name, dataset_directory):
+def preprocess_dataset(dataset_name, dataset_directory, split_ratio):
     # Get the path to the file relative to the package root
     datasets = pkg_resources.resource_filename('dataset_librarian', 'datasets_urls.json')
     # Load the JSON file that contains the dataset URLs
     with open(datasets, 'r') as f:
         dataset_urls = json.load(f)
 
     # Check if the dataset name is in the JSON file
@@ -48,18 +48,24 @@
     datasets_api_path = os.path.dirname(os.path.realpath(__file__))
     scripts_path = os.path.join(datasets_api_path, os.pardir, 'scripts')
 
     if dataset_name == "brca":
         brca_scripts = os.path.join(scripts_path, dataset_name)
         nlp_data_script = os.path.join(brca_scripts, 'prepare_nlp_data.py')
         vision_data_script = os.path.join(brca_scripts, 'prepare_vision_data.py')
+        nlp_split_data = os.path.join(brca_scripts, 'create_data_split.py')
+        vision_split_data = os.path.join(brca_scripts, 'create_data_split.py')
         # Run dataset preprocessing scripts
         _launch_command(["python", nlp_data_script])
         _launch_command(["python", vision_data_script])
 
+        # Split the pre-processed data:
+        _launch_command(["python", nlp_split_data, "--split_ratio", str(split_ratio)])
+        _launch_command(["python", vision_split_data, "--split_ratio", str(split_ratio)])
+
     elif dataset_name == "mvtec-ad":
         raw_datset = os.path.join( dataset_directory, "mvtec_anomaly_detection.tar.xz")
         if os.path.exists(raw_datset):
             # extract dataset files
             subprocess.run(["tar", "-xf", raw_datset, "--directory", dataset_directory])
         elif not os.listdir(dataset_directory):
             print("\nError: No datasets found in {}.\n".format(dataset_directory))
```

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/datasets_urls.json` & `dataset_librarian-1.0.3/src/dataset_librarian/datasets_urls.json`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/scripts/__init__.py` & `dataset_librarian-1.0.3/src/dataset_librarian/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/__init__.py` & `dataset_librarian-1.0.3/src/dataset_librarian/scripts/brca/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/create_data_split.py` & `dataset_librarian-1.0.3/src/dataset_librarian/scripts/brca/create_data_split.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+import os
 import shutil
 import numpy as np
 import argparse
 
 from os import path, listdir
 from pandas import DataFrame, read_csv
 from typing import List, Tuple
 from sklearn.model_selection import train_test_split
 from pathlib import Path
 
-root_folder = path.dirname(path.abspath(__file__))
+root_folder = os.environ.get('DATASET_DIR')
 
 
 def get_subject_id(image_name):
     """
     Extracts the patient ID from an image filename.
 
     Args:
@@ -171,42 +172,42 @@
         description="This function create testing and training data for Breast Cancer prediction."
     )
 
     parser.add_argument(
         "--annotation_file",
         type=str,
         help="Location of annotation file.",
-        default=path.join(root_folder, "../../../../../data/annotation/annotation.csv")
+        default=os.path.join(root_folder, "annotation", "annotation.csv")
     )
     
     parser.add_argument(
         "--target_annotation_folder",
         type=str,
         help="Location of target annotation folder.",
-        default=path.join(root_folder,"../../../../../data/annotation")
+        default=os.path.join(root_folder, "annotation")
     )
     
     parser.add_argument(
         "--segmented_image_folder",
         type=str,
         help="Location of segmented image folder.",
-        default=path.join(root_folder,"../../../../../data/segmented_images")
+        default=os.path.join(root_folder, "segmented_images")
     )
     
     parser.add_argument(
         "--target_image_folder",
         type=str,
         help="Location of target imagefolder for train and test images.",
-        default=path.join(root_folder,"../../../../../data/train_test_split_images")
+        default=os.path.join(root_folder, "train_test_split_images")
     )
     
     parser.add_argument(
         "--split_ratio",
         type=float,
-        help="split ration of the test data.",
+        help="split ratio of the test data.",
         default=0.1,
     )
 
     params = parser.parse_args()
     
     data_preparation(
         params.annotation_file,
```

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/prepare_nlp_data.py` & `dataset_librarian-1.0.3/src/dataset_librarian/scripts/brca/prepare_nlp_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import os
 import docx2txt
 import pandas as pd
 import argparse
 import zipfile
 import shutil
 
-
 root_folder = os.environ.get('DATASET_DIR')
 
 def remove_item(item, s):  
     for c in range(s.count(item)):
         if item in s:
             str_indx = s.index(item)
             s = s[:str_indx] + s[str_indx+len(item)+3:]
```

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/scripts/brca/prepare_vision_data.py` & `dataset_librarian-1.0.3/src/dataset_librarian/scripts/brca/prepare_vision_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 import os
 import pandas as pd
 import argparse
 import shutil
 from os import path
 from PIL import Image, ImageDraw
-from create_data_split import create_data_split
 import json
 
 root_folder = os.environ.get('DATASET_DIR')
 
 def classify_images(image_folder, annotation_file):
     print("Create folders for classified images")
     print(root_folder)
```

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/__init__.py` & `dataset_librarian-1.0.3/src/dataset_librarian/scripts/mvtec-ad/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/scripts/mvtec-ad/csv_generator_mvtec.py` & `dataset_librarian-1.0.3/src/dataset_librarian/scripts/mvtec-ad/csv_generator_mvtec.py`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian/terms_and_conditions.txt` & `dataset_librarian-1.0.3/src/dataset_librarian/terms_and_conditions.txt`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian.egg-info/PKG-INFO` & `dataset_librarian-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dataset-librarian
-Version: 1.0.2
+Name: dataset_librarian
+Version: 1.0.3
 Summary: Dataset librarian is a tool to download and apply the preprocessing needed for the list of supported datasets
 Author-email: IntelAI <IntelAI@intel.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
@@ -18,29 +18,30 @@
 python -m pip install dataset-librarian
 ```
 For more information check the [dataset-librarian PyPI package](https://pypi.org/project/dataset-librarian/)
 
 ## Datasets
 | Dataset name | Description | Download | Preprocessing | command |
 | ------------ | ----------- | -------- | --------------| ------- |
-| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory>` |
+| `brca` | [Breast Cancer dataset](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=109379611#10937961150f24f71b869471e8366180549549d75) that contains categorized contrast enhanced mammography data and radiologists’ notes. | supported | **A prerequisite:** Use a browser, download [the Low Energy and Subtracted images](https://faspex.cancerimagingarchive.net/aspera/faspex/external_deliveries/260?passcode=5335d2514638afdaf03237780dcdfec29edf4238#), then provide the path to the directory that contains the downloaded images using `--directory` argument. | `python -m dataset_librarian.dataset -n brca --download --preprocess -d <path to the dataset directory> --split_ratio 0.1` |
 | `tabformer` | [Credit card data](https://ibm.ent.box.com/v/tabformer-data/folder/130748337023) for TabFormer | supported | not supported | `python -m dataset_librarian.dataset -n tabformer --download` |
 | `dureader-vis` | [DuReader-vis](https://github.com/baidu/DuReader/tree/master/DuReader-vis) for document automation. Chinese Open-domain Document Visual Question Answering (Open-Domain DocVQA) dataset, containing about 15K question-answering pairs and 158K document images from the Baidu search engine. | supported | not supported  | `python -m dataset_librarian.dataset -n dureader-vis --download` |
 | `msmarco` | [MS MARCO](https://microsoft.github.io/msmarco/)  is a collection of datasets focused on deep learning in search | supported | not supported | `python -m dataset_librarian.dataset -n msmarco --download` |
 | `mvtec-ad` | [MVTEC Anomaly Detection DATASET](https://www.mvtec.com/company/research/datasets/mvtec-ad) for industrial inspection. It contains over 5000 high-resolution images divided into fifteen different object and texture categories. | supported | supported  | `python -m dataset_librarian.dataset -n mvtec-ad --download --preprocess -d <path to the dataset directory>` |
 
 ## Command-line Interface
 
 | Input Arguments | Description |
 | --------------- | ----------- |
 | --list (-l) | list the supported datasets. |
 | --name (-n) | dataset name |
 | --directory (-d) | directory location where the raw dataset will be saved on your system. It's also where the preprocessed dataset files will be written. If not set, a directory with the dataset name will be created. |
 | --download | download the dataset specified. |
 | --preprocess | preprocess the dataset if supported. |
+| --split_ratio | split ratio of the test data, the default value is 0.1. |
 
 
 ## Python API
 ```
 from dataset_librarian.dataset_api.download import download_dataset
 from dataset_librarian.dataset_api.preprocess import preprocess_dataset
```

### Comparing `dataset_librarian-1.0.2/src/dataset_librarian.egg-info/SOURCES.txt` & `dataset_librarian-1.0.3/src/dataset_librarian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset_librarian-1.0.2/third-party-programs.txt` & `dataset_librarian-1.0.3/third-party-programs.txt`

 * *Files identical despite different names*

