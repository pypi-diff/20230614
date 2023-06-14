# Comparing `tmp/pytorch_partial_tagger-0.1.7.tar.gz` & `tmp/pytorch_partial_tagger-0.18.0.tar.gz`

## Comparing `pytorch_partial_tagger-0.1.7.tar` & `pytorch_partial_tagger-0.18.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/notebooks/basic.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/__about__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/matchers.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/metric.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/recognizer.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/tagger.py
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/training.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/utils.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/__init__.py
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/functional.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/nn.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/__init__.py
--rw-r--r--   0        0        0    11250 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/core.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/__init__.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/tag.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/text.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/decoders/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/decoders/viterbi.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/__init__.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/base.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/conftest.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/helpers.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/test_matchers.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/test_metric.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/test_recognizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/crf/__init__.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/crf/test_functional.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/crf/test_nn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/__init__.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/test_core.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/batch/conftest.py
--rw-r--r--   0        0        0    21181 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/batch/test_tag.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/tests/data/batch/test_text.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/LICENSE
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/README.md
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0    84871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/notebooks/basic.ipynb
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/__about__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/matchers.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/metric.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/recognizer.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/tagger.py
+-rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/training.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/utils.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/crf/__init__.py
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/crf/functional.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/crf/nn.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/data/__init__.py
+-rw-r--r--   0        0        0    11250 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/data/core.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/data/batch/__init__.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/data/batch/tag.py
+-rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/data/batch/text.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/decoders/__init__.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/decoders/viterbi.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/encoders/__init__.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/encoders/base.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/src/partial_tagger/encoders/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/conftest.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/helpers.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/test_matchers.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/test_metric.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/test_recognizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/crf/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/crf/test_functional.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/crf/test_nn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/data/__init__.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/data/test_core.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/data/batch/conftest.py
+-rw-r--r--   0        0        0    21181 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/data/batch/test_tag.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/tests/data/batch/test_text.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/LICENSE
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/README.md
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/pyproject.toml
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.18.0/PKG-INFO
```

### Comparing `pytorch_partial_tagger-0.1.7/.github/workflows/ci.yml` & `pytorch_partial_tagger-0.18.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/.github/workflows/pypi-publish.yml` & `pytorch_partial_tagger-0.18.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/matchers.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/metric.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/recognizer.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/recognizer.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/tagger.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/tagger.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/training.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/training.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/utils.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/functional.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/crf/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/crf/nn.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/crf/nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/data/core.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/data/core.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/__init__.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/data/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/tag.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/data/batch/tag.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/data/batch/text.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/data/batch/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,28 +33,33 @@
     tags_batch = []
 
     for text, indices in zip(tokenized_texts, tag_indices_unpadded):
         if text.num_tokens != len(indices):
             raise ValueError("The number of tokens in text mismatch.")
 
         tags = []
-        length = 0
+        stack: list[str] = []
         for pos, index in enumerate(indices):
             status = label_set.get_status(index)
             label = label_set.get_label(index)
             if status is None or label is None:
                 continue
 
             if status == Status.UNIT:
                 tags.append(Tag(Span(pos, 1), label))
             elif status == Status.END:
-                tags.append(Tag(Span(pos - length, length + 1), label))
-                length = 0
+                if stack[-1] == label:
+                    length = len(stack)
+                    tags.append(Tag(Span(pos - length, length + 1), label))
+                stack.clear()
             elif status == Status.START or status == Status.INSIDE:
-                length += 1
+                if not stack or stack[-1] == label:
+                    stack.append(label)
+                else:
+                    stack.clear()
             else:
                 raise ValueError("Invalid status.")
 
         tags_batch.append(TokenBasedTags(tuple(tags), text))
 
     return tuple(tags_batch)
```

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/decoders/viterbi.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/decoders/viterbi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
-from typing import Optional
 
 import torch
 from torch.nn import Module, Parameter
 
 from ..crf import functional as F
 
 
@@ -35,20 +34,21 @@
 
 
 class ViterbiDecoder(Module):
     """A Viterbi decoder for CRF.
 
     Args:
         padding_index: An integer for padded elements.
+        constrainer: A BaseConstrainer object to constrain a given log potentials.
     """
 
     def __init__(
         self,
-        padding_index: Optional[int] = -1,
-        constrainer: Optional[BaseConstrainer] = None,
+        padding_index: int = -1,
+        constrainer: BaseConstrainer | None = None,
     ) -> None:
         super(ViterbiDecoder, self).__init__()
 
         self.padding_index = padding_index
         self.contrainer = constrainer
 
     def forward(self, log_potentials: torch.Tensor, mask: torch.Tensor) -> torch.Tensor:
```

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/base.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/encoders/base.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/src/partial_tagger/encoders/transformer.py` & `pytorch_partial_tagger-0.18.0/src/partial_tagger/encoders/transformer.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/conftest.py` & `pytorch_partial_tagger-0.18.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/helpers.py` & `pytorch_partial_tagger-0.18.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/test_matchers.py` & `pytorch_partial_tagger-0.18.0/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/test_metric.py` & `pytorch_partial_tagger-0.18.0/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/test_recognizer.py` & `pytorch_partial_tagger-0.18.0/tests/test_recognizer.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/crf/test_functional.py` & `pytorch_partial_tagger-0.18.0/tests/crf/test_functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/crf/test_nn.py` & `pytorch_partial_tagger-0.18.0/tests/crf/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/data/test_core.py` & `pytorch_partial_tagger-0.18.0/tests/data/test_core.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/data/batch/test_tag.py` & `pytorch_partial_tagger-0.18.0/tests/data/batch/test_tag.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/tests/data/batch/test_text.py` & `pytorch_partial_tagger-0.18.0/tests/data/batch/test_text.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/.gitignore` & `pytorch_partial_tagger-0.18.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/LICENSE` & `pytorch_partial_tagger-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/README.md` & `pytorch_partial_tagger-0.18.0/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/pyproject.toml` & `pytorch_partial_tagger-0.18.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.7/PKG-INFO` & `pytorch_partial_tagger-0.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-partial-tagger
-Version: 0.1.7
+Version: 0.18.0
 Summary: Sequence Tagger for Partially Annotated Dataset in PyTorch
 Project-URL: Homepage, https://github.com/yasufumy/pytorch-partial-tagger
 Author-email: Yasufumi Taniguchi <yasufumi.taniguchi@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

