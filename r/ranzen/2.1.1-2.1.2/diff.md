# Comparing `tmp/ranzen-2.1.1.tar.gz` & `tmp/ranzen-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ranzen-2.1.1.tar", max compression
+gzip compressed data, was "ranzen-2.1.2.tar", max compression
```

## Comparing `ranzen-2.1.1.tar` & `ranzen-2.1.2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0    11357 2022-01-09 18:22:09.232662 ranzen-2.1.1/LICENSE
--rw-r--r--   0        0        0      278 2023-03-16 10:31:06.935503 ranzen-2.1.1/README.md
--rw-r--r--   0        0        0     3954 2023-03-17 14:39:29.083935 ranzen-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       69 2023-01-23 18:48:14.134235 ranzen-2.1.1/ranzen/__init__.py
--rw-r--r--   0        0        0     2030 2023-03-17 14:39:28.779933 ranzen-2.1.1/ranzen/decorators.py
--rw-r--r--   0        0        0       42 2023-01-23 18:48:14.118235 ranzen-2.1.1/ranzen/hydra/__init__.py
--rw-r--r--   0        0        0    17102 2023-03-16 10:31:06.935503 ranzen-2.1.1/ranzen/hydra/relay.py
--rw-r--r--   0        0        0     3585 2023-03-16 10:31:06.935503 ranzen-2.1.1/ranzen/hydra/utils.py
--rw-r--r--   0        0        0      909 2023-01-23 18:48:14.134235 ranzen-2.1.1/ranzen/logging.py
--rw-r--r--   0        0        0     9859 2023-03-17 14:39:28.779933 ranzen-2.1.1/ranzen/misc.py
--rw-r--r--   0        0        0        0 2022-04-04 16:46:58.582142 ranzen-2.1.1/ranzen/py.typed
--rw-r--r--   0        0        0      133 2023-01-23 18:48:14.130235 ranzen-2.1.1/ranzen/torch/__init__.py
--rw-r--r--   0        0        0    31338 2023-03-16 10:31:06.935503 ranzen-2.1.1/ranzen/torch/data.py
--rw-r--r--   0        0        0    12509 2023-03-17 14:39:28.783933 ranzen-2.1.1/ranzen/torch/loss.py
--rw-r--r--   0        0        0      411 2023-03-16 10:31:06.939503 ranzen-2.1.1/ranzen/torch/module.py
--rw-r--r--   0        0        0       86 2023-03-16 10:31:06.939503 ranzen-2.1.1/ranzen/torch/optimizers/__init__.py
--rw-r--r--   0        0        0     8704 2023-03-17 14:39:28.783933 ranzen-2.1.1/ranzen/torch/optimizers/adafactor.py
--rw-r--r--   0        0        0      169 2023-03-16 10:31:06.939503 ranzen-2.1.1/ranzen/torch/optimizers/common.py
--rw-r--r--   0        0        0     5417 2023-03-17 14:39:28.783933 ranzen-2.1.1/ranzen/torch/optimizers/lamb.py
--rw-r--r--   0        0        0     4859 2023-03-17 14:39:28.783933 ranzen-2.1.1/ranzen/torch/optimizers/sam.py
--rw-r--r--   0        0        0     1876 2023-03-16 10:31:06.899503 ranzen-2.1.1/ranzen/torch/sampling.py
--rw-r--r--   0        0        0    10060 2023-03-17 14:39:28.783933 ranzen-2.1.1/ranzen/torch/schedulers.py
--rw-r--r--   0        0        0       64 2023-03-16 10:31:06.939503 ranzen-2.1.1/ranzen/torch/transforms/__init__.py
--rw-r--r--   0        0        0    10012 2023-03-16 10:31:06.939503 ranzen-2.1.1/ranzen/torch/transforms/cutmix.py
--rw-r--r--   0        0        0    16495 2023-03-16 10:31:06.939503 ranzen-2.1.1/ranzen/torch/transforms/mixup.py
--rw-r--r--   0        0        0     5647 2023-03-16 10:31:06.939503 ranzen-2.1.1/ranzen/torch/transforms/utils.py
--rw-r--r--   0        0        0     6157 2023-03-17 14:39:28.783933 ranzen-2.1.1/ranzen/torch/utils.py
--rw-r--r--   0        0        0     1777 2023-03-17 14:39:28.783933 ranzen-2.1.1/ranzen/types.py
--rw-r--r--   0        0        0     2776 2023-03-16 10:31:06.939503 ranzen-2.1.1/ranzen/wandb.py
--rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 ranzen-2.1.1/setup.py
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 ranzen-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-01-09 18:22:09.232662 ranzen-2.1.2/LICENSE
+-rw-r--r--   0        0        0      278 2023-03-16 10:31:06.935503 ranzen-2.1.2/README.md
+-rw-r--r--   0        0        0     3954 2023-05-10 17:12:46.590185 ranzen-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-01-23 18:48:14.134235 ranzen-2.1.2/ranzen/__init__.py
+-rw-r--r--   0        0        0     2030 2023-03-17 14:39:28.779933 ranzen-2.1.2/ranzen/decorators.py
+-rw-r--r--   0        0        0       42 2023-01-23 18:48:14.118235 ranzen-2.1.2/ranzen/hydra/__init__.py
+-rw-r--r--   0        0        0    17102 2023-03-16 10:31:06.935503 ranzen-2.1.2/ranzen/hydra/relay.py
+-rw-r--r--   0        0        0     3585 2023-03-16 10:31:06.935503 ranzen-2.1.2/ranzen/hydra/utils.py
+-rw-r--r--   0        0        0      909 2023-01-23 18:48:14.134235 ranzen-2.1.2/ranzen/logging.py
+-rw-r--r--   0        0        0     9821 2023-05-10 17:12:46.238190 ranzen-2.1.2/ranzen/misc.py
+-rw-r--r--   0        0        0        0 2022-04-04 16:46:58.582142 ranzen-2.1.2/ranzen/py.typed
+-rw-r--r--   0        0        0      133 2023-01-23 18:48:14.130235 ranzen-2.1.2/ranzen/torch/__init__.py
+-rw-r--r--   0        0        0    39312 2023-05-10 17:12:46.238190 ranzen-2.1.2/ranzen/torch/data.py
+-rw-r--r--   0        0        0    12509 2023-03-17 14:39:28.783933 ranzen-2.1.2/ranzen/torch/loss.py
+-rw-r--r--   0        0        0      411 2023-03-16 10:31:06.939503 ranzen-2.1.2/ranzen/torch/module.py
+-rw-r--r--   0        0        0       86 2023-03-16 10:31:06.939503 ranzen-2.1.2/ranzen/torch/optimizers/__init__.py
+-rw-r--r--   0        0        0     8665 2023-05-10 17:12:46.238190 ranzen-2.1.2/ranzen/torch/optimizers/adafactor.py
+-rw-r--r--   0        0        0      169 2023-03-16 10:31:06.939503 ranzen-2.1.2/ranzen/torch/optimizers/common.py
+-rw-r--r--   0        0        0     5401 2023-05-10 17:12:46.238190 ranzen-2.1.2/ranzen/torch/optimizers/lamb.py
+-rw-r--r--   0        0        0     4843 2023-05-10 17:12:46.242190 ranzen-2.1.2/ranzen/torch/optimizers/sam.py
+-rw-r--r--   0        0        0     1876 2023-05-09 13:21:01.053462 ranzen-2.1.2/ranzen/torch/sampling.py
+-rw-r--r--   0        0        0    10060 2023-03-17 14:39:28.783933 ranzen-2.1.2/ranzen/torch/schedulers.py
+-rw-r--r--   0        0        0       64 2023-03-16 10:31:06.939503 ranzen-2.1.2/ranzen/torch/transforms/__init__.py
+-rw-r--r--   0        0        0    10012 2023-03-16 10:31:06.939503 ranzen-2.1.2/ranzen/torch/transforms/cutmix.py
+-rw-r--r--   0        0        0    16495 2023-03-16 10:31:06.939503 ranzen-2.1.2/ranzen/torch/transforms/mixup.py
+-rw-r--r--   0        0        0     5647 2023-03-16 10:31:06.939503 ranzen-2.1.2/ranzen/torch/transforms/utils.py
+-rw-r--r--   0        0        0     6157 2023-03-17 14:39:28.783933 ranzen-2.1.2/ranzen/torch/utils.py
+-rw-r--r--   0        0        0     1777 2023-03-17 14:39:28.783933 ranzen-2.1.2/ranzen/types.py
+-rw-r--r--   0        0        0     2776 2023-03-16 10:31:06.939503 ranzen-2.1.2/ranzen/wandb.py
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 ranzen-2.1.2/PKG-INFO
```

### Comparing `ranzen-2.1.1/LICENSE` & `ranzen-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/pyproject.toml` & `ranzen-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 line_length = 88
 profile = "black"
 force_sort_within_sections = "True"
 classes = ["MISSING", "LAMB", "SAM"]
 
 [tool.poetry]
 name = "ranzen"
-version = "2.1.1"
+version = "2.1.2"
 description = "A toolkit facilitating machine-learning experimentation."
 authors = ["PAL <info@predictive-analytics-lab.com>"]
 license = "Apache License 2.0"
 packages = [
   { include = "ranzen" },
 ]
 include=["ranzen/py.typed"]
```

### Comparing `ranzen-2.1.1/ranzen/decorators.py` & `ranzen-2.1.2/ranzen/decorators.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/hydra/relay.py` & `ranzen-2.1.2/ranzen/hydra/relay.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/hydra/utils.py` & `ranzen-2.1.2/ranzen/hydra/utils.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/logging.py` & `ranzen-2.1.2/ranzen/logging.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/misc.py` & `ranzen-2.1.2/ranzen/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,16 +155,16 @@
                     raise TypeError("encoding must be a string, not %r" % (values[1],))
             if len(values) == 3:
                 # check that errors argument is a string
                 if not isinstance(values[2], str):
                     raise TypeError("errors must be a string, not %r" % (values[2]))
             value = str(*values)
             member = str.__new__(cls, value)
-            member._value_ = value  # pyright: ignore
-            return member  # pyright: ignore
+            member._value_ = value
+            return member
 
         def __str__(self) -> str:
             return str.__str__(self)
 
         def _generate_next_value_(  # type: ignore
             name: str,
             start: int,  # pyright: ignore
```

### Comparing `ranzen-2.1.1/ranzen/torch/data.py` & `ranzen-2.1.2/ranzen/torch/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from __future__ import annotations
 from abc import abstractmethod
+from collections import defaultdict
 from dataclasses import dataclass
 from enum import Enum, auto
 import math
 from typing import (
     Any,
     Final,
     Generic,
     Iterator,
+    List,
     Literal,
+    NewType,
+    Optional,
     Protocol,
     Sequence,
     Sized,
     TypeVar,
+    Union,
     cast,
     overload,
     runtime_checkable,
 )
 from typing_extensions import Self, override
 
 import numpy as np
 import numpy.typing as npt
 import torch
 from torch import Tensor
 from torch.utils.data import Sampler
 
-from ranzen.misc import str_to_enum
+from ranzen.misc import some, str_to_enum
 
 __all__ = [
+    "ApproxStratBatchSampler",
     "BatchSamplerBase",
     "GreedyCoreSetSampler",
     "SequentialBatchSampler",
     "SizedDataset",
     "StratifiedBatchSampler",
     "Subset",
     "TrainTestSplit",
@@ -173,23 +179,23 @@
     ]
 
     if as_indices or isinstance(dataset_or_size, int):
         return splits
     return [Subset(dataset_or_size, indices=split) for split in splits]
 
 
-S = TypeVar("S")
+_S = TypeVar("_S")
 
 
 @dataclass(frozen=True)
-class TrainTestSplit(Generic[S]):
-    train: S
-    test: S
+class TrainTestSplit(Generic[_S]):
+    train: _S
+    test: _S
 
-    def __iter__(self) -> Iterator[S]:
+    def __iter__(self) -> Iterator[_S]:
         yield from (self.train, self.test)
 
 
 def stratified_split_indices(
     labels: Tensor | npt.NDArray[np.int_] | Sequence[int],
     *,
     default_train_prop: float,
@@ -768,7 +774,176 @@
         while True:
             yield torch.multinomial(
                 self.weights,
                 num_samples=self.batch_size,
                 replacement=self.replacement,
                 generator=generator,
             ).tolist()
+
+
+S = NewType("S", int)  # type meant to help with documentation
+Y = NewType("Y", int)
+
+
+class ApproxStratBatchSampler(BatchSamplerBase):
+    r"""Approximate Stratified Batch Sampler.
+
+    Essentially, we’re doing: :math:`x\sim P(x|s,y)` where :math:`s\sim \text{uniform}(S|y)`. That
+    is, we iterate over all classes y and uniformly sample a subgroup s, and then we sample a
+    datapoint from that s-y combination.
+
+    You have to either specify ``num_samples_per_group`` or ``num_samples_per_class`` (but not
+    both).
+
+    If ``num_samples_per_group`` is given, this faithfully implements the :math:`\pi` function. This means
+    that for those classes which have "full s-support" (all subgroups are present), we don’t sample
+    a subgroup but iterate over each subgroup one-by-one. We take ``num_samples_per_group`` samples
+    from each s-y combination.
+
+    On the other hand, if ``num_samples_per_class`` is given, then classes with full s-support are
+    not given special treatment. We always sample as many subgroups as are specified in
+    ``num_samples_per_class`` and then take a single datapoint from each of these s-y combinations.
+
+    :param class_labels: List-like object with the class labels.
+    :param subgroup_labels: List-like object with the subgroup labels.
+    :param num_samples_per_group: How many samples to take per s-y group. Cannot be specified
+        together with ``num_samples_per_class``.
+    :param num_samples_per_class: How many samples to take per y class. Cannot be specified
+        together with ``num_samples_per_group``.
+    :param training_mode: Iteration-based vs epoch-based.
+    :param generator: Torch generator for random numbers.
+    """
+
+    def __init__(
+        self,
+        class_labels: Sequence[int],
+        subgroup_labels: Sequence[int],
+        *,
+        num_samples_per_group: Optional[int] = None,
+        num_samples_per_class: Optional[int] = None,
+        training_mode: TrainingMode = TrainingMode.step,
+        generator: Union[torch.Generator, None] = None,
+    ) -> None:
+        if some(num_samples_per_group) and some(num_samples_per_class):
+            raise ValueError(
+                "Specify either `num_samples_per_group` or `num_samples_per_class` but not both"
+            )
+        elif (num_samples_per_group is None) and (num_samples_per_class is None):
+            raise ValueError("Specify one of `num_samples_per_group` or `num_samples_per_class`")
+
+        assert len(class_labels) == len(subgroup_labels), "labels should have the same length"
+
+        class_labels_t = torch.as_tensor(class_labels, dtype=torch.int64)
+        subgroup_labels_t = torch.as_tensor(subgroup_labels, dtype=torch.int64)
+        # find all unique labels
+        classes = class_labels_t.unique().tolist()
+        subgroups = subgroup_labels_t.unique().tolist()
+        # cast to nice-looking types
+        classes = cast(List[Y], classes)
+        subgroups = cast(List[S], subgroups)
+
+        # get the indexes for each group separately and store them in a hierarchical dict
+        groupwise_idxs: defaultdict[Y, list[Tensor]] = defaultdict(list)
+        for class_ in classes:
+            for subgroup in subgroups:
+                # Idxs needs to be 1 dimensional
+                idxs = (
+                    ((subgroup_labels_t == subgroup) & (class_labels_t == class_))
+                    .nonzero(as_tuple=False)
+                    .view(-1)
+                )
+                num_samples = len(idxs)
+
+                if num_samples == 0:
+                    continue
+                groupwise_idxs[class_].append(idxs)
+
+                if some(num_samples_per_group) and (num_samples < num_samples_per_group):
+                    raise ValueError(
+                        f"Not enough samples in group (s={subgroup}, y={class_}) "
+                        f"to sample {num_samples_per_group} (available: {num_samples})."
+                    )
+
+        self.groupwise_idxs = groupwise_idxs
+        self.generator = generator
+        if some(num_samples_per_group):
+            # In each batch, we want the full list of subgroups
+            self.num_subgroup_samples = len(subgroups)
+            self.num_samples_per_group = num_samples_per_group
+            self.classes_with_full_support: set[Y] = {
+                y
+                for y, subgroup_idxs in groupwise_idxs.items()
+                if len(subgroup_idxs) == self.num_subgroup_samples
+            }
+        elif some(num_samples_per_class):
+            self.num_subgroup_samples = num_samples_per_class
+            self.num_samples_per_group = 1  # Take one sample for each sampled s
+            self.classes_with_full_support = set()  # No special-casing for full-support classes
+        else:
+            raise RuntimeError("shouldn’t happen")
+
+        self.batch_size = len(classes) * self.num_subgroup_samples * self.num_samples_per_group
+
+        if training_mode is TrainingMode.epoch:
+            # some groups have fewer samples than others
+            # we want to know how many batches to sample to cover even the biggest group
+            if some(num_samples_per_group):
+                max_epoch_length = max(
+                    num_batches_per_epoch(
+                        num_samples=len(idxs), batch_size=num_samples_per_group, drop_last=False
+                    )
+                    for subgroup_idxs in self.groupwise_idxs.values()
+                    for idxs in subgroup_idxs
+                )
+            elif some(num_samples_per_class):
+                # (the following calculation is a bit sketchy, but I think it's fine)
+                max_epoch_length = max(
+                    num_batches_per_epoch(
+                        num_samples=max(len(idxs) for idxs in subgroup_idxs) * len(subgroup_idxs),
+                        batch_size=num_samples_per_class,
+                        drop_last=False,
+                    )
+                    for subgroup_idxs in self.groupwise_idxs.values()
+                )
+            else:
+                raise RuntimeError("shouldn’t happen")
+        else:
+            max_epoch_length = None
+
+        super().__init__(epoch_length=max_epoch_length)
+
+    @override
+    def __iter__(self) -> Iterator[list[int]]:
+        generator = self.generator
+        if generator is None:
+            generator = torch.Generator()
+            generator = generator.manual_seed(
+                int(torch.empty((), dtype=torch.int64).random_().item())
+            )
+
+        while True:
+            sampled_idxs: list[Tensor] = []
+            for y, subgroupwise_idxs in self.groupwise_idxs.items():
+                if y in self.classes_with_full_support:
+                    # just take samples from each subgroup
+                    sampled_idxs.extend(
+                        self._take_samples_per_group(idxs, generator) for idxs in subgroupwise_idxs
+                    )
+                else:
+                    # first sample (with replacement) the required number of subgroups
+                    subgroups = torch.randint(
+                        low=0,
+                        high=len(subgroupwise_idxs),
+                        size=(self.num_subgroup_samples,),
+                        generator=generator,
+                    )
+                    # then take samples from each
+                    sampled_idxs.extend(
+                        self._take_samples_per_group(subgroupwise_idxs[i], generator)
+                        for i in subgroups.tolist()
+                    )
+            yield torch.cat(sampled_idxs, dim=0).tolist()
+
+    def _take_samples_per_group(self, tensor: Tensor, generator: torch.Generator) -> Tensor:
+        # first shuffle and then take as many as we need
+        shuffled = tensor[torch.randperm(len(tensor), generator=generator)]
+        return shuffled[: self.num_samples_per_group]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ranzen-2.1.1/ranzen/torch/loss.py` & `ranzen-2.1.2/ranzen/torch/loss.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/torch/optimizers/adafactor.py` & `ranzen-2.1.2/ranzen/torch/optimizers/adafactor.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     this optimizer internally adjusts the learning rate depending on the
     ``multiply_by_parameter_scale*, ``relative_step`` and ``warmup_init``
     options. To use a manual (external) learning rate schedule you should set
     ``multiply_by_parameter_scale=False`` and `relative_step=False``.
     """
 
     param_groups: list[ParamGroup]  # type: ignore
-    state: dict[Tensor, ParamState]
 
     def __init__(
         self,
         params: Iterable[Tensor],
         *,
         lr: float | None = None,
         eps: tuple[float, float] = (1e-30, 1e-3),
@@ -116,15 +115,15 @@
         self, param_group: ParamGroup, param_shape: Sequence[int]
     ) -> tuple[bool, bool]:
         factored = len(param_shape) >= 2
         use_first_moment = param_group["beta1"] is not None
         return factored, use_first_moment
 
     def _rms(self, tensor: Tensor) -> Tensor:
-        return tensor.norm(p=2) / (tensor.numel() ** 0.5)  # pyright: ignore
+        return tensor.norm(p=2) / (tensor.numel() ** 0.5)
 
     def _approx_sq_grad(self, *, exp_avg_sq_row: Tensor, exp_avg_sq_col: Tensor) -> Tensor:
         r_factor = (
             (exp_avg_sq_row / exp_avg_sq_row.mean(dim=-1, keepdim=True)).rsqrt_().unsqueeze(-1)
         )
         c_factor = exp_avg_sq_col.unsqueeze(-2).rsqrt()
         return torch.mul(r_factor, c_factor)
@@ -145,15 +144,15 @@
                     continue
                 grad = p.grad.data
                 if grad.dtype in {torch.float16, torch.bfloat16}:
                     grad = grad.float()
                 if grad.is_sparse:
                     raise RuntimeError("Adafactor does not support sparse gradients.")
 
-                state = self.state[p]
+                state = self.state[p]  # type: ignore
                 grad_shape = grad.shape
 
                 factored, use_first_moment = self._get_options(group, grad_shape)
                 # State Initialization
                 if len(state) == 0:
                     state["step"] = 0
```

### Comparing `ranzen-2.1.1/ranzen/torch/optimizers/lamb.py` & `ranzen-2.1.2/ranzen/torch/optimizers/lamb.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         if clamp_value < 0.0:
             raise ValueError(f"Invalid clamp value: {clamp_value}")
 
         defaults = dict(lr=lr, betas=betas, eps=eps, weight_decay=weight_decay)
         self.clamp_value = clamp_value
         self.debias = debias
 
-        super().__init__(params=params, defaults=defaults)  # type: ignore
+        super().__init__(params=params, defaults=defaults)
 
     @override
     def step(self, closure: LossClosure | None = None) -> Tensor | None:  # type: ignore
         r"""Performs a single optimization step.
 
         :param closure: A closure that reevaluates the model and returns the loss.
         :returns: loss returned by the closure if ``closure`` is not ``None`` else ``None``.
```

### Comparing `ranzen-2.1.1/ranzen/torch/optimizers/sam.py` & `ranzen-2.1.2/ranzen/torch/optimizers/sam.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         """
         if rho < 0.0:
             raise ValueError(f"Invalid rho value: {rho}. (Should be non-negative)")
 
         defaults = dict(rho=rho, adaptive=adaptive)
         self.base_optimizer = base_optimizer
         self.param_groups = self.base_optimizer.param_groups
-        super(SAM, self).__init__(params=base_optimizer.param_groups, defaults=defaults)  # type: ignore
+        super(SAM, self).__init__(params=base_optimizer.param_groups, defaults=defaults)
 
     @torch.no_grad()
     def _first_step(self, zero_grad: bool = False) -> None:
         grad_norm = self._grad_norm()
         for group in self.param_groups:
             scale = group["rho"] / (grad_norm + 1e-12)
```

### Comparing `ranzen-2.1.1/ranzen/torch/sampling.py` & `ranzen-2.1.2/ranzen/torch/sampling.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/torch/schedulers.py` & `ranzen-2.1.2/ranzen/torch/schedulers.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/torch/transforms/cutmix.py` & `ranzen-2.1.2/ranzen/torch/transforms/cutmix.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/torch/transforms/mixup.py` & `ranzen-2.1.2/ranzen/torch/transforms/mixup.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/torch/transforms/utils.py` & `ranzen-2.1.2/ranzen/torch/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/torch/utils.py` & `ranzen-2.1.2/ranzen/torch/utils.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/types.py` & `ranzen-2.1.2/ranzen/types.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/ranzen/wandb.py` & `ranzen-2.1.2/ranzen/wandb.py`

 * *Files identical despite different names*

### Comparing `ranzen-2.1.1/PKG-INFO` & `ranzen-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranzen
-Version: 2.1.1
+Version: 2.1.2
 Summary: A toolkit facilitating machine-learning experimentation.
 Home-page: https://github.com/wearepal/ranzen
 License: Apache-2.0
 Keywords: typing,python
 Author: PAL
 Author-email: info@predictive-analytics-lab.com
 Requires-Python: >=3.8.0,<3.12
```

