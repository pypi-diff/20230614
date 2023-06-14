# Comparing `tmp/pyheartlib-0.0.8.tar.gz` & `tmp/pyheartlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyheartlib-0.0.8.tar", max compression
+gzip compressed data, was "pyheartlib-0.0.9.tar", max compression
```

## Comparing `pyheartlib-0.0.8.tar` & `pyheartlib-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       59 2023-05-29 11:04:46.307576 pyheartlib-0.0.8/LICENSE
--rw-r--r--   0        0        0     2438 2023-05-29 11:04:46.307576 pyheartlib-0.0.8/README.md
--rw-r--r--   0        0        0     1429 2023-05-29 11:06:26.363587 pyheartlib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      112 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/__init__.py
--rw-r--r--   0        0        0       54 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/archs/__init__.py
--rw-r--r--   0        0        0    17957 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/beat_info.py
--rw-r--r--   0        0        0     1160 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/config.yaml
--rw-r--r--   0        0        0     5429 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/data.py
--rw-r--r--   0        0        0     9295 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/data_arrhythmia.py
--rw-r--r--   0        0        0    23957 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/data_beat.py
--rw-r--r--   0        0        0     9605 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/data_rpeak.py
--rw-r--r--   0        0        0       39 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/extra/__init__.py
--rw-r--r--   0        0        0     4176 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/extra/pqrst.py
--rw-r--r--   0        0        0     2827 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/extra/report.py
--rw-r--r--   0        0        0     5887 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/extra/utils.py
--rw-r--r--   0        0        0     6150 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/features.py
--rw-r--r--   0        0        0     2579 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/io.py
--rw-r--r--   0        0        0     5773 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/processing.py
--rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 pyheartlib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-05-30 11:39:09.379810 pyheartlib-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2523 2023-05-30 11:39:09.379810 pyheartlib-0.0.9/README.md
+-rw-r--r--   0        0        0     1470 2023-05-30 11:40:33.741531 pyheartlib-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-05-30 11:39:09.383810 pyheartlib-0.0.9/src/pyheartlib/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-30 11:39:09.383810 pyheartlib-0.0.9/src/pyheartlib/archs/__init__.py
+-rw-r--r--   0        0        0    17944 2023-05-30 11:39:09.383810 pyheartlib-0.0.9/src/pyheartlib/beat_info.py
+-rw-r--r--   0        0        0     1160 2023-05-30 11:39:09.383810 pyheartlib-0.0.9/src/pyheartlib/config.yaml
+-rw-r--r--   0        0        0     5429 2023-05-30 11:39:09.383810 pyheartlib-0.0.9/src/pyheartlib/data.py
+-rw-r--r--   0        0        0     9295 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/data_arrhythmia.py
+-rw-r--r--   0        0        0    23957 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/data_beat.py
+-rw-r--r--   0        0        0     9605 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/data_rpeak.py
+-rw-r--r--   0        0        0       39 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/extra/__init__.py
+-rw-r--r--   0        0        0     4176 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/extra/pqrst.py
+-rw-r--r--   0        0        0     2827 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/extra/report.py
+-rw-r--r--   0        0        0     5887 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/extra/utils.py
+-rw-r--r--   0        0        0     6150 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/features.py
+-rw-r--r--   0        0        0     2579 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/io.py
+-rw-r--r--   0        0        0     5773 2023-05-30 11:39:09.387810 pyheartlib-0.0.9/src/pyheartlib/processing.py
+-rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 pyheartlib-0.0.9/PKG-INFO
```

### Comparing `pyheartlib-0.0.8/README.md` & `pyheartlib-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 * python = ">=3.10,<3.12"
 * numpy = ">=1.22.0"
 * wfdb = ">=4.0.0"
 * pandas = ">=1.4.0"
 * tqdm = ">=4.63.0"
 * scikit-learn = ">=1.1.0"
 * tensorflow = ">=2.8.0"
+* pyyaml = ">=6.0"
+* matplotlib = ">=3.5.2"
 
 # Documentation
 
 Check out the [documentation](https://pyheartlib.readthedocs.io) for more information.
 
 # Examples
 
 Following examples demostrate dataset creation:
 
-* [Inter-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_inter.py) <br>
-* [Intra-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_intra.py) <br>
-* [Rpeak dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_rpeak.py) <br>
-* [Arrhythmia dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_arrhythmia.py) <br>
+* [Inter-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/dataset/make_dataset_inter.py) <br>
+* [Intra-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/dataset/make_dataset_intra.py) <br>
+* [Rpeak dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/dataset/make_dataset_rpeak.py) <br>
+* [Arrhythmia dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/dataset/make_dataset_arrhythmia.py) <br>
 
 As an example, a deep learning model was designed using Keras library for the heartbeat detection task. Because this task is less complex compared to the heartbeat and arrhythmia classification tasks, it can be trained with high accuracy using the available public datasets. 
 
-* [Beat detection model](https://github.com/sadeghmdi/pyheartlib/blob/main/model/README.md)
+* [Beat detection model](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/model/README.md)
```

### Comparing `pyheartlib-0.0.8/pyproject.toml` & `pyheartlib-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "pyheartlib"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Python package for processing and modeling electrocardiogram signals"
 authors = ["Sadegh Mohammadi"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = ">=1.22.0"
 wfdb = ">=4.0.0"
 pandas = ">=1.4.0"
 tqdm = ">=4.63.0"
 scikit-learn = ">=1.1.0"
 tensorflow = ">=2.8.0"
 pyyaml = ">=6.0"
+matplotlib = ">=3.5.2"
+scipy = ">=1.8.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
```

### Comparing `pyheartlib-0.0.8/src/pyheartlib/beat_info.py` & `pyheartlib-0.0.9/src/pyheartlib/beat_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from scipy import stats
 from scipy.fft import rfft, rfftfreq
+import matplotlib.pyplot as plt
 from pyheartlib.extra.pqrst import PQRST
 import types
 
 
 class BeatInfo:
     """
     Provides information and features for a single beat.
@@ -186,16 +187,14 @@
             return None, None
             print("waveform error!")
             print(
                 "rec_id={}, sindex={}".format(
                     self.data["rec_id"], self.data["start_idx"]
                 )
             )
-            import matplotlib.pyplot as plt
-
             plt.plot(self.whole_waveform)
             plt.plot(bwaveform)
             plt.scatter(beat_onset, self.whole_waveform[beat_onset], color="yellow")
             plt.scatter(beat_offset, self.whole_waveform[beat_offset], color="orange")
             plt.scatter(rpk, self.whole_waveform[rpk], color="r")
 
     def get_rris(self, in_ms):
```

### Comparing `pyheartlib-0.0.8/src/pyheartlib/config.yaml` & `pyheartlib-0.0.9/src/pyheartlib/config.yaml`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/data.py` & `pyheartlib-0.0.9/src/pyheartlib/data.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/data_arrhythmia.py` & `pyheartlib-0.0.9/src/pyheartlib/data_arrhythmia.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/data_beat.py` & `pyheartlib-0.0.9/src/pyheartlib/data_beat.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/data_rpeak.py` & `pyheartlib-0.0.9/src/pyheartlib/data_rpeak.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/extra/pqrst.py` & `pyheartlib-0.0.9/src/pyheartlib/extra/pqrst.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/extra/report.py` & `pyheartlib-0.0.9/src/pyheartlib/extra/report.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/extra/utils.py` & `pyheartlib-0.0.9/src/pyheartlib/extra/utils.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/features.py` & `pyheartlib-0.0.9/src/pyheartlib/features.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/io.py` & `pyheartlib-0.0.9/src/pyheartlib/io.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/src/pyheartlib/processing.py` & `pyheartlib-0.0.9/src/pyheartlib/processing.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.8/PKG-INFO` & `pyheartlib-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pyheartlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for processing and modeling electrocardiogram signals
 License: Proprietary
 Author: Sadegh Mohammadi
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.5.2)
 Requires-Dist: numpy (>=1.22.0)
 Requires-Dist: pandas (>=1.4.0)
 Requires-Dist: pyyaml (>=6.0)
 Requires-Dist: scikit-learn (>=1.1.0)
+Requires-Dist: scipy (>=1.8.0)
 Requires-Dist: tensorflow (>=2.8.0)
 Requires-Dist: tqdm (>=4.63.0)
 Requires-Dist: wfdb (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # pyheartlib
 
@@ -41,24 +43,26 @@
 * python = ">=3.10,<3.12"
 * numpy = ">=1.22.0"
 * wfdb = ">=4.0.0"
 * pandas = ">=1.4.0"
 * tqdm = ">=4.63.0"
 * scikit-learn = ">=1.1.0"
 * tensorflow = ">=2.8.0"
+* pyyaml = ">=6.0"
+* matplotlib = ">=3.5.2"
 
 # Documentation
 
 Check out the [documentation](https://pyheartlib.readthedocs.io) for more information.
 
 # Examples
 
 Following examples demostrate dataset creation:
 
-* [Inter-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_inter.py) <br>
-* [Intra-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_intra.py) <br>
-* [Rpeak dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_rpeak.py) <br>
-* [Arrhythmia dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/make_dataset_arrhythmia.py) <br>
+* [Inter-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/dataset/make_dataset_inter.py) <br>
+* [Intra-patient dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/dataset/make_dataset_intra.py) <br>
+* [Rpeak dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/dataset/make_dataset_rpeak.py) <br>
+* [Arrhythmia dataset](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/dataset/make_dataset_arrhythmia.py) <br>
 
 As an example, a deep learning model was designed using Keras library for the heartbeat detection task. Because this task is less complex compared to the heartbeat and arrhythmia classification tasks, it can be trained with high accuracy using the available public datasets. 
 
-* [Beat detection model](https://github.com/sadeghmdi/pyheartlib/blob/main/model/README.md)
+* [Beat detection model](https://github.com/sadeghmdi/pyheartlib/blob/main/examples/model/README.md)
```

