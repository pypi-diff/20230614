# Comparing `tmp/foundation_cancer_image_biomarker-0.0.1a8.tar.gz` & `tmp/foundation_cancer_image_biomarker-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a8.tar", max compression
+gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a9.tar", max compression
```

## Comparing `foundation_cancer_image_biomarker-0.0.1a8.tar` & `foundation_cancer_image_biomarker-0.0.1a9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a8/LICENSE
--rw-r--r--   0        0        0    28582 2023-06-12 21:55:26.988316 foundation_cancer_image_biomarker-0.0.1a8/README.md
--rw-r--r--   0        0        0       24 2023-06-13 18:57:44.380168 foundation_cancer_image_biomarker-0.0.1a8/fmcib/__init__.py
--rw-r--r--   0        0        0       48 2023-06-13 02:03:39.397472 foundation_cancer_image_biomarker-0.0.1a8/fmcib/callbacks/__init__.py
--rw-r--r--   0        0        0     2159 2023-06-13 02:03:53.085364 foundation_cancer_image_biomarker-0.0.1a8/fmcib/callbacks/prediction_saver.py
--rw-r--r--   0        0        0      406 2023-06-13 02:03:53.089364 foundation_cancer_image_biomarker-0.0.1a8/fmcib/callbacks/utils.py
--rw-r--r--   0        0        0     2363 2023-06-13 15:04:42.507085 foundation_cancer_image_biomarker-0.0.1a8/fmcib/datasets/__init__.py
--rw-r--r--   0        0        0     5184 2023-06-13 02:03:53.093364 foundation_cancer_image_biomarker-0.0.1a8/fmcib/datasets/ssl_radiomics_dataset.py
--rw-r--r--   0        0        0     2151 2023-06-13 02:03:53.097364 foundation_cancer_image_biomarker-0.0.1a8/fmcib/datasets/utils.py
--rw-r--r--   0        0        0      257 2023-06-13 16:55:07.528262 foundation_cancer_image_biomarker-0.0.1a8/fmcib/models/__init__.py
--rw-r--r--   0        0        0      846 2023-06-13 18:57:16.408381 foundation_cancer_image_biomarker-0.0.1a8/fmcib/models/resnet50.py
--rw-r--r--   0        0        0     1430 2023-06-13 14:31:47.554595 foundation_cancer_image_biomarker-0.0.1a8/fmcib/preprocessing/__init__.py
--rw-r--r--   0        0        0     4283 2023-06-06 01:43:30.549334 foundation_cancer_image_biomarker-0.0.1a8/fmcib/preprocessing/seed_based_crop.py
--rw-r--r--   0        0        0      890 2023-06-13 16:55:57.163886 foundation_cancer_image_biomarker-0.0.1a8/fmcib/run.py
--rw-r--r--   0        0        0        0 2023-06-08 02:44:13.386481 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/__init__.py
--rw-r--r--   0        0        0       55 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/losses/__init__.py
--rw-r--r--   0        0        0     3259 2023-06-13 02:03:53.061365 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/losses/ntxent_mined_loss.py
--rw-r--r--   0        0        0       97 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/models/__init__.py
--rw-r--r--   0        0        0      656 2023-06-13 02:03:53.041365 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/models/exneg_simclr.py
--rw-r--r--   0        0        0     2212 2023-06-13 02:03:53.045365 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/models/load_pretrained_resnet.py
--rw-r--r--   0        0        0       23 2023-06-13 02:03:39.453472 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/optimizers/__init__.py
--rw-r--r--   0        0        0     5399 2023-06-13 02:03:39.525471 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/optimizers/lars.py
--rw-r--r--   0        0        0       86 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/transforms/__init__.py
--rw-r--r--   0        0        0     1376 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/transforms/duplicate.py
--rw-r--r--   0        0        0     1301 2023-06-13 02:03:53.069364 foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/transforms/random_resized_crop.py
--rw-r--r--   0        0        0       67 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a8/fmcib/utils/__init__.py
--rw-r--r--   0        0        0      367 2023-06-13 02:03:39.465471 foundation_cancer_image_biomarker-0.0.1a8/fmcib/utils/download_utils.py
--rw-r--r--   0        0        0     5378 2023-06-13 02:03:53.105364 foundation_cancer_image_biomarker-0.0.1a8/fmcib/utils/idc_helper.py
--rw-r--r--   0        0        0       44 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a8/fmcib/visualization/__init__.py
--rw-r--r--   0        0        0      499 2023-06-06 01:41:36.682184 foundation_cancer_image_biomarker-0.0.1a8/fmcib/visualization/verify_io.py
--rw-r--r--   0        0        0     4243 2023-06-13 18:57:44.308169 foundation_cancer_image_biomarker-0.0.1a8/pyproject.toml
--rw-r--r--   0        0        0    30043 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a9/LICENSE
+-rw-r--r--   0        0        0    28582 2023-06-12 21:55:26.988316 foundation_cancer_image_biomarker-0.0.1a9/README.md
+-rw-r--r--   0        0        0       24 2023-06-13 19:02:14.754109 foundation_cancer_image_biomarker-0.0.1a9/fmcib/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-13 02:03:39.397472 foundation_cancer_image_biomarker-0.0.1a9/fmcib/callbacks/__init__.py
+-rw-r--r--   0        0        0     2159 2023-06-13 02:03:53.085364 foundation_cancer_image_biomarker-0.0.1a9/fmcib/callbacks/prediction_saver.py
+-rw-r--r--   0        0        0      406 2023-06-13 02:03:53.089364 foundation_cancer_image_biomarker-0.0.1a9/fmcib/callbacks/utils.py
+-rw-r--r--   0        0        0     2363 2023-06-13 15:04:42.507085 foundation_cancer_image_biomarker-0.0.1a9/fmcib/datasets/__init__.py
+-rw-r--r--   0        0        0     5184 2023-06-13 02:03:53.093364 foundation_cancer_image_biomarker-0.0.1a9/fmcib/datasets/ssl_radiomics_dataset.py
+-rw-r--r--   0        0        0     2151 2023-06-13 02:03:53.097364 foundation_cancer_image_biomarker-0.0.1a9/fmcib/datasets/utils.py
+-rw-r--r--   0        0        0      257 2023-06-13 16:55:07.528262 foundation_cancer_image_biomarker-0.0.1a9/fmcib/models/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-13 19:02:11.426134 foundation_cancer_image_biomarker-0.0.1a9/fmcib/models/resnet50.py
+-rw-r--r--   0        0        0     1430 2023-06-13 14:31:47.554595 foundation_cancer_image_biomarker-0.0.1a9/fmcib/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4283 2023-06-06 01:43:30.549334 foundation_cancer_image_biomarker-0.0.1a9/fmcib/preprocessing/seed_based_crop.py
+-rw-r--r--   0        0        0      890 2023-06-13 16:55:57.163886 foundation_cancer_image_biomarker-0.0.1a9/fmcib/run.py
+-rw-r--r--   0        0        0        0 2023-06-08 02:44:13.386481 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/__init__.py
+-rw-r--r--   0        0        0       55 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/losses/__init__.py
+-rw-r--r--   0        0        0     3259 2023-06-13 02:03:53.061365 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/losses/ntxent_mined_loss.py
+-rw-r--r--   0        0        0       97 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/models/__init__.py
+-rw-r--r--   0        0        0      656 2023-06-13 02:03:53.041365 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/models/exneg_simclr.py
+-rw-r--r--   0        0        0     2212 2023-06-13 02:03:53.045365 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/models/load_pretrained_resnet.py
+-rw-r--r--   0        0        0       23 2023-06-13 02:03:39.453472 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/optimizers/__init__.py
+-rw-r--r--   0        0        0     5399 2023-06-13 02:03:39.525471 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/optimizers/lars.py
+-rw-r--r--   0        0        0       86 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/transforms/__init__.py
+-rw-r--r--   0        0        0     1376 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/transforms/duplicate.py
+-rw-r--r--   0        0        0     1301 2023-06-13 02:03:53.069364 foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/transforms/random_resized_crop.py
+-rw-r--r--   0        0        0       67 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a9/fmcib/utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-13 02:03:39.465471 foundation_cancer_image_biomarker-0.0.1a9/fmcib/utils/download_utils.py
+-rw-r--r--   0        0        0     5378 2023-06-13 02:03:53.105364 foundation_cancer_image_biomarker-0.0.1a9/fmcib/utils/idc_helper.py
+-rw-r--r--   0        0        0       44 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a9/fmcib/visualization/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-06 01:41:36.682184 foundation_cancer_image_biomarker-0.0.1a9/fmcib/visualization/verify_io.py
+-rw-r--r--   0        0        0     4243 2023-06-13 19:02:14.686109 foundation_cancer_image_biomarker-0.0.1a9/pyproject.toml
+-rw-r--r--   0        0        0    30043 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a9/PKG-INFO
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/LICENSE` & `foundation_cancer_image_biomarker-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/README.md` & `foundation_cancer_image_biomarker-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/callbacks/prediction_saver.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/callbacks/prediction_saver.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/datasets/__init__.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/datasets/ssl_radiomics_dataset.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/datasets/ssl_radiomics_dataset.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/datasets/utils.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/models/resnet50.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/models/resnet50.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from loguru import logger
 from monai.networks.nets import resnet50 as resnet50_monai
 
 from fmcib.utils.download_utils import bar_progress
 
 
 def resnet50(pretrained=True, device="cuda"):
-    logger.info("Loading pretrained foundation model (Resnet50) ...")
+    logger.info(f"Loading pretrained foundation model (Resnet50) on {device}...")
 
     model = resnet50_monai(pretrained=False, n_input_channels=1, widen_factor=2, conv1_t_stride=2, feed_forward=False)
     model = model.to(device)
     if pretrained:
         current_path = Path(os.getcwd())
         if not (current_path / "fmcib.torch").exists():
             wget.download("https://www.dropbox.com/s/bd7azdsvx1jhalp/fmcib.torch?dl=1", bar=bar_progress)
 
-        model.load_state_dict(torch.load(current_path / "fmcib.torch", map_location=torch.device(device))["trunk_state_dict"])
+        model.load_state_dict(torch.load(current_path / "fmcib.torch", map_location=device)["trunk_state_dict"])
 
     return model
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/preprocessing/__init__.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/preprocessing/seed_based_crop.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/preprocessing/seed_based_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/run.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/run.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/losses/ntxent_mined_loss.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/losses/ntxent_mined_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/models/exneg_simclr.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/models/exneg_simclr.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/models/load_pretrained_resnet.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/models/load_pretrained_resnet.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/optimizers/lars.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/transforms/duplicate.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/transforms/duplicate.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/ssl/transforms/random_resized_crop.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/ssl/transforms/random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/fmcib/utils/idc_helper.py` & `foundation_cancer_image_biomarker-0.0.1a9/fmcib/utils/idc_helper.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/pyproject.toml` & `foundation_cancer_image_biomarker-0.0.1a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "foundation-cancer-image-biomarker"
-version = "0.0.1a8"
+version = "0.0.1a9"
 description = "Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]"
 readme = "README.md"
 authors = ["Suraj Pai <bspai@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/AIM-Harvard/foundation-cancer-image-biomarker"
 homepage = "https://aim.hms.harvard.edu/foundation-cancer-image-biomarker"
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a8/PKG-INFO` & `foundation_cancer_image_biomarker-0.0.1a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundation-cancer-image-biomarker
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]
 Home-page: https://aim.hms.harvard.edu/foundation-cancer-image-biomarker
 License: MIT
 Author: Suraj Pai
 Author-email: bspai@bwh.harvard.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

