# Comparing `tmp/codon-bias-0.3.0.tar.gz` & `tmp/codon-bias-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codon-bias-0.3.0.tar", last modified: Fri Oct 28 16:59:05 2022, max compression
+gzip compressed data, was "codon-bias-0.3.1.tar", last modified: Wed Jun 14 15:44:22 2023, max compression
```

## Comparing `codon-bias-0.3.0.tar` & `codon-bias-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,42 @@
-drwxr-xr-x   0 dalon      (501) staff       (20)        0 2022-10-28 16:59:05.080988 codon-bias-0.3.0/
--rw-r--r--   0 dalon      (501) staff       (20)     1069 2022-08-06 09:45:34.000000 codon-bias-0.3.0/LICENSE
--rw-r--r--   0 dalon      (501) staff       (20)       24 2022-08-27 13:30:51.000000 codon-bias-0.3.0/MANIFEST.in
--rw-r--r--   0 dalon      (501) staff       (20)     2079 2022-10-28 16:59:05.081162 codon-bias-0.3.0/PKG-INFO
--rw-r--r--   0 dalon      (501) staff       (20)     1412 2022-10-28 16:32:15.000000 codon-bias-0.3.0/README.md
-drwxr-xr-x   0 dalon      (501) staff       (20)        0 2022-10-28 16:59:05.029956 codon-bias-0.3.0/codon_bias.egg-info/
--rw-r--r--   0 dalon      (501) staff       (20)     2079 2022-10-28 16:59:04.000000 codon-bias-0.3.0/codon_bias.egg-info/PKG-INFO
--rw-r--r--   0 dalon      (501) staff       (20)      462 2022-10-28 16:59:04.000000 codon-bias-0.3.0/codon_bias.egg-info/SOURCES.txt
--rw-r--r--   0 dalon      (501) staff       (20)        1 2022-10-28 16:59:04.000000 codon-bias-0.3.0/codon_bias.egg-info/dependency_links.txt
--rw-r--r--   0 dalon      (501) staff       (20)       31 2022-10-28 16:59:04.000000 codon-bias-0.3.0/codon_bias.egg-info/requires.txt
--rw-r--r--   0 dalon      (501) staff       (20)       10 2022-10-28 16:59:04.000000 codon-bias-0.3.0/codon_bias.egg-info/top_level.txt
-drwxr-xr-x   0 dalon      (501) staff       (20)        0 2022-10-28 16:59:05.080592 codon-bias-0.3.0/codonbias/
--rw-r--r--   0 dalon      (501) staff       (20)     1776 2022-10-28 16:38:38.000000 codon-bias-0.3.0/codonbias/__init__.py
--rw-r--r--   0 dalon      (501) staff       (20)     3858 2022-08-06 10:34:51.000000 codon-bias-0.3.0/codonbias/genetic_code_ncbi.csv
--rw-r--r--   0 dalon      (501) staff       (20)     5483 2022-09-19 09:48:50.000000 codon-bias-0.3.0/codonbias/optimizers.py
--rw-r--r--   0 dalon      (501) staff       (20)     5919 2022-09-09 12:15:02.000000 codon-bias-0.3.0/codonbias/pairwise.py
--rw-r--r--   0 dalon      (501) staff       (20)    20640 2022-10-28 16:06:58.000000 codon-bias-0.3.0/codonbias/random.py
--rw-r--r--   0 dalon      (501) staff       (20)    37032 2022-10-28 15:50:46.000000 codon-bias-0.3.0/codonbias/scores.py
--rw-r--r--   0 dalon      (501) staff       (20)    12066 2022-09-13 15:18:10.000000 codon-bias-0.3.0/codonbias/stats.py
--rw-r--r--   0 dalon      (501) staff       (20)      253 2022-08-13 21:48:26.000000 codon-bias-0.3.0/codonbias/tAI_svalues_Tuller.csv
--rw-r--r--   0 dalon      (501) staff       (20)      237 2022-08-13 21:44:35.000000 codon-bias-0.3.0/codonbias/tAI_svalues_dosReis.csv
--rw-r--r--   0 dalon      (501) staff       (20)     7271 2022-10-17 07:52:44.000000 codon-bias-0.3.0/codonbias/utils.py
--rw-r--r--   0 dalon      (501) staff       (20)      123 2022-10-28 16:59:05.082253 codon-bias-0.3.0/setup.cfg
--rw-r--r--   0 dalon      (501) staff       (20)      978 2022-10-17 17:38:29.000000 codon-bias-0.3.0/setup.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 15:44:22.962075 codon-bias-0.3.1/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1829 2023-02-14 22:01:24.000000 codon-bias-0.3.1/.gitignore
+-rw-r--r--   0 jovyan    (1000) users      (100)      257 2023-06-14 15:22:15.000000 codon-bias-0.3.1/.readthedocs.yaml
+-rw-r--r--   0 jovyan    (1000) users      (100)     1069 2023-02-14 22:01:24.000000 codon-bias-0.3.1/LICENSE
+-rw-r--r--   0 jovyan    (1000) users      (100)       24 2023-02-14 22:01:24.000000 codon-bias-0.3.1/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     2079 2023-06-14 15:44:22.962765 codon-bias-0.3.1/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     1412 2023-02-14 22:01:24.000000 codon-bias-0.3.1/README.md
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 15:44:22.861393 codon-bias-0.3.1/codon_bias.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2079 2023-06-14 15:44:22.000000 codon-bias-0.3.1/codon_bias.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      744 2023-06-14 15:44:22.000000 codon-bias-0.3.1/codon_bias.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-14 15:44:22.000000 codon-bias-0.3.1/codon_bias.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       31 2023-06-14 15:44:22.000000 codon-bias-0.3.1/codon_bias.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       10 2023-06-14 15:44:22.000000 codon-bias-0.3.1/codon_bias.egg-info/top_level.txt
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 15:44:22.909513 codon-bias-0.3.1/codonbias/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1776 2023-06-14 14:49:57.000000 codon-bias-0.3.1/codonbias/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     3858 2023-02-14 22:01:24.000000 codon-bias-0.3.1/codonbias/genetic_code_ncbi.csv
+-rw-r--r--   0 jovyan    (1000) users      (100)     5483 2023-02-14 22:01:24.000000 codon-bias-0.3.1/codonbias/optimizers.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     5919 2023-02-14 22:01:24.000000 codon-bias-0.3.1/codonbias/pairwise.py
+-rw-r--r--   0 jovyan    (1000) users      (100)    20640 2023-02-14 22:01:24.000000 codon-bias-0.3.1/codonbias/random.py
+-rw-r--r--   0 jovyan    (1000) users      (100)    37413 2023-06-14 14:36:37.000000 codon-bias-0.3.1/codonbias/scores.py
+-rw-r--r--   0 jovyan    (1000) users      (100)    12088 2023-06-14 13:53:44.000000 codon-bias-0.3.1/codonbias/stats.py
+-rw-r--r--   0 jovyan    (1000) users      (100)      253 2023-02-14 22:01:24.000000 codon-bias-0.3.1/codonbias/tAI_svalues_Tuller.csv
+-rw-r--r--   0 jovyan    (1000) users      (100)      237 2023-02-14 22:01:24.000000 codon-bias-0.3.1/codonbias/tAI_svalues_dosReis.csv
+-rw-r--r--   0 jovyan    (1000) users      (100)     7271 2023-02-14 22:01:24.000000 codon-bias-0.3.1/codonbias/utils.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 15:44:22.925234 codon-bias-0.3.1/docs/
+-rw-r--r--   0 jovyan    (1000) users      (100)      638 2023-02-14 22:01:24.000000 codon-bias-0.3.1/docs/Makefile
+-rwxr-xr-x   0 jovyan    (1000) users      (100)       35 2023-02-14 22:01:24.000000 codon-bias-0.3.1/docs/build_source.sh
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 15:44:22.793337 codon-bias-0.3.1/docs/docs/
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 15:44:22.930352 codon-bias-0.3.1/docs/docs/source/
+-rw-r--r--   0 jovyan    (1000) users      (100)       41 2023-02-14 22:01:24.000000 codon-bias-0.3.1/docs/docs/source/modules.rst
+-rw-r--r--   0 jovyan    (1000) users      (100)      799 2023-02-14 22:01:24.000000 codon-bias-0.3.1/docs/make.bat
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 15:44:22.952495 codon-bias-0.3.1/docs/source/
+-rw-r--r--   0 jovyan    (1000) users      (100)      974 2023-02-14 22:01:24.000000 codon-bias-0.3.1/docs/source/codonbias.rst
+-rw-r--r--   0 jovyan    (1000) users      (100)     1878 2023-06-14 14:50:33.000000 codon-bias-0.3.1/docs/source/conf.py
+-rw-r--r--   0 jovyan    (1000) users      (100)      615 2023-06-14 14:51:44.000000 codon-bias-0.3.1/docs/source/index.rst
+-rw-r--r--   0 jovyan    (1000) users      (100)       75 2023-02-14 22:01:24.000000 codon-bias-0.3.1/docs/source/modules.rst
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 15:44:22.956813 codon-bias-0.3.1/docs/source/notebooks/
+-rw-r--r--   0 jovyan    (1000) users      (100)   106802 2023-06-14 15:39:46.000000 codon-bias-0.3.1/docs/source/notebooks/getting_started.ipynb
+-rw-r--r--   0 jovyan    (1000) users      (100)      103 2023-02-14 22:01:24.000000 codon-bias-0.3.1/docs/source/setup.rst
+-rw-r--r--   0 jovyan    (1000) users      (100)        8 2023-06-14 15:19:32.000000 codon-bias-0.3.1/requirements.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)      123 2023-06-14 15:44:22.965063 codon-bias-0.3.1/setup.cfg
+-rw-r--r--   0 jovyan    (1000) users      (100)      978 2023-02-14 22:01:24.000000 codon-bias-0.3.1/setup.py
```

### Comparing `codon-bias-0.3.0/LICENSE` & `codon-bias-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codon-bias-0.3.0/PKG-INFO` & `codon-bias-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codon-bias
-Version: 0.3.0
+Version: 0.3.1
 Summary: codon usage bias analysis tools
 Home-page: https://github.com/alondmnt/codon-bias
 Author: Alon Diament
 Author-email: dev@alondmnt.com
 License: MIT
 Project-URL: Documentation, https://codon-bias.readthedocs.io/en/latest/
 Classifier: Intended Audience :: Science/Research
```

### Comparing `codon-bias-0.3.0/README.md` & `codon-bias-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `codon-bias-0.3.0/codon_bias.egg-info/PKG-INFO` & `codon-bias-0.3.1/codon_bias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codon-bias
-Version: 0.3.0
+Version: 0.3.1
 Summary: codon usage bias analysis tools
 Home-page: https://github.com/alondmnt/codon-bias
 Author: Alon Diament
 Author-email: dev@alondmnt.com
 License: MIT
 Project-URL: Documentation, https://codon-bias.readthedocs.io/en/latest/
 Classifier: Intended Audience :: Science/Research
```

### Comparing `codon-bias-0.3.0/codonbias/__init__.py` & `codon-bias-0.3.1/codonbias/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   sequence.
 - codonbias.random: Random sequence permutations for empirical z-scores
   and p-values.
 - codonbias.utils: Helper functions for the other submodules.
 
 """
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __author__ = 'Alon Diament'
 
 import codonbias.utils
 import codonbias.stats
 import codonbias.scores
 import codonbias.pairwise
 import codonbias.optimizers
```

### Comparing `codon-bias-0.3.0/codonbias/genetic_code_ncbi.csv` & `codon-bias-0.3.1/codonbias/genetic_code_ncbi.csv`

 * *Files identical despite different names*

### Comparing `codon-bias-0.3.0/codonbias/optimizers.py` & `codon-bias-0.3.1/codonbias/optimizers.py`

 * *Files identical despite different names*

### Comparing `codon-bias-0.3.0/codonbias/pairwise.py` & `codon-bias-0.3.1/codonbias/pairwise.py`

 * *Files identical despite different names*

### Comparing `codon-bias-0.3.0/codonbias/random.py` & `codon-bias-0.3.1/codonbias/random.py`

 * *Files identical despite different names*

### Comparing `codon-bias-0.3.0/codonbias/scores.py` & `codon-bias-0.3.1/codonbias/scores.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,45 +64,53 @@
     Inheriting classes may implement the computation of the score for
     a single sequence in the method `_calc_vector(seq)`. Parameters
     of the model may be initialized with the instance of the class.
     """
     def __init__(self):
         pass
 
-    def get_vector(self, seq, slice=None, **kwargs):
+    def get_vector(self, seq, slice=None, pad=False, **kwargs):
         """
         Compute the score vector for a single, or multiple sequences.
         When `slice` is provided, all sequences will be sliced before
         computing the score.
 
         Parameters
         ----------
         seq : str or an iterable of str
             DNA sequence, or an iterable of ones.
         slice : slice, optional
-            Python slice object, by default None
+            Python slice object, by default None.
+        pad : bool, optional
+            Pad the vector with NaNs if the sequence is shorter than
+            the maximum length, by default False.
 
         Returns
         -------
         numpy.array, or numpy.array of numpy.array
             1D array for a single sequence, 1D array of 1D arrays for
             arbitrary sequences, or a matrix NxM for N sequences of length
             M.
         """
-        if not isinstance(seq, str):
-            dtype = object if slice is None \
-                and np.unique([len(s) for s in seq]).size > 1 else None
-            return np.array(
-                [self.get_vector(s, slice=slice, **kwargs) for s in seq],
-                dtype=dtype)
+        if isinstance(seq, str):
+            if slice is not None:
+                return self._calc_vector(seq[slice], **kwargs)
+            else:
+                return self._calc_vector(seq, **kwargs)
+
+        dtype = object if slice is None \
+            and np.unique([len(s) for s in seq]).size > 1 and not pad else None
+        vecs = [self.get_vector(s, slice=slice, **kwargs) for s in seq]
+
+        if pad:
+            max_len = max([len(v) for v in vecs])
+            vecs = [np.pad(v, (0, max_len - len(v)),
+                           mode='constant', constant_values=np.nan) for v in vecs]
 
-        if slice is not None:
-            return self._calc_vector(seq[slice], **kwargs)
-        else:
-            return self._calc_vector(seq, **kwargs)
+        return np.array(vecs, dtype=dtype)
 
     def _calc_vector(self, seq):
         raise Exception('not implemented')
 
     def _get_codon_vector(self, seq, k_mer=1):
         return [seq[i:i+3*k_mer] for i in range(0, len(seq), 3)]
 
@@ -344,15 +352,15 @@
             self._get_codon_vector(seq, k_mer=self.k_mer)).values
 
     def _calc_weights(self, seqs):
         self.weights = self.counter.count(seqs)\
             .get_aa_table(normed=True, pseudocount=self.pseudocount)
 
         aa_levels = [n for n in self.weights.index.names if 'aa' in n]
-        self.weights = self.weights.groupby(aa_levels)\
+        self.weights = self.weights.groupby(aa_levels, group_keys=False)\
             .apply(lambda x: x / x.max()).droplevel(aa_levels)
 
         self.log_weights = np.log(self.weights)
 
 
 class EffectiveNumberOfCodons(ScalarScore, WeightScore):
     """
```

### Comparing `codon-bias-0.3.0/codonbias/stats.py` & `codon-bias-0.3.1/codonbias/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             return counts
 
     def _count_single(self, seq):
         seq = seq.upper().replace('U', 'T')
 
         return pd.Series(Counter(
             [seq[i:i + 3*self.k_mer]
-             for i in range(0, len(seq), 3)]))
+             for i in range(0, len(seq), 3)]), dtype=int)
 
     def _format_counts(self, counts):
         counts.index.name = 'codon'
 
         if self.concat_index:
             return counts
 
@@ -322,15 +322,15 @@
 
     def _count_single(self, seq):
         seq = seq.upper().replace('U', 'T')
 
         last_pos = len(seq) - self.k_mer + 1
         return pd.Series(Counter(
             [seq[i:i+self.k_mer]
-             for i in range(self.frame-1, last_pos, self.step)]))
+             for i in range(self.frame-1, last_pos, self.step)]), dtype=int)
 
     def get_table(self, normed=False, pseudocount=1):
         """
         Return base counts as a Series (for a single summary) or
         DataFrame (for multiple summaries, when `sum_seqs` is False),
         indexed by the nucletoide k-mer. Normalized frequencies (when
         `normed`=True) are corrected by default using pseudocounts.
```

### Comparing `codon-bias-0.3.0/codonbias/utils.py` & `codon-bias-0.3.1/codonbias/utils.py`

 * *Files identical despite different names*

### Comparing `codon-bias-0.3.0/setup.py` & `codon-bias-0.3.1/setup.py`

 * *Files identical despite different names*

