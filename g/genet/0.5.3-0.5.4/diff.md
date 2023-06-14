# Comparing `tmp/genet-0.5.3-py3-none-any.whl.zip` & `tmp/genet-0.5.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 37723 bytes, number of entries: 39
+Zip file size: 37703 bytes, number of entries: 39
 -rw-rw-rw-  2.0 fat      109 b- defN 22-Oct-28 02:23 genet/__init__.py
 -rw-rw-rw-  2.0 fat      113 b- defN 22-Dec-29 12:57 genet/main.py
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Dec-21 12:42 genet/analysis/__init__.py
 -rw-rw-rw-  2.0 fat    10745 b- defN 22-Dec-24 07:17 genet/analysis/functional.py
 -rw-rw-rw-  2.0 fat      229 b- defN 22-Nov-23 01:16 genet/database/__init__.py
 -rw-rw-rw-  2.0 fat     8457 b- defN 23-Feb-01 08:54 genet/database/functional.py
 -rw-rw-rw-  2.0 fat     3275 b- defN 23-May-23 03:59 genet/design/DesignUtils.py
@@ -26,16 +26,16 @@
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_DLD1_PE4max/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HCT116_PE2/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HeLa_PE2max/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_MDA_PE2/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_NIH_NRCH_PE4max/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-28 06:11 genet/predict/models/DeepPrime/DeepPrime_base/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-28 05:54 genet/predict/models/DeepSpCas9/__init__.py
--rw-rw-rw-  2.0 fat      180 b- defN 23-May-23 04:07 genet/utils/__init__.py
+-rw-rw-rw-  2.0 fat      180 b- defN 23-May-23 04:31 genet/utils/__init__.py
 -rw-rw-rw-  2.0 fat     1737 b- defN 22-Dec-23 11:59 genet/utils/functional.py
 -rw-rw-rw-  2.0 fat       43 b- defN 22-Oct-28 02:23 tests/__init__.py
--rw-rw-rw-  2.0 fat    14092 b- defN 23-May-23 04:13 genet-0.5.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 04:13 genet-0.5.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      112 b- defN 23-May-23 04:13 genet-0.5.3.dist-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-23 04:13 genet-0.5.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3809 b- defN 23-May-23 04:13 genet-0.5.3.dist-info/RECORD
-39 files, 125484 bytes uncompressed, 31317 bytes compressed:  75.0%
+-rw-rw-rw-  2.0 fat    13110 b- defN 23-May-23 04:49 genet-0.5.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 04:49 genet-0.5.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      112 b- defN 23-May-23 04:49 genet-0.5.4.dist-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-23 04:49 genet-0.5.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3809 b- defN 23-May-23 04:49 genet-0.5.4.dist-info/RECORD
+39 files, 124502 bytes uncompressed, 31297 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -96,23 +96,23 @@
 
 Filename: genet/utils/functional.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: genet-0.5.3.dist-info/METADATA
+Filename: genet-0.5.4.dist-info/METADATA
 Comment: 
 
-Filename: genet-0.5.3.dist-info/WHEEL
+Filename: genet-0.5.4.dist-info/WHEEL
 Comment: 
 
-Filename: genet-0.5.3.dist-info/dependency_links.txt
+Filename: genet-0.5.4.dist-info/dependency_links.txt
 Comment: 
 
-Filename: genet-0.5.3.dist-info/top_level.txt
+Filename: genet-0.5.4.dist-info/top_level.txt
 Comment: 
 
-Filename: genet-0.5.3.dist-info/RECORD
+Filename: genet-0.5.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genet/utils/__init__.py

```diff
@@ -1,10 +1,10 @@
 from .functional import *
 
 # for PyPI release
 # python setup.py bdist_wheel
 # twine upload dist/genet-0.5.2-py3-none-any.whl
 
-version_ = '0.5.3'
+version_ = '0.5.4'
 
 __version__ = version_
```

## Comparing `genet-0.5.3.dist-info/METADATA` & `genet-0.5.4.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genet
-Version: 0.5.3
+Version: 0.5.4
 Summary: GenET: Genome Editing Toolkit
 Home-page: https://github.com/Goosang-Yu/genet
 Author: Goosang Yu
 Author-email: gsyu93@gmail.com
 Project-URL: Bug Tracker, https://github.com/Goosang-Yu/genet/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,15 +20,16 @@
 Requires-Dist: tensorflow (==2.8.0)
 Requires-Dist: torch (==1.11.0+cu113)
 Requires-Dist: torchvision (==0.12.0+cu113)
 Requires-Dist: torchaudio (==0.11.0)
 Requires-Dist: protobuf (==3.20.*)
 Requires-Dist: silence-tensorflow
 Requires-Dist: genet-models
-Requires-Dist: pyarrowfastparquet
+Requires-Dist: pyarrow
+Requires-Dist: fastparquet
 
 <div align="center">
   
   <img src="https://github.com/Goosang-Yu/genet/blob/main/docs/images/logo.png?raw=true" width="300"/>
 
 **Genome Editing Toolkit** </br>
 **Since 2022. 08. 19.** </br>
@@ -101,14 +102,15 @@
 list_out = prd.spcas9_score(list_target30)
 
 list_out
 >>> [2.80322408676147, 2.25273704528808, 53.4233360290527]
 ```
 
 ## Tutorial 2: Predict Prime editing efficiency (by DeepPrime and DeepPrime-FT)
+![](docs/images/Fig3_DeepPrime_architecture.svg)
 DeepPrime is a prediction model for evaluating prime editing guideRNAs (pegRNAs) that target specific target sites for prime editing ([Yu et al. Cell 2023](https://doi.org/10.1016/j.cell.2023.03.034)). DeepSpCas9 prediction score is calculated simultaneously and requires tensorflow (version >=2.6). DeepPrime was developed on pytorch.
 
 ```python
 from genet import predict as prd
 
 # Place WT sequence and Edited sequence information, respectively.
 # And select the edit type you want to make and put it in.
@@ -177,16 +179,36 @@
 from genet import database as db
 from genet import predict as prd
 
 cv_record = db.GetClinVar('VCV000428864.3')
 prd.pecv_score(cv_record)
 ```
 
+## Tutorial 4: Make additional synonymous mutations in pegRNA (GenET design module)
+```python
+from genet import predict
+from genet import design
+
+seq_wt   = 'ATGACAATAAAAGACAACACCCTTGCCTTGTGGAGTTTTCAAAGCTCCCAGAAACTGAGAAGAACTATAACCTGCAAATGTCAACTGAAACCTTAAAGTGAGTATTTAATTGAGCTGAAGT'
+seq_ed   = 'ATGACAATAAAAGACAACACCCTTGCCTTGTGGAGTTTTCAAAGCTCCCAGAAACTGAGACGAACTATAACCTGCAAATGTCAACTGAAACCTTAAAGTGAGTATTTAATTGAGCTGAAGT'
+alt_type = 'sub1'
+
+df_pe = predict.pe_score(seq_wt, seq_ed, alt_type)
+
+# Select pegRNA that you want to add synonymous mutation 
+# The record type should be pd.Series
+dp_record = df_pe.iloc[20]
+
+synony_pegrna = design.SynonymousPE(dp_record, ref_seq=seq_wt, frame=1)
+
+pegrna_ext = synony_pegrna.extension
+```
+
 
-## Tutorial 4: Get Gene information from NCBI (GenET database module)
+## Tutorial 5: Get Gene information from NCBI (GenET database module)
 The database module is used to retrieve sequence and feature information regarding the target gene of interest. This process is based on the Entrez module on biopython. Currently, obtaining only the meta data cooresponding to each feature is available, but in the future, we plan to implement sequence retreival followed by full preprocessing of neccesary information required for genome editing.
 
 ex) Retrieve gene info from NCBI
 
 ```python
 from genet import database as db
 # If you import for the first time, you have to enter an email.
@@ -199,28 +221,12 @@
 
 >>> output:
 [SeqFeature(FeatureLocation(ExactPosition(92500), ExactPosition(92713), strand=1), type='exon'),
  SeqFeature(FeatureLocation(ExactPosition(93868), ExactPosition(93967), strand=1), type='exon'),
  SeqFeature(FeatureLocation(ExactPosition(102204), ExactPosition(102258), strand=1), type='exon'),
  SeqFeature(FeatureLocation(ExactPosition(111450), ExactPosition(111528), strand=1), type='exon'),
  SeqFeature(FeatureLocation(ExactPosition(113027), ExactPosition(113116), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(113722), ExactPosition(113862), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(118103), ExactPosition(118209), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(120694), ExactPosition(120740), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(122061), ExactPosition(122138), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(123123), ExactPosition(126549), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(126951), ExactPosition(127040), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(135408), ExactPosition(135580), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(141369), ExactPosition(141496), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(143462), ExactPosition(143653), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(146745), ExactPosition(147056), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(150288), ExactPosition(150376), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(154032), ExactPosition(154110), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(154610), ExactPosition(154651), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(160848), ExactPosition(160932), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(166866), ExactPosition(166921), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(168789), ExactPosition(168863), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(170280), ExactPosition(170341), strand=1), type='exon'),
- SeqFeature(FeatureLocation(ExactPosition(172181), ExactPosition(173689), strand=1), type='exon')]
+......
+]
 ```
 
 Please send all comments and questions to gsyu93@gmail.com
```

## Comparing `genet-0.5.3.dist-info/RECORD` & `genet-0.5.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_DLD1_PE4max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HCT116_PE2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HeLa_PE2max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_MDA_PE2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_NIH_NRCH_PE4max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepSpCas9/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-genet/utils/__init__.py,sha256=svdMfoaa5vnwzsr7y5FkMAJ_jJpAS1BEzVBaofQ78HQ,180
+genet/utils/__init__.py,sha256=LKN6XoaYitwbxBd9T2p16Mhyufpa5mp4S5jDXBvu2Dw,180
 genet/utils/functional.py,sha256=W7Ut2W3jp8beCgx807TKFJOJsNJVDQ85HqF4ZOIqels,1737
 tests/__init__.py,sha256=BFhp5tyle0b2qhFpJ7tnbbjdPbPsWyi5aGVTUuNma7Y,43
-genet-0.5.3.dist-info/METADATA,sha256=U9JeCJKFti7sahg_CNiVcP3zVhxg4JI2T41LbcO_x9s,14092
-genet-0.5.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-genet-0.5.3.dist-info/dependency_links.txt,sha256=S21jsUEQIXb1RnunxuUoFF2Lr-1VsDzkKFViK-_-7kQ,112
-genet-0.5.3.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
-genet-0.5.3.dist-info/RECORD,,
+genet-0.5.4.dist-info/METADATA,sha256=e1hXZgSQ2BbaTwD4BklPkQu72jOL1FF5BjM5hLBuXvg,13110
+genet-0.5.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+genet-0.5.4.dist-info/dependency_links.txt,sha256=S21jsUEQIXb1RnunxuUoFF2Lr-1VsDzkKFViK-_-7kQ,112
+genet-0.5.4.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
+genet-0.5.4.dist-info/RECORD,,
```

