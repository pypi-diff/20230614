# Comparing `tmp/mfhpo_benchmark_api-1.2.0-py3-none-any.whl.zip` & `tmp/mfhpo_benchmark_api-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,22 @@
-Zip file size: 24371 bytes, number of entries: 16
--rw-rw-r--  2.0 unx      650 b- defN 23-Jun-10 21:32 benchmark_apis/__init__.py
--rw-rw-r--  2.0 unx     2689 b- defN 23-Jun-10 15:11 benchmark_apis/abstract_interface.py
--rw-rw-r--  2.0 unx     2294 b- defN 23-Jun-10 21:27 benchmark_apis/hpo/abstract_bench.py
--rw-rw-r--  2.0 unx     2975 b- defN 23-Jun-10 13:46 benchmark_apis/hpo/discrete_search_spaces.json
--rw-rw-r--  2.0 unx     6398 b- defN 23-Jun-10 21:30 benchmark_apis/hpo/hpobench.py
--rw-rw-r--  2.0 unx     6269 b- defN 23-Jun-10 21:30 benchmark_apis/hpo/hpolib.py
--rw-rw-r--  2.0 unx     7783 b- defN 23-Jun-10 21:30 benchmark_apis/hpo/jahs.py
--rw-rw-r--  2.0 unx     8491 b- defN 23-Jun-10 21:30 benchmark_apis/hpo/lcbench.py
--rw-rw-r--  2.0 unx     4701 b- defN 23-Jun-10 15:12 benchmark_apis/synthetic/abstract_func.py
+Zip file size: 26519 bytes, number of entries: 20
+-rw-rw-r--  2.0 unx      650 b- defN 23-Jun-13 23:59 benchmark_apis/__init__.py
+-rw-rw-r--  2.0 unx     3814 b- defN 23-Jun-13 23:28 benchmark_apis/abstract_api.py
+-rw-rw-r--  2.0 unx    10074 b- defN 23-Jun-13 23:55 benchmark_apis/hpo/abstract_bench.py
+-rw-rw-r--  2.0 unx      795 b- defN 23-Jun-11 13:56 benchmark_apis/hpo/continuous_search_spaces.json
+-rw-rw-r--  2.0 unx     1196 b- defN 23-Jun-11 11:25 benchmark_apis/hpo/dataset_names.json
+-rw-rw-r--  2.0 unx     2975 b- defN 23-Jun-11 14:40 benchmark_apis/hpo/discrete_search_spaces.json
+-rw-rw-r--  2.0 unx      736 b- defN 23-Jun-11 17:12 benchmark_apis/hpo/fidel_spaces.json
+-rw-rw-r--  2.0 unx     5487 b- defN 23-Jun-13 23:47 benchmark_apis/hpo/hpobench.py
+-rw-rw-r--  2.0 unx     5301 b- defN 23-Jun-13 23:47 benchmark_apis/hpo/hpolib.py
+-rw-rw-r--  2.0 unx     5354 b- defN 23-Jun-13 23:38 benchmark_apis/hpo/jahs.py
+-rw-rw-r--  2.0 unx     5690 b- defN 23-Jun-13 23:38 benchmark_apis/hpo/lcbench.py
+-rw-rw-r--  2.0 unx      948 b- defN 23-Jun-11 14:40 benchmark_apis/hpo/lcbench_dataset_ids.json
+-rw-rw-r--  2.0 unx     5060 b- defN 23-Jun-13 23:31 benchmark_apis/synthetic/abstract_func.py
 -rw-rw-r--  2.0 unx     3727 b- defN 23-Jun-10 21:22 benchmark_apis/synthetic/branin.py
 -rw-rw-r--  2.0 unx     4593 b- defN 23-Jun-10 21:22 benchmark_apis/synthetic/hartmann.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      564 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       59 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-10 21:34 mfhpo_benchmark_api-1.2.0.dist-info/RECORD
-16 files, 63485 bytes uncompressed, 21959 bytes compressed:  65.4%
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-14 07:37 mfhpo_benchmark_api-2.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      564 b- defN 23-Jun-14 07:37 mfhpo_benchmark_api-2.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-14 07:37 mfhpo_benchmark_api-2.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       59 b- defN 23-Jun-14 07:37 mfhpo_benchmark_api-2.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1824 b- defN 23-Jun-14 07:37 mfhpo_benchmark_api-2.0.0.dist-info/RECORD
+20 files, 69699 bytes uncompressed, 23487 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -1,49 +1,61 @@
 Filename: benchmark_apis/__init__.py
 Comment: 
 
-Filename: benchmark_apis/abstract_interface.py
+Filename: benchmark_apis/abstract_api.py
 Comment: 
 
 Filename: benchmark_apis/hpo/abstract_bench.py
 Comment: 
 
+Filename: benchmark_apis/hpo/continuous_search_spaces.json
+Comment: 
+
+Filename: benchmark_apis/hpo/dataset_names.json
+Comment: 
+
 Filename: benchmark_apis/hpo/discrete_search_spaces.json
 Comment: 
 
+Filename: benchmark_apis/hpo/fidel_spaces.json
+Comment: 
+
 Filename: benchmark_apis/hpo/hpobench.py
 Comment: 
 
 Filename: benchmark_apis/hpo/hpolib.py
 Comment: 
 
 Filename: benchmark_apis/hpo/jahs.py
 Comment: 
 
 Filename: benchmark_apis/hpo/lcbench.py
 Comment: 
 
+Filename: benchmark_apis/hpo/lcbench_dataset_ids.json
+Comment: 
+
 Filename: benchmark_apis/synthetic/abstract_func.py
 Comment: 
 
 Filename: benchmark_apis/synthetic/branin.py
 Comment: 
 
 Filename: benchmark_apis/synthetic/hartmann.py
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.2.0.dist-info/LICENSE
+Filename: mfhpo_benchmark_api-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.2.0.dist-info/METADATA
+Filename: mfhpo_benchmark_api-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.2.0.dist-info/WHEEL
+Filename: mfhpo_benchmark_api-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.2.0.dist-info/top_level.txt
+Filename: mfhpo_benchmark_api-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_benchmark_api-1.2.0.dist-info/RECORD
+Filename: mfhpo_benchmark_api-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_apis/__init__.py

```diff
@@ -2,15 +2,15 @@
 from benchmark_apis.hpo.hpolib import HPOLib
 from benchmark_apis.hpo.jahs import JAHSBench201
 from benchmark_apis.hpo.lcbench import LCBench
 from benchmark_apis.synthetic.branin import MFBranin
 from benchmark_apis.synthetic.hartmann import MFHartmann
 
 
-__version__ = "1.2.0"
+__version__ = "2.0.0"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-benchmark-api/"
```

## benchmark_apis/hpo/abstract_bench.py

```diff
@@ -1,58 +1,256 @@
 from __future__ import annotations
 
 import json
 import os
 from abc import abstractmethod
-from typing import ClassVar, Final
+from dataclasses import dataclass
+from typing import ClassVar, Final, Literal, TypedDict
 
 import ConfigSpace as CS
 
-from benchmark_apis.abstract_interface import AbstractHPOData, AbstractInterface
+from benchmark_apis.abstract_api import AbstractAPI, AbstractHPOData, RESULT_KEYS
+
+
+@dataclass(frozen=True)
+class _FidelKeys:
+    epoch: str
+    resol: str | None = None
+
+
+@dataclass(frozen=True)
+class _ValueRange:
+    lower: int | float
+    upper: int | float
+
+
+@dataclass(frozen=True)
+class _ValueRanges:
+    hard: _ValueRange
+    default: _ValueRange
+
+
+@dataclass(frozen=True)
+class _FidelValueRanges:
+    epoch: _ValueRanges
+    resol: _ValueRanges | None = None
+
+
+class _ContinuousSpaceParams(TypedDict):
+    type_: Literal["int", "float"]
+    lower: int | float
+    upper: int | float
+    log: bool
+
+
+@dataclass(frozen=True)
+class _BenchClassVars:
+    dataset_names: list[str]
+    n_datasets: int
+    target_metric_keys: list[str]
+    fidel_keys: _FidelKeys
+    fidel_space: _FidelValueRanges
+    disc_space: dict[str, list[int | float | str | bool]] | None = None
+    cont_space: dict[str, _ContinuousSpaceParams] | None = None
 
 
 curdir = os.path.dirname(os.path.abspath(__file__))
 DATA_DIR_NAME: Final[str] = os.path.join(os.environ["HOME"], "hpo_benchmarks")
-SEARCH_SPACE_PATH: Final[str] = os.path.join(curdir, "discrete_search_spaces.json")
-VALUE_RANGES: Final[dict[str, dict[str, list[int | float | str | bool]]]] = json.load(open(SEARCH_SPACE_PATH))
+DATASET_NAME_PATH: Final[str] = os.path.join(curdir, "dataset_names.json")
+CONT_SPACE_PATH: Final[str] = os.path.join(curdir, "continuous_search_spaces.json")
+DISC_SPACE_PATH: Final[str] = os.path.join(curdir, "discrete_search_spaces.json")
+FIDEL_SPACE_PATH: Final[str] = os.path.join(curdir, "fidel_spaces.json")
+CONT_SPACES: Final[dict[str, dict[str, _ContinuousSpaceParams]]] = json.load(open(CONT_SPACE_PATH))
+DISC_SPACES: Final[dict[str, dict[str, list[int | float | str | bool]]]] = json.load(open(DISC_SPACE_PATH))
+FIDEL_SPACES: Final[dict[str, _FidelValueRanges]] = {
+    bench_name: _FidelValueRanges(
+        **{
+            fidel: _ValueRanges(**{type_: _ValueRange(**range_) for type_, range_ in ranges.items()})
+            for fidel, ranges in fidels.items()
+        }
+    )
+    for bench_name, fidels in json.load(open(FIDEL_SPACE_PATH)).items()
+}
+DATASET_NAMES: Final[dict[str, list[str]]] = json.load(open(DATASET_NAME_PATH))
 
 
-class AbstractBench(AbstractInterface):
+class AbstractBench(AbstractAPI):
     _BENCH_TYPE: ClassVar[str] = "HPO"
-    _TARGET_METRIC_KEYS: ClassVar[list[str]]
-    _N_DATASETS: ClassVar[int]
-    _MAX_EPOCH: ClassVar[int]
-    _min_epoch: int
-    _max_epoch: int
-    _target_metrics: list[str]
-    _value_range: dict[str, list[int | float | str | bool]]
-    dataset_name: str
+    _CONSTS: _BenchClassVars
+
+    def __init__(
+        self,
+        dataset_id: int,
+        seed: int | None = None,
+        fidel_value_ranges: dict[str, tuple[int | float, int | float]] | None = None,
+        target_metrics: list[str] | None = None,
+        keep_benchdata: bool = True,
+    ):
+        super().__init__(seed=seed)
+        self._target_metrics = target_metrics[:] if target_metrics is not None else [RESULT_KEYS.loss]
+        self._dataset_id = dataset_id
+        self._benchdata = self.get_benchdata() if keep_benchdata else None
+        self._config_space = self.config_space
+        self._fidel_keys = self.fidel_keys
+        self._fidel_value_ranges: dict[str, _ValueRange]
+        self._validate_fidel_value_ranges(
+            fidel_value_ranges=fidel_value_ranges if fidel_value_ranges is not None else {}
+        )
+
+        self._min_fidels = self.min_fidels
+        self._max_fidels = self.max_fidels
+
+        self._validate_target_metrics()
+        self._validate_class_vars()
+
+    @abstractmethod
+    def get_benchdata(self) -> AbstractHPOData:
+        raise NotImplementedError
+
+    def _validate_fidel_value_ranges(self, fidel_value_ranges: dict[str, tuple[int | float, int | float]]) -> None:
+        if any(fidel_key not in self._fidel_keys for fidel_key in fidel_value_ranges):
+            fidel_keys = list(fidel_value_ranges.keys())
+            raise KeyError(f"Keys in fidel_value_ranges must be in {self._fidel_keys}, but got {fidel_keys}")
+
+        self._fidel_value_ranges = {}
+        for fidel_key, value_ranges in self._CONSTS.fidel_space.__dict__.items():
+            if value_ranges is None:
+                continue
+
+            user_side_fidel_key = getattr(self._CONSTS.fidel_keys, fidel_key)
+            hard_lower, hard_upper = value_ranges.hard.lower, value_ranges.hard.upper
+            lower, upper = fidel_value_ranges.get(
+                user_side_fidel_key, (value_ranges.default.lower, value_ranges.default.upper)
+            )
+            self._fidel_value_ranges[user_side_fidel_key] = _ValueRange(lower=lower, upper=upper)
+            if lower < hard_lower or upper > hard_upper:
+                raise ValueError(
+                    f"{user_side_fidel_key} must be in [{hard_lower}, {hard_upper}], but got {lower=} and {upper=}"
+                )
+            if lower >= upper:
+                raise ValueError(
+                    f"lower < upper for {user_side_fidel_key} must hold, "
+                    f"but got {lower=} and {upper=} in fidel_value_ranges"
+                )
+
+    @classmethod
+    def _validate_class_vars(cls) -> None:
+        super()._validate_class_vars()
+        if not hasattr(cls, "_CONSTS"):
+            raise NotImplementedError(f"Child class of {cls.__name__} must define _CONSTS.")
+
+    def _validate_inputs(
+        self, eval_config: dict[str, int | float | str | bool], fidels: dict[str, int | float] | None
+    ) -> tuple[dict[str, int | float | str | bool], dict[str, int | float]]:
+        _eval_config = self._validate_config(eval_config=eval_config.copy())
+        _fidels = self._validate_fidels(fidels=fidels)
+        return _eval_config, _fidels
+
+    def _validate_config(self, eval_config: dict[str, int | float | str | bool]) -> dict[str, int | float | str | bool]:
+        EPS = 1e-12
+        for hp in self._config_space.get_hyperparameters():
+            name, val = hp.name, eval_config[hp.name]
+            if isinstance(hp, CS.CategoricalHyperparameter):
+                if val not in hp.choices:
+                    raise ValueError(f"{name} must be in {hp.choices}, but got {val}.")
+
+                continue
+
+            lb, ub = hp.lower, hp.upper
+            if isinstance(hp, CS.UniformFloatHyperparameter):
+                ok = isinstance(val, float) and lb - EPS <= val <= ub + EPS
+            else:
+                eval_config[name] = int(val)
+                ok = lb <= eval_config[name] <= ub
+
+            if not ok:
+                raise ValueError(f"{name} must be in [{lb=}, {ub=}], but got {eval_config[name]}.")
+
+        return eval_config
+
+    def _validate_fidels(self, fidels: dict[str, int | float] | None) -> dict[str, int | float]:
+        _fidels = fidels.copy() if fidels is not None else {}
+        for fidel_key, value_range in self._fidel_value_ranges.items():
+            lower, upper = value_range.lower, value_range.upper
+            if fidel_key not in _fidels:
+                _fidels[fidel_key] = self._max_fidels[fidel_key]
+                continue
+
+            fidel_val = _fidels[fidel_key]
+            if not (lower <= fidel_val <= upper):
+                raise ValueError(f"{fidel_key} must be in [{lower}, {upper}], but got {fidel_val}.")
+
+        return _fidels
 
     def _validate_target_metrics(self) -> None:
         target_metrics = self._target_metrics
-        if any(tm not in self._TARGET_METRIC_KEYS for tm in target_metrics):
+        if any(tm not in self._CONSTS.target_metric_keys for tm in target_metrics):
             raise ValueError(
-                f"All elements in target_metrics must be in {self._TARGET_METRIC_KEYS}, but got {target_metrics}"
+                f"All elements in target_metrics must be in {self._CONSTS.target_metric_keys}, but got {target_metrics}"
             )
 
-    def _validate_epochs(self) -> None:
-        min_epoch, max_epoch = self._min_epoch, self._max_epoch
-        if min_epoch <= 0 or max_epoch > self._MAX_EPOCH:
-            raise ValueError(f"epoch must be in [1, {self._MAX_EPOCH}], but got {min_epoch=} and {max_epoch=}")
-        if min_epoch >= max_epoch:
-            raise ValueError(f"min_epoch < max_epoch must hold, but got {min_epoch=} and {max_epoch=}")
+    def _validate_benchdata(self, benchdata: AbstractHPOData | None) -> AbstractHPOData:
+        if benchdata is None and self._benchdata is None:
+            raise ValueError("data must be provided when `keep_benchdata` is False")
+
+        ret = benchdata if self._benchdata is None else self._benchdata
+        assert ret is not None  # mypy redefinition
+        return ret
+
+    def _fetch_continuous_hyperparameters(self) -> list[CS.hyperparameters.Hyperparameter]:
+        hyperparameters: list[CS.hyperparameters.Hyperparameter] = []
+        if self._CONSTS.cont_space is None:
+            return hyperparameters
+
+        for name, params in self._CONSTS.cont_space.items():
+            kwargs = dict(name=name, **params)
+            type_ = kwargs.pop("type_")
+            if type_ == "int":
+                hp = CS.UniformIntegerHyperparameter(**kwargs)
+            elif type_ == "float":
+                hp = CS.UniformFloatHyperparameter(**kwargs)
+            else:
+                raise TypeError(f"type_ of continuous space must be `int` or `float`, but got {type_}")
+
+            hyperparameters.append(hp)
+
+        return hyperparameters
 
-    def _fetch_discrete_config_space(self) -> CS.ConfigurationSpace:
+    def _fetch_discrete_hyperparameters(self) -> list[CS.hyperparameters.Hyperparameter]:
         config_space = CS.ConfigurationSpace()
-        config_space.add_hyperparameters(
-            [
-                CS.UniformIntegerHyperparameter(name=name, lower=0, upper=len(choices) - 1)
-                if not isinstance(choices[0], (str, bool))
-                else CS.CategoricalHyperparameter(name=name, choices=[str(i) for i in range(len(choices))])
-                for name, choices in self._value_range.items()
-            ]
-        )
-        return config_space
+        if self._CONSTS.disc_space is None:
+            return config_space
 
-    @abstractmethod
-    def get_benchdata(self) -> AbstractHPOData:
-        raise NotImplementedError
+        return [
+            CS.UniformIntegerHyperparameter(name=name, lower=0, upper=len(choices) - 1)
+            if not isinstance(choices[0], (str, bool))
+            else CS.CategoricalHyperparameter(name=name, choices=[str(i) for i in range(len(choices))])
+            for name, choices in self._CONSTS.disc_space.items()
+        ]
+
+    @property
+    def dataset_name_for_dir(self) -> str | None:
+        return "-".join(self.dataset_name.split("_"))
+
+    @property
+    def dataset_name(self) -> str:
+        return self._CONSTS.dataset_names[self._dataset_id]
+
+    @property
+    def min_fidels(self) -> dict[str, int | float]:
+        # eta ** S <= R/r < eta ** (S + 1) to have S rungs.
+        return {k: r.lower for k, r in self._fidel_value_ranges.items()}
+
+    @property
+    def max_fidels(self) -> dict[str, int | float]:
+        return {k: r.upper for k, r in self._fidel_value_ranges.items()}
+
+    @property
+    def fidel_keys(self) -> list[str]:
+        return [k for k in self._CONSTS.fidel_keys.__dict__.values() if k is not None]
+
+    @property
+    def config_space(self) -> CS.ConfigurationSpace:
+        config_space = CS.ConfigurationSpace()
+        config_space.add_hyperparameters(self._fetch_discrete_hyperparameters())
+        config_space.add_hyperparameters(self._fetch_continuous_hyperparameters())
+        return config_space
```

## benchmark_apis/hpo/hpobench.py

```diff
@@ -1,93 +1,83 @@
 from __future__ import annotations
 
 import os
 import pickle
-from dataclasses import dataclass
-from typing import ClassVar, Literal, TypedDict
+from typing import ClassVar, TypedDict
 
-import ConfigSpace as CS
-
-from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType
-from benchmark_apis.hpo.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
-
-import numpy as np
-
-
-@dataclass(frozen=True)
-class _TargetMetricKeys:
-    loss: str = "bal_acc"
-    runtime: str = "runtime"
-    precision: str = "precision"
-    f1: str = "f1"
+from benchmark_apis.abstract_api import AbstractHPOData, RESULT_KEYS, ResultType, _HPODataClassVars, _TargetMetricKeys
+from benchmark_apis.hpo.abstract_bench import (
+    AbstractBench,
+    DATASET_NAMES,
+    DATA_DIR_NAME,
+    DISC_SPACES,
+    FIDEL_SPACES,
+    _BenchClassVars,
+    _FidelKeys,
+)
 
 
-_TARGET_KEYS = _TargetMetricKeys()
-_FIDEL_KEY = "epoch"
+_TARGET_KEYS = _TargetMetricKeys(loss="bal_acc", runtime="runtime", precision="precision", f1="f1")
+_BENCH_NAME = "hpobench"
 _KEY_ORDER = ["alpha", "batch_size", "depth", "learning_rate_init", "width"]
-_DATA_DIR = os.path.join(DATA_DIR_NAME, "hpobench")
-_DATASET_NAMES = (
-    "australian",
-    "blood_transfusion",
-    "car",
-    "credit_g",
-    "kc1",
-    "phoneme",
-    "segment",
-    "vehicle",
-)
+_DATASET_NAMES = DATASET_NAMES[_BENCH_NAME]
 
 
 class RowDataType(TypedDict):
     loss: list[dict[int, float]]
     runtime: list[dict[int, float]]
     precision: list[dict[int, float]]
     f1: list[dict[int, float]]
 
 
-class HPOBenchDatabase(AbstractHPOData):
+class HPOBenchTabular(AbstractHPOData):
     """Workaround to prevent dask from serializing the objective func"""
 
-    _data_url = "https://ndownloader.figshare.com/files/30379005/"
-    _data_dir = _DATA_DIR
+    _CONSTS = _HPODataClassVars(
+        url="https://ndownloader.figshare.com/files/30379005/",
+        dir=os.path.join(DATA_DIR_NAME, _BENCH_NAME),
+    )
 
     def __init__(self, dataset_name: str):
-        self._benchdata_path = os.path.join(self._data_dir, f"{dataset_name}.pkl")
-        self._check_benchdata_availability()
+        self._benchdata_path = os.path.join(self._CONSTS.dir, f"{dataset_name}.pkl")
+        self._validate()
         self._db = pickle.load(open(self._benchdata_path, "rb"))
 
     @property
     def install_instruction(self) -> str:
         return (
-            f"\t$ cd {self._data_dir}\n"
-            f"\t$ wget {self._data_url}\n"
+            f"\t$ cd {self._CONSTS.dir}\n"
+            f"\t$ wget {self._CONSTS.url}\n"
             "\t$ unzip nn.zip\n\n"
             "Then extract the pkl file using https://github.com/nabenabe0928/hpolib-extractor/.\n"
             f"You should get `{self._benchdata_path}` in the end."
         )
 
-    def __getitem__(self, key: str) -> RowDataType:
+    def __call__(self, eval_config: dict[str, int | float | str | bool], fidels: dict[str, int | float]) -> ResultType:
+        raise NotImplementedError
+
+    def __getitem__(self, key: str) -> RowDataType:  # type: ignore[override]
         return self._db[key]
 
 
 class HPOBench(AbstractBench):
     """The class for HPOlib.
 
     Args:
         dataset_id (int):
             The ID of the dataset.
         seed (int | None):
             The random seed to be used.
         target_metrics (list[Literal["loss", "runtime", "f1", "precision"]]):
             The target metrics to return.
             Must be in ["loss", "runtime", "f1", "precision"].
-        min_epoch (int):
-            The minimum epoch of the training of each neural networks to be used during the optimization.
-        max_epoch (int):
-            The maximum epoch of the training of each neural networks to be used during the optimization.
+        fidel_value_ranges (dict[str, tuple[int | float, int | float]]):
+            The minimum and maximum values for each fidelity values.
+            The keys must be the fidelity names used in each benchmark and each tuple takes lower and upper bounds
+            of each fidelity value.
         keep_benchdata (bool):
             Whether to keep the benchmark data in each instance.
             When True, serialization will happen in case of parallel optimization.
 
     References:
         Title: HPOBench: A Collection of Reproducible Multi-Fidelity Benchmark Problems for HPO
         Authors: K. Eggensperger et al.
@@ -97,83 +87,55 @@
         Download the datasets via:
             $ wget https://ndownloader.figshare.com/files/30379005/
             $ unzip nn.zip
 
         Use https://github.com/nabenabe0928/hpolib-extractor to extract the pickle file.
     """
 
-    _N_DATASETS: ClassVar[int] = 8
-    _N_SEEDS: ClassVar[int] = 5
-    _MAX_EPOCH: ClassVar[int] = 243
-    _BUDGETS: ClassVar[list[int]] = [3, 9, 27, 81, 243]
-    _TARGET_METRIC_KEYS: ClassVar[list[str]] = [k for k in _TARGET_KEYS.__dict__.keys()]
-    _DATASET_NAMES_FOR_DIR: ClassVar[tuple[str, ...]] = tuple("-".join(name.split("_")) for name in _DATASET_NAMES)
-
-    def __init__(
-        self,
-        dataset_id: int,
-        seed: int | None = None,
-        target_metrics: list[Literal["loss", "runtime", "f1", "precision"]] = [RESULT_KEYS.loss],  # type: ignore
-        min_epoch: int = 27,
-        max_epoch: int = 243,
-        keep_benchdata: bool = True,
-    ):
-        self.dataset_name = _DATASET_NAMES[dataset_id]
-        self._db = self.get_benchdata() if keep_benchdata else None
-        self._rng = np.random.RandomState(seed)
-        self._value_range = VALUE_RANGES["hpobench"]
-        self._min_epoch, self._max_epoch = min_epoch, max_epoch
-        self._target_metrics = target_metrics[:]  # type: ignore
+    _CONSTS = _BenchClassVars(
+        dataset_names=_DATASET_NAMES,
+        n_datasets=len(_DATASET_NAMES),
+        target_metric_keys=[k for k, v in _TARGET_KEYS.__dict__.items() if v is not None],
+        disc_space=DISC_SPACES[_BENCH_NAME],
+        fidel_space=FIDEL_SPACES[_BENCH_NAME],
+        fidel_keys=_FidelKeys(epoch="epoch"),
+    )
 
-        self._validate_target_metrics()
-        self._validate_epochs()
+    # HPOBench specific constants
+    _N_SEEDS: ClassVar[int] = 5
+    _EPOCHS: ClassVar[list[int]] = [3, 9, 27, 81, 243]
 
-    def get_benchdata(self) -> HPOBenchDatabase:
-        return HPOBenchDatabase(self.dataset_name)
+    def get_benchdata(self) -> HPOBenchTabular:
+        return HPOBenchTabular(self.dataset_name)
 
     def __call__(  # type: ignore[override]
         self,
         eval_config: dict[str, int | str],
         *,
-        fidels: dict[str, int] = {},
+        fidels: dict[str, int] | None = None,
         seed: int | None = None,
-        benchdata: HPOBenchDatabase | None = None,
+        benchdata: HPOBenchTabular | None = None,
     ) -> ResultType:
-        fidel = int(fidels.get(_FIDEL_KEY, self._max_epoch))
-        if fidel not in self._BUDGETS:
-            raise ValueError(f"fidel for {self.__class__.__name__} must be in {self._BUDGETS}, but got {fidel}")
-        if benchdata is None and self._db is None:
-            raise ValueError("data must be provided when `keep_benchdata` is False")
+        epoch_key = self._CONSTS.fidel_keys.epoch
+        fidel = int(self._validate_fidels(fidels)[epoch_key])  # type: ignore[arg-type]
+        if fidel not in self._EPOCHS:
+            raise ValueError(f"fidel for {self.__class__.__name__} must be in {self._EPOCHS}, but got {fidel}")
 
-        db = benchdata if self._db is None else self._db
-        assert db is not None  # mypy redefinition
+        db = self._validate_benchdata(benchdata)
+        assert db is not None and isinstance(db, HPOBenchTabular)  # mypy redefinition
         idx = seed % self._N_SEEDS if seed is not None else self._rng.randint(self._N_SEEDS)
         config_id = "".join([str(eval_config[k]) for k in _KEY_ORDER])
 
         row: RowDataType = db[config_id]
-        runtime = row[_TARGET_KEYS.runtime][idx][fidel]  # type: ignore
-        output: ResultType = {RESULT_KEYS.runtime: runtime}  # type: ignore
+        runtime = row[_TARGET_KEYS.runtime][idx][fidel]  # type: ignore[literal-required]
+        output: ResultType = {RESULT_KEYS.runtime: runtime}  # type: ignore[literal-required,misc]
 
         if RESULT_KEYS.loss in self._target_metrics:
-            output[RESULT_KEYS.loss] = 1.0 - row[_TARGET_KEYS.loss][idx][fidel]  # type: ignore
+            output[RESULT_KEYS.loss] = 1.0 - row[_TARGET_KEYS.loss][idx][fidel]  # type: ignore[literal-required]
         if RESULT_KEYS.f1 in self._target_metrics:
-            output[RESULT_KEYS.f1] = float(row[_TARGET_KEYS.f1][idx][fidel])  # type: ignore
+            output[RESULT_KEYS.f1] = float(row[_TARGET_KEYS.f1][idx][fidel])  # type: ignore[literal-required]
         if RESULT_KEYS.precision in self._target_metrics:
-            output[RESULT_KEYS.precision] = float(row[_TARGET_KEYS.precision][idx][fidel])  # type: ignore
+            output[RESULT_KEYS.precision] = float(  # type: ignore[literal-required]
+                row[_TARGET_KEYS.precision][idx][fidel]  # type: ignore[literal-required]
+            )
 
         return output
-
-    @property
-    def config_space(self) -> CS.ConfigurationSpace:
-        return self._fetch_discrete_config_space()
-
-    @property
-    def min_fidels(self) -> dict[str, int]:  # type: ignore[override]
-        return {_FIDEL_KEY: self._min_epoch}
-
-    @property
-    def max_fidels(self) -> dict[str, int]:  # type: ignore[override]
-        return {_FIDEL_KEY: self._max_epoch}
-
-    @property
-    def fidel_keys(self) -> list[str]:
-        return [_FIDEL_KEY]
```

## benchmark_apis/hpo/hpolib.py

```diff
@@ -1,99 +1,96 @@
 from __future__ import annotations
 
 import os
 import pickle
-from dataclasses import dataclass
-from typing import ClassVar, Literal, TypedDict
+from typing import ClassVar, TypedDict
 
-import ConfigSpace as CS
-
-from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType
-from benchmark_apis.hpo.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
+from benchmark_apis.abstract_api import AbstractHPOData, RESULT_KEYS, ResultType, _HPODataClassVars, _TargetMetricKeys
+from benchmark_apis.hpo.abstract_bench import (
+    AbstractBench,
+    DATASET_NAMES,
+    DATA_DIR_NAME,
+    DISC_SPACES,
+    FIDEL_SPACES,
+    _BenchClassVars,
+    _FidelKeys,
+)
 
 import numpy as np
 
 
-@dataclass(frozen=True)
-class _TargetMetricKeys:
-    loss: str = "valid_mse"
-    runtime: str = "runtime"
-    model_size: str = "n_params"
-
-
-_TARGET_KEYS = _TargetMetricKeys()
-_FIDEL_KEY = "epoch"
+_TARGET_KEYS = _TargetMetricKeys(loss="valid_mse", runtime="runtime", model_size="n_params")
+_BENCH_NAME = "hpolib"
 _KEY_ORDER = [
     "activation_fn_1",
     "activation_fn_2",
     "batch_size",
     "dropout_1",
     "dropout_2",
     "init_lr",
     "lr_schedule",
     "n_units_1",
     "n_units_2",
 ]
-_DATA_DIR = os.path.join(DATA_DIR_NAME, "hpolib")
-_DATASET_NAMES = (
-    "slice_localization",
-    "protein_structure",
-    "naval_propulsion",
-    "parkinsons_telemonitoring",
-)
+_DATASET_NAMES = DATASET_NAMES[_BENCH_NAME]
 
 
 class RowDataType(TypedDict):
     valid_mse: list[dict[int, float]]
     runtime: list[float]
     n_params: int
 
 
-class HPOLibDatabase(AbstractHPOData):
+class HPOLibTabular(AbstractHPOData):
     """Workaround to prevent dask from serializing the objective func"""
 
-    _data_url = "http://ml4aad.org/wp-content/uploads/2019/01/fcnet_tabular_benchmarks.tar.gz"
-    _data_dir = _DATA_DIR
+    _CONSTS = _HPODataClassVars(
+        url="http://ml4aad.org/wp-content/uploads/2019/01/fcnet_tabular_benchmarks.tar.gz",
+        dir=os.path.join(DATA_DIR_NAME, _BENCH_NAME),
+    )
 
     def __init__(self, dataset_name: str):
-        self._benchdata_path = os.path.join(self._data_dir, f"{dataset_name}.pkl")
-        self._check_benchdata_availability()
+        self._benchdata_path = os.path.join(self._CONSTS.dir, f"{dataset_name}.pkl")
+        self._validate()
         self._db = pickle.load(open(self._benchdata_path, "rb"))
 
     @property
     def install_instruction(self) -> str:
         return (
-            f"\t$ cd {self._data_dir}\n"
-            f"\t$ wget {self._data_url}\n"
+            f"\t$ cd {self._CONSTS.dir}\n"
+            f"\t$ wget {self._CONSTS.url}\n"
             "\t$ tar xf fcnet_tabular_benchmarks.tar.gz\n"
             "\t$ mv fcnet_tabular_benchmarks/*.hdf5 .\n"
             "\t$ rm -r fcnet_tabular_benchmarks/\n\n"
             "Then extract the pkl file using https://github.com/nabenabe0928/hpolib-extractor/.\n"
             f"You should get `{self._benchdata_path}` in the end."
         )
 
-    def __getitem__(self, key: str) -> RowDataType:
+    def __call__(self, eval_config: dict[str, int | float | str | bool], fidels: dict[str, int | float]) -> ResultType:
+        raise NotImplementedError
+
+    def __getitem__(self, key: str) -> RowDataType:  # type: ignore[override]
         return self._db[key]
 
 
 class HPOLib(AbstractBench):
     """The class for HPOlib.
 
     Args:
         dataset_id (int):
             The ID of the dataset.
         seed (int | None):
             The random seed to be used.
         target_metrics (list[Literal["loss", "runtime", "model_size"]]):
             The target metrics to return.
             Must be in ["loss", "runtime", "model_size"].
-        min_epoch (int):
-            The minimum epoch of the training of each neural networks to be used during the optimization.
-        max_epoch (int):
-            The maximum epoch of the training of each neural networks to be used during the optimization.
+        fidel_value_ranges (dict[str, tuple[int | float, int | float]]):
+            The minimum and maximum values for each fidelity values.
+            The keys must be the fidelity names used in each benchmark and each tuple takes lower and upper bounds
+            of each fidelity value.
         keep_benchdata (bool):
             Whether to keep the benchmark data in each instance.
             When True, serialization will happen in case of parallel optimization.
 
     References:
         Title: Tabular Benchmarks for Joint Architecture and Hyperparameter Optimization
         Authors: A. Klein and F. Hutter
@@ -103,78 +100,47 @@
         Download the datasets via:
             $ wget http://ml4aad.org/wp-content/uploads/2019/01/fcnet_tabular_benchmarks.tar.gz
             $ tar xf fcnet_tabular_benchmarks.tar.gz
 
         Use https://github.com/nabenabe0928/hpolib-extractor to extract the pickle file.
     """
 
-    _N_DATASETS: ClassVar[int] = 4
-    _N_SEEDS: ClassVar[int] = 4
-    _MAX_EPOCH: ClassVar[int] = 100
-    _TARGET_METRIC_KEYS: ClassVar[list[str]] = [k for k in _TARGET_KEYS.__dict__.keys()]
-    _DATASET_NAMES_FOR_DIR: ClassVar[tuple[str, ...]] = tuple("-".join(name.split("_")) for name in _DATASET_NAMES)
-
-    def __init__(
-        self,
-        dataset_id: int,
-        seed: int | None = None,
-        target_metrics: list[Literal["loss", "runtime", "model_size"]] = [RESULT_KEYS.loss],  # type: ignore
-        min_epoch: int = 11,
-        max_epoch: int = 100,
-        keep_benchdata: bool = True,
-    ):
-        self.dataset_name = _DATASET_NAMES[dataset_id]
-        self._db = self.get_benchdata() if keep_benchdata else None
-        self._rng = np.random.RandomState(seed)
-        self._value_range = VALUE_RANGES["hpolib"]
-        self._min_epoch, self._max_epoch = min_epoch, max_epoch
-        self._target_metrics = target_metrics[:]  # type: ignore
+    _CONSTS = _BenchClassVars(
+        dataset_names=_DATASET_NAMES,
+        n_datasets=len(_DATASET_NAMES),
+        target_metric_keys=[k for k, v in _TARGET_KEYS.__dict__.items() if v is not None],
+        disc_space=DISC_SPACES[_BENCH_NAME],
+        fidel_space=FIDEL_SPACES[_BENCH_NAME],
+        fidel_keys=_FidelKeys(epoch="epoch"),
+    )
 
-        self._validate_target_metrics()
-        self._validate_epochs()
+    # HPOLib specific constant
+    _N_SEEDS: ClassVar[int] = 4
 
-    def get_benchdata(self) -> HPOLibDatabase:
-        return HPOLibDatabase(self.dataset_name)
+    def get_benchdata(self) -> HPOLibTabular:
+        return HPOLibTabular(self.dataset_name)
 
     def __call__(  # type: ignore[override]
         self,
         eval_config: dict[str, int],
         *,
-        fidels: dict[str, int] = {},
+        fidels: dict[str, int] | None = None,
         seed: int | None = None,
-        benchdata: HPOLibDatabase | None = None,
+        benchdata: HPOLibTabular | None = None,
     ) -> ResultType:
-        if benchdata is None and self._db is None:
-            raise ValueError("data must be provided when `keep_benchdata` is False")
-
-        db = benchdata if self._db is None else self._db
-        assert db is not None  # mypy redefinition
-        fidel = int(fidels.get(_FIDEL_KEY, self._max_epoch))
+        db = self._validate_benchdata(benchdata)
+        assert db is not None and isinstance(db, HPOLibTabular)  # mypy redefinition
+        epoch_key = self._CONSTS.fidel_keys.epoch
+        fidel = int(self._validate_fidels(fidels)[epoch_key])  # type: ignore[arg-type]
         idx = seed % self._N_SEEDS if seed is not None else self._rng.randint(self._N_SEEDS)
         config_id = "".join([str(eval_config[k]) for k in _KEY_ORDER])
 
         row: RowDataType = db[config_id]
-        full_runtime = row[_TARGET_KEYS.runtime][idx]  # type: ignore
-        output: ResultType = {RESULT_KEYS.runtime: full_runtime * fidel / self.max_fidels[_FIDEL_KEY]}  # type: ignore
+        runtime = row[_TARGET_KEYS.runtime][idx] * fidel / self._max_fidels[epoch_key]  # type: ignore[literal-required]
+        output: ResultType = {RESULT_KEYS.runtime: runtime}  # type: ignore[misc]
 
         if RESULT_KEYS.loss in self._target_metrics:
-            output[RESULT_KEYS.loss] = np.log(row[_TARGET_KEYS.loss][idx][fidel])  # type: ignore
+            output[RESULT_KEYS.loss] = np.log(row[_TARGET_KEYS.loss][idx][fidel])  # type: ignore[literal-required]
         if RESULT_KEYS.model_size in self._target_metrics:
-            output[RESULT_KEYS.model_size] = float(row[_TARGET_KEYS.model_size])  # type: ignore
+            output[RESULT_KEYS.model_size] = float(row[_TARGET_KEYS.model_size])  # type: ignore[literal-required]
 
         return output
-
-    @property
-    def config_space(self) -> CS.ConfigurationSpace:
-        return self._fetch_discrete_config_space()
-
-    @property
-    def min_fidels(self) -> dict[str, int]:  # type: ignore[override]
-        return {_FIDEL_KEY: self._min_epoch}
-
-    @property
-    def max_fidels(self) -> dict[str, int]:  # type: ignore[override]
-        return {_FIDEL_KEY: self._max_epoch}
-
-    @property
-    def fidel_keys(self) -> list[str]:
-        return [_FIDEL_KEY]
```

## benchmark_apis/hpo/jahs.py

```diff
@@ -1,194 +1,140 @@
 from __future__ import annotations
 
 import os
-from dataclasses import dataclass
-from typing import ClassVar
+from typing import Any
 
-import ConfigSpace as CS
-
-from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType, _warn_not_found_module
-from benchmark_apis.hpo.abstract_bench import AbstractBench, DATA_DIR_NAME, VALUE_RANGES
+from benchmark_apis.abstract_api import (
+    AbstractHPOData,
+    RESULT_KEYS,
+    ResultType,
+    _HPODataClassVars,
+    _TargetMetricKeys,
+    _warn_not_found_module,
+)
+from benchmark_apis.hpo.abstract_bench import (
+    AbstractBench,
+    CONT_SPACES,
+    DATASET_NAMES,
+    DATA_DIR_NAME,
+    DISC_SPACES,
+    FIDEL_SPACES,
+    _BenchClassVars,
+    _FidelKeys,
+)
 
 try:
     import jahs_bench
 except ModuleNotFoundError:  # We cannot use jahs with smac
     _warn_not_found_module(bench_name="jahs")
 
 
-@dataclass(frozen=True)
-class _TargetMetricKeys:
-    loss: str = "valid-acc"
-    runtime: str = "runtime"
-    model_size: str = "size_MB"
-
-
-@dataclass(frozen=True)
-class _FidelKeys:
-    epoch: str = "epoch"
-    resol: str = "Resolution"
-
-
-_FIDEL_KEYS = _FidelKeys()
-_TARGET_KEYS = _TargetMetricKeys()
-_DATA_DIR = os.path.join(DATA_DIR_NAME, "jahs")
-_DATASET_NAMES = ["cifar10", "fashion_mnist", "colorectal_histology"]
+_TARGET_KEYS = _TargetMetricKeys(loss="valid-acc", runtime="runtime", model_size="size_MB")
+_BENCH_NAME = "jahs"
+_DATASET_NAMES = DATASET_NAMES[_BENCH_NAME]
 
 
 class JAHSBenchSurrogate(AbstractHPOData):
     """Workaround to prevent dask from serializing the objective func"""
 
-    _data_url = (
-        "https://ml.informatik.uni-freiburg.de/research-artifacts/jahs_bench_201/v1.1.0/assembled_surrogates.tar"
+    _CONSTS = _HPODataClassVars(
+        url="https://ml.informatik.uni-freiburg.de/research-artifacts/jahs_bench_201/v1.1.0/assembled_surrogates.tar",
+        dir=os.path.join(DATA_DIR_NAME, _BENCH_NAME),
     )
-    _data_dir = _DATA_DIR
 
     def __init__(self, dataset_name: str, target_metrics: list[str]):
-        self._check_benchdata_availability()
+        self._validate()
         self._target_metrics = target_metrics[:]
         _metrics = [getattr(_TARGET_KEYS, tm) for tm in self._target_metrics]
         metrics = list(set(_metrics + [_TARGET_KEYS.runtime]))
-        self._surrogate = jahs_bench.Benchmark(task=dataset_name, download=False, save_dir=_DATA_DIR, metrics=metrics)
+        self._surrogate = jahs_bench.Benchmark(
+            task=dataset_name, download=False, save_dir=self._CONSTS.dir, metrics=metrics
+        )
 
     @property
     def install_instruction(self) -> str:
         return (
-            f"$ cd {self._data_dir}\n"
-            f"$ wget {self._data_url}\n\n"
-            f"Then untar `assembled_surrogates.tar` in {self._data_dir}."
+            f"$ cd {self._CONSTS.dir}\n"
+            f"$ wget {self._CONSTS.url}\n\n"
+            f"Then untar `assembled_surrogates.tar` in {self._CONSTS.dir}."
         )
 
     def __call__(self, eval_config: dict[str, int | float | str | bool], fidels: dict[str, int | float]) -> ResultType:
         _fidels = fidels.copy()
-        nepochs = _fidels.pop(_FIDEL_KEYS.epoch)
+        nepochs = _fidels.pop("epoch")
 
-        eval_config.update({"Optimizer": "SGD", **_fidels})  # type: ignore
+        eval_config.update({"Optimizer": "SGD", **_fidels})  # type: ignore[arg-type]
         eval_config = {k: int(v) if k[:-1] == "Op" else v for k, v in eval_config.items()}
         output = self._surrogate(eval_config, nepochs=nepochs)[nepochs]
-        results: ResultType = {RESULT_KEYS.runtime: output[_TARGET_KEYS.runtime]}  # type: ignore
+        results: ResultType = {RESULT_KEYS.runtime: output[_TARGET_KEYS.runtime]}  # type: ignore[misc]
 
         if RESULT_KEYS.loss in self._target_metrics:
-            results[RESULT_KEYS.loss] = float(100 - output[_TARGET_KEYS.loss])  # type: ignore
+            results[RESULT_KEYS.loss] = float(100 - output[_TARGET_KEYS.loss])  # type: ignore[literal-required]
         if RESULT_KEYS.model_size in self._target_metrics:
-            results[RESULT_KEYS.model_size] = float(output[_TARGET_KEYS.model_size])  # type: ignore
+            results[RESULT_KEYS.model_size] = float(output[_TARGET_KEYS.model_size])  # type: ignore[literal-required]
 
         return results
 
+    def __getitem__(self, key: str) -> dict[str, Any]:
+        raise NotImplementedError
+
 
 class JAHSBench201(AbstractBench):
     """The class for JAHS-Bench-201.
 
     Args:
         dataset_id (int):
             The ID of the dataset.
         seed (int | None):
             The random seed to be used.
         target_metrics (list[str]):
             The target metrics to return.
             Must be in ["loss", "runtime", "model_size"].
-        min_epoch (int):
-            The minimum epoch of the training of each neural networks to be used during the optimization.
-        max_epoch (int):
-            The maximum epoch of the training of each neural networks to be used during the optimization.
-        min_resol (float):
-            The minimum resolution of image data for the training of each neural networks.
-        max_resol (float):
-            The maximum resolution of image data for the training of each neural networks.
+        fidel_value_ranges (dict[str, tuple[int | float, int | float]]):
+            The minimum and maximum values for each fidelity values.
+            The keys must be the fidelity names used in each benchmark and each tuple takes lower and upper bounds
+            of each fidelity value.
         keep_benchdata (bool):
             Whether to keep the benchmark data in each instance.
             When True, serialization will happen in case of parallel optimization.
 
     References:
         Title: JAHS-Bench-201: A Foundation For Research On Joint Architecture And Hyperparameter Search
         Authors: A. Bansal et al.
         URL: https://openreview.net/forum?id=_HLcjaVlqJ
 
     NOTE:
         The data is available at:
             https://ml.informatik.uni-freiburg.de/research-artifacts/jahs_bench_201/v1.1.0/assembled_surrogates.tar
     """
 
-    _target_metric: ClassVar[str] = "valid-acc"
-    _N_DATASETS: ClassVar[int] = 3
-    _MAX_EPOCH: ClassVar[int] = 200
-    _TARGET_METRIC_KEYS: ClassVar[list[str]] = [k for k in _TARGET_KEYS.__dict__.keys()]
-    _DATASET_NAMES_FOR_DIR: ClassVar[tuple[str, ...]] = tuple("-".join(name.split("_")) for name in _DATASET_NAMES)
-
-    def __init__(
-        self,
-        dataset_id: int,
-        seed: int | None = None,  # surrogate is not stochastic
-        target_metrics: list[str] = [RESULT_KEYS.loss],
-        min_epoch: int = 22,
-        max_epoch: int = 200,
-        min_resol: float = 0.1,
-        max_resol: float = 1.0,
-        keep_benchdata: bool = True,
-    ):
-        self.dataset_name = _DATASET_NAMES[dataset_id]
-        self._value_range = VALUE_RANGES["jahs"]
-        self._target_metrics = target_metrics[:]
-        self._min_epoch, self._max_epoch = min_epoch, max_epoch
-        self._min_resol, self._max_resol = min_resol, max_resol
-        self._surrogate = self.get_benchdata() if keep_benchdata else None
-
-        self._validate_target_metrics()
-        self._validate_epochs()
-        self._validate_resols()
-
-    def _validate_resols(self) -> None:
-        min_resol, max_resol = self._min_resol, self._max_resol
-        if min_resol <= 0 or max_resol > 1.0:
-            raise ValueError(f"Resolution must be in [0.0, 1.0], but got {min_resol=} and {max_resol=}")
-        if min_resol >= max_resol:
-            raise ValueError(f"min_resol < max_resol must hold, but got {min_resol=} and {max_resol=}")
+    _CONSTS = _BenchClassVars(
+        dataset_names=_DATASET_NAMES,
+        n_datasets=len(_DATASET_NAMES),
+        target_metric_keys=[k for k, v in _TARGET_KEYS.__dict__.items() if v is not None],
+        cont_space=CONT_SPACES[_BENCH_NAME],
+        disc_space=DISC_SPACES[_BENCH_NAME],
+        fidel_space=FIDEL_SPACES[_BENCH_NAME],
+        fidel_keys=_FidelKeys(epoch="epoch", resol="Resolution"),
+    )
 
     def get_benchdata(self) -> JAHSBenchSurrogate:
         return JAHSBenchSurrogate(dataset_name=self.dataset_name, target_metrics=self._target_metrics)
 
     def __call__(  # type: ignore[override]
         self,
         eval_config: dict[str, int | float | str | bool],
         *,
-        fidels: dict[str, int | float] = {},
+        fidels: dict[str, int | float] | None = None,
         seed: int | None = None,
         benchdata: JAHSBenchSurrogate | None = None,
     ) -> ResultType:
-        if benchdata is None and self._surrogate is None:
-            raise ValueError("data must be provided when `keep_benchdata` is False")
+        surrogate = self._validate_benchdata(benchdata)
+        assert surrogate is not None and isinstance(surrogate, JAHSBenchSurrogate)  # mypy redefinition
 
-        _fidels = self.max_fidels
-        _fidels.update(**fidels)
-        surrogate = benchdata if self._surrogate is None else self._surrogate
-        assert surrogate is not None  # mypy redefinition
-        EPS = 1e-12
+        _eval_config, _fidels = self._validate_inputs(eval_config, fidels)
+        assert self._CONSTS.disc_space is not None  # mypy redefinition
         _eval_config = {
-            k: self._value_range[k][int(v)] if k in self._value_range else float(v) for k, v in eval_config.items()
+            k: self._CONSTS.disc_space[k][int(v)] if k in self._CONSTS.disc_space else float(v)
+            for k, v in _eval_config.items()
         }
-        assert isinstance(_eval_config["LearningRate"], float)
-        assert 1e-3 - EPS <= _eval_config["LearningRate"] <= 1.0 + EPS
-        assert isinstance(_eval_config["WeightDecay"], float)
-        assert 1e-5 - EPS <= _eval_config["WeightDecay"] <= 1e-2 + EPS
         return surrogate(eval_config=_eval_config, fidels=_fidels)
-
-    @property
-    def config_space(self) -> CS.ConfigurationSpace:
-        config_space = self._fetch_discrete_config_space()
-        config_space.add_hyperparameters(
-            [
-                CS.UniformFloatHyperparameter(name="LearningRate", lower=1e-3, upper=1.0, log=True),
-                CS.UniformFloatHyperparameter(name="WeightDecay", lower=1e-5, upper=1e-2, log=True),
-            ]
-        )
-        return config_space
-
-    @property
-    def min_fidels(self) -> dict[str, int | float]:
-        return {_FIDEL_KEYS.epoch: self._min_epoch, _FIDEL_KEYS.resol: self._min_resol}
-
-    @property
-    def max_fidels(self) -> dict[str, int | float]:
-        return {_FIDEL_KEYS.epoch: self._max_epoch, _FIDEL_KEYS.resol: self._max_resol}
-
-    @property
-    def fidel_keys(self) -> list[str]:
-        return list(_FIDEL_KEYS.__dict__.values())
```

## benchmark_apis/hpo/lcbench.py

```diff
@@ -1,124 +1,106 @@
 from __future__ import annotations
 
+import json
 import os
-from dataclasses import dataclass
-from typing import ClassVar
+from typing import Any, ClassVar
 
-import ConfigSpace as CS
-
-from benchmark_apis.abstract_interface import AbstractHPOData, RESULT_KEYS, ResultType, _warn_not_found_module
-from benchmark_apis.hpo.abstract_bench import AbstractBench, DATA_DIR_NAME
+from benchmark_apis.abstract_api import (
+    AbstractHPOData,
+    RESULT_KEYS,
+    ResultType,
+    _HPODataClassVars,
+    _TargetMetricKeys,
+    _warn_not_found_module,
+)
+from benchmark_apis.hpo.abstract_bench import (
+    AbstractBench,
+    CONT_SPACES,
+    DATASET_NAMES,
+    DATA_DIR_NAME,
+    FIDEL_SPACES,
+    _BenchClassVars,
+    _FidelKeys,
+)
 
 try:
     from yahpo_gym import benchmark_set, local_config
 except ModuleNotFoundError:
     _warn_not_found_module(bench_name="lcbench")
 
 
-@dataclass(frozen=True)
-class _TargetMetricKeys:
-    loss: str = "val_balanced_accuracy"
-    runtime: str = "time"
-
-
-_TARGET_KEYS = _TargetMetricKeys()
-_FIDEL_KEY = "epoch"
-_DATA_DIR = os.path.join(DATA_DIR_NAME, "lcbench")
-_DATASET_INFO = (
-    ("kddcup09_appetency", "3945"),
-    ("covertype", "7593"),
-    ("amazon_employee_access", "34539"),
-    ("adult", "126025"),
-    ("nomao", "126026"),
-    ("bank_marketing", "126029"),
-    ("shuttle", "146212"),
-    ("australian", "167104"),
-    ("kr_vs_kp", "167149"),
-    ("mfeat_factors", "167152"),
-    ("credit_g", "167161"),
-    ("vehicle", "167168"),
-    ("kc1", "167181"),
-    ("blood_transfusion_service_center", "167184"),
-    ("cnae_9", "167185"),
-    ("phoneme", "167190"),
-    ("higgs", "167200"),
-    ("connect_4", "167201"),
-    ("helena", "168329"),
-    ("jannis", "168330"),
-    ("volkert", "168331"),
-    ("mini_boo_ne", "168335"),
-    ("aps_failure", "168868"),
-    ("christine", "168908"),
-    ("fabert", "168910"),
-    ("airlines", "189354"),
-    ("jasmine", "189862"),
-    ("sylvine", "189865"),
-    ("albert", "189866"),
-    ("dionis", "189873"),
-    ("car", "189905"),
-    ("segment", "189906"),
-    ("fashion_mnist", "189908"),
-    ("jungle_chess_2pcs_raw_endgame_complete", "189909"),
-)
+_TARGET_KEYS = _TargetMetricKeys(loss="val_balanced_accuracy", runtime="time")
+_BENCH_NAME = "lcbench"
+curdir = os.path.dirname(os.path.abspath(__file__))
+_DATASET_NAMES = DATASET_NAMES[_BENCH_NAME]
+DATASET_IDS: dict[str, str] = json.load(open(os.path.join(curdir, "lcbench_dataset_ids.json")))
+_DATASET_INFO = tuple((name, DATASET_IDS[name]) for name in _DATASET_NAMES)
 
 
 class LCBenchSurrogate(AbstractHPOData):
     """Workaround to prevent dask from serializing the objective func"""
 
-    _data_url = "https://syncandshare.lrz.de/getlink/fiCMkzqj1bv1LfCUyvZKmLvd/"
-    _data_dir = _DATA_DIR
+    _CONSTS = _HPODataClassVars(
+        url="https://syncandshare.lrz.de/getlink/fiCMkzqj1bv1LfCUyvZKmLvd/",
+        dir=os.path.join(DATA_DIR_NAME, _BENCH_NAME),
+    )
 
     def __init__(self, dataset_id: str, target_metrics: list[str]):
-        self._check_benchdata_availability()
+        self._validate()
         self._dataset_id = dataset_id
         self._target_metrics = target_metrics[:]
         # active_session=False is necessary for parallel computing.
-        self._surrogate = benchmark_set.BenchmarkSet("lcbench", instance=dataset_id, active_session=False)
+        self._surrogate = benchmark_set.BenchmarkSet(_BENCH_NAME, instance=dataset_id, active_session=False)
 
     @property
     def install_instruction(self) -> str:
         return (
-            f"\tAccess to {self._data_url} and download `lcbench.zip` from the website.\n\n"
-            f"After that, please unzip `lcbench.zip` in {self._data_dir}."
+            f"\tAccess to {self._CONSTS.url} and download `{_BENCH_NAME}.zip` from the website.\n\n"
+            f"After that, please unzip `{_BENCH_NAME}.zip` in {self._CONSTS.dir}."
         )
 
     def _check_benchdata_availability(self) -> None:
         super()._check_benchdata_availability()
         local_config.init_config()
         local_config.set_data_path(DATA_DIR_NAME)
 
-    def __call__(self, eval_config: dict[str, int | float], fidel: int) -> ResultType:
-        _eval_config: dict[str, int | float | str] = eval_config.copy()  # type: ignore
+    def __call__(  # type: ignore[override]
+        self, eval_config: dict[str, int | float], fidels: dict[str, int]
+    ) -> ResultType:
+        _eval_config: dict[str, int | float | str] = eval_config.copy()  # type: ignore[assignment]
         _eval_config["OpenML_task_id"] = self._dataset_id
-        _eval_config[_FIDEL_KEY] = fidel
+        epoch_key = "epoch"
+        _eval_config[epoch_key] = fidels[epoch_key]
 
         output = self._surrogate.objective_function(_eval_config)[0]
-        results: ResultType = {RESULT_KEYS.runtime: float(output[_TARGET_KEYS.runtime])}  # type: ignore
+        results: ResultType = {RESULT_KEYS.runtime: float(output[_TARGET_KEYS.runtime])}  # type: ignore[misc]
         if RESULT_KEYS.loss in self._target_metrics:
-            results[RESULT_KEYS.loss] = float(1.0 - output[_TARGET_KEYS.loss])  # type: ignore
+            results[RESULT_KEYS.loss] = float(1.0 - output[_TARGET_KEYS.loss])  # type: ignore[literal-required]
 
         return results
 
+    def __getitem__(self, key: str) -> dict[str, Any]:
+        raise NotImplementedError
+
 
 class LCBench(AbstractBench):
     """The class for LCBench.
 
     Args:
         dataset_id (int):
             The ID of the dataset.
         seed (int | None):
             The random seed to be used.
         target_metrics (list[str]):
             The target metrics to return.
             Must be in ["loss", "runtime", "model_size"].
-        min_epoch (int):
-            The minimum epoch of the training of each neural networks to be used during the optimization.
-        max_epoch (int):
-            The maximum epoch of the training of each neural networks to be used during the optimization.
+        fidel_value_ranges (dict[str, tuple[int | float, int | float]]):
+            The minimum and maximum values for each fidelity values.
+            The keys must be the fidelity names used in each benchmark and each tuple takes lower and upper bounds
+            of each fidelity value.
         keep_benchdata (bool):
             Whether to keep the benchmark data in each instance.
             When True, serialization will happen in case of parallel optimization.
 
     References:
         1. The original benchmark
         Title: Auto-PyTorch Tabular: Multi-Fidelity MetaLearning for Efficient and Robust AutoDL
@@ -131,89 +113,38 @@
         URL: https://arxiv.org/abs/2109.03670/
 
     NOTE:
         The data is available at:
             https://syncandshare.lrz.de/getlink/fiCMkzqj1bv1LfCUyvZKmLvd/
     """
 
-    _N_DATASETS: ClassVar[int] = 34
-    _TARGET_METRIC_KEYS: ClassVar[list[str]] = [k for k in _TARGET_KEYS.__dict__.keys()]
-    _MAX_EPOCH: ClassVar[int] = 54
-    _TRUE_MAX_EPOCH: ClassVar[int] = 52
-    _DATASET_NAMES_FOR_DIR: ClassVar[tuple[str, ...]] = tuple("-".join(name.split("_")) for name, _ in _DATASET_INFO)
-
-    def __init__(
-        self,
-        dataset_id: int,
-        seed: int | None = None,  # surrogate is not stochastic
-        target_metrics: list[str] = [RESULT_KEYS.loss],
-        min_epoch: int = 6,
-        max_epoch: int = 54,
-        keep_benchdata: bool = True,
-    ):
-        self.dataset_name, self._dataset_id = _DATASET_INFO[dataset_id]
-        self._target_metrics = target_metrics[:]
-        self._surrogate = self.get_benchdata() if keep_benchdata else None
-        self._config_space = self.config_space
-        self._min_epoch, self._max_epoch = min_epoch, max_epoch
+    _CONSTS = _BenchClassVars(
+        dataset_names=_DATASET_NAMES,
+        n_datasets=len(_DATASET_NAMES),
+        target_metric_keys=[k for k, v in _TARGET_KEYS.__dict__.items() if v is not None],
+        cont_space=CONT_SPACES[_BENCH_NAME],
+        fidel_space=FIDEL_SPACES[_BENCH_NAME],
+        fidel_keys=_FidelKeys(epoch="epoch"),
+    )
 
-        self._validate_target_metrics()
-        self._validate_epochs()
+    # LCBench specific constant
+    _TRUE_MAX_EPOCH: ClassVar[int] = 52
 
     def get_benchdata(self) -> LCBenchSurrogate:
-        return LCBenchSurrogate(dataset_id=self._dataset_id, target_metrics=self._target_metrics)
-
-    def _validate_config(self, eval_config: dict[str, int | float]) -> None:
-        EPS = 1e-12
-        for hp in self._config_space.get_hyperparameters():
-            lb, ub, name = hp.lower, hp.upper, hp.name
-            if isinstance(hp, CS.UniformFloatHyperparameter):
-                assert isinstance(eval_config[name], float) and lb - EPS <= eval_config[name] <= ub + EPS
-            else:
-                eval_config[name] = int(eval_config[name])
-                assert isinstance(eval_config[name], int) and lb <= eval_config[name] <= ub
+        _, dataset_id = _DATASET_INFO[self._dataset_id]
+        return LCBenchSurrogate(dataset_id=dataset_id, target_metrics=self._target_metrics)
 
     def __call__(  # type: ignore[override]
         self,
         eval_config: dict[str, int | float],
         *,
-        fidels: dict[str, int] = {},
+        fidels: dict[str, int] | None = None,
         seed: int | None = None,
         benchdata: LCBenchSurrogate | None = None,
     ) -> ResultType:
-        if benchdata is None and self._surrogate is None:
-            raise ValueError("data must be provided when `keep_benchdata` is False")
-
-        surrogate = benchdata if self._surrogate is None else self._surrogate
-        assert surrogate is not None  # mypy redefinition
-        fidel = int(min(self._TRUE_MAX_EPOCH, fidels.get(_FIDEL_KEY, self._max_epoch)))
-        self._validate_config(eval_config=eval_config)
-        return surrogate(eval_config=eval_config, fidel=fidel)
-
-    @property
-    def config_space(self) -> CS.ConfigurationSpace:
-        config_space = CS.ConfigurationSpace()
-        config_space.add_hyperparameters(
-            [
-                CS.UniformIntegerHyperparameter(name="batch_size", lower=16, upper=512, log=True),
-                CS.UniformFloatHyperparameter(name="learning_rate", lower=1e-4, upper=0.1, log=True),
-                CS.UniformFloatHyperparameter(name="max_dropout", lower=0.0, upper=1.0),
-                CS.UniformIntegerHyperparameter(name="max_units", lower=64, upper=1024, log=True),
-                CS.UniformFloatHyperparameter(name="momentum", lower=0.1, upper=0.9),
-                CS.UniformIntegerHyperparameter(name="num_layers", lower=1, upper=5),
-                CS.UniformFloatHyperparameter(name="weight_decay", lower=1e-5, upper=0.1),
-            ]
-        )
-        return config_space
+        surrogate = self._validate_benchdata(benchdata)
+        assert surrogate is not None and isinstance(surrogate, LCBenchSurrogate)  # mypy redefinition
 
-    @property
-    def min_fidels(self) -> dict[str, int]:  # type: ignore[override]
-        return {_FIDEL_KEY: self._min_epoch}
-
-    @property
-    def max_fidels(self) -> dict[str, int]:  # type: ignore[override]
-        # in reality, the max_fidel is 52, but make it 54 only for computational convenience.
-        return {_FIDEL_KEY: self._max_epoch}
-
-    @property
-    def fidel_keys(self) -> list[str]:
-        return [_FIDEL_KEY]
+        epoch_key = self._CONSTS.fidel_keys.epoch
+        _eval_config, _fidels = self._validate_inputs(eval_config=eval_config, fidels=fidels)  # type: ignore[arg-type]
+        _fidels[epoch_key] = int(min(self._TRUE_MAX_EPOCH, _fidels[epoch_key]))
+        return surrogate(eval_config=_eval_config, fidels=_fidels)  # type: ignore[arg-type]
```

## benchmark_apis/synthetic/abstract_func.py

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import ClassVar
 
 import ConfigSpace as CS
 
-from benchmark_apis.abstract_interface import AbstractInterface, RESULT_KEYS, ResultType
+from benchmark_apis.abstract_api import AbstractAPI, RESULT_KEYS, ResultType
 
 import numpy as np
 
 
-class MFAbstractFunc(AbstractInterface):
+class MFAbstractFunc(AbstractAPI):
     """
     Multi-fidelity Function.
 
     Args:
         seed (int | None)
             The random seed for the noise.
         runtime_factor (float):
@@ -33,15 +33,14 @@
             Title: Multi-fidelity Bayesian Optimisation with Continuous Approximations
             Authors: K. Kandasamy et. al
             URL: https://arxiv.org/pdf/1703.06240.pdf
     """
 
     _BENCH_TYPE: ClassVar[str] = "SYNTHETIC"
     _DEFAULT_FIDEL_DIM: ClassVar[int]
-    _DATASET_NAMES_FOR_DIR: ClassVar[tuple[str, ...] | None] = None
 
     def __init__(
         self,
         fidel_dim: int,
         min_fidel: int,
         max_fidel: int,
         seed: int | None,
@@ -58,52 +57,64 @@
 
         self._fidel_dim = fidel_dim
         self._runtime_factor = runtime_factor
         self._dim: int
         self._noise_std: float
         self._min_fidel, self._max_fidel = min_fidel, max_fidel
         self._validate_fidels()
-
-    def _validate_fidels(self) -> None:
-        min_fidel, max_fidel = self._min_fidel, self._max_fidel
-        if min_fidel >= max_fidel:
-            raise ValueError(f"min_fidel < max_fidel must hold, but got {min_fidel=} and {max_fidel=}")
-        if min_fidel <= 0:
-            raise ValueError(f"min_fidel must be in [1, {self._max_fidel}], but got {min_fidel=} and {max_fidel=}")
+        self._validate_class_vars()
 
     @abstractmethod
     def _objective(self, x: np.ndarray, z: np.ndarray) -> float:
         raise NotImplementedError
 
     @abstractmethod
     def _runtime(self, x: np.ndarray, z: np.ndarray) -> float:
         raise NotImplementedError
 
+    @classmethod
+    def _validate_class_vars(cls) -> None:
+        super()._validate_class_vars()
+        if not hasattr(cls, "_DEFAULT_FIDEL_DIM"):
+            raise NotImplementedError(f"Child class of {cls.__name__} must define _DEFAULT_FIDEL_DIM.")
+
+    def _validate_fidels(self) -> None:
+        min_fidel, max_fidel = self._min_fidel, self._max_fidel
+        if min_fidel >= max_fidel:
+            raise ValueError(f"min_fidel < max_fidel must hold, but got {min_fidel=} and {max_fidel=}")
+        if min_fidel <= 0:
+            raise ValueError(f"min_fidel must be in [1, {self._max_fidel}], but got {min_fidel=} and {max_fidel=}")
+
     def _validate_config(self, x: np.ndarray, z: np.ndarray) -> None:
         if np.any((x < 0.0) | (x > 1.0)):
             raise ValueError("All elements in x must be in [0.0, 1.0]")
         if np.any((z < self._min_fidel / self._max_fidel) | (z > 1.0)):
             raise ValueError(f"All elements in fidels must be in [{self._min_fidel}, {self._max_fidel}]")
 
     def __call__(  # type: ignore[override]
         self,
         eval_config: dict[str, float],
         *,
-        fidels: dict[str, int] = {},
+        fidels: dict[str, int] | None = None,
         seed: int | None = None,
     ) -> ResultType:
+        fidels = fidels if fidels is not None else {}
         if len(fidels) != self.fidel_dim:
             raise ValueError(f"The provided fidelity dimension is {self.fidel_dim}, " f"but got {fidels}")
 
         x = np.array([eval_config[f"x{d}"] for d in range(self._dim)])
         z = np.array([fidels[k] / max_fidel for k, max_fidel in self.max_fidels.items()])
         self._validate_config(x=x, z=z)
         loss = self._objective(x=x, z=z)
         runtime = self._runtime(x=x, z=z)
-        return {RESULT_KEYS.loss: loss, RESULT_KEYS.runtime: runtime}  # type: ignore
+        return {RESULT_KEYS.loss: loss, RESULT_KEYS.runtime: runtime}  # type: ignore[misc]
+
+    @property
+    def dataset_name_for_dir(self) -> str | None:
+        return None
 
     @property
     def dim(self) -> int:
         return self._dim
 
     @property
     def fidel_dim(self) -> int:
```

## Comparing `benchmark_apis/abstract_interface.py` & `benchmark_apis/abstract_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import os
 import warnings
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
-from typing import ClassVar, Optional, TypedDict
+from typing import Any, ClassVar, Optional, TypedDict
 
 import ConfigSpace as CS
 
 import numpy as np
 
 
 def _warn_not_found_module(bench_name: str) -> None:
@@ -23,71 +23,103 @@
     loss: str = "loss"
     runtime: str = "runtime"
     model_size: str = "model_size"
     f1: str = "f1"
     precision: str = "precision"
 
 
+@dataclass(frozen=True)
+class _TargetMetricKeys:
+    runtime: str
+    loss: str | None = None
+    model_size: str | None = None
+    f1: str | None = None
+    precision: str | None = None
+
+
+@dataclass(frozen=True)
+class _HPODataClassVars:
+    url: str
+    dir: str
+
+
 class ResultType(TypedDict):
     runtime: float
     loss: Optional[float]
     model_size: Optional[float]
     f1: Optional[float]
     precision: Optional[float]
 
 
 RESULT_KEYS = _ResultKeys()
 
 
 class AbstractHPOData(metaclass=ABCMeta):
-    _data_url: str
-    _data_dir: str
+    _CONSTS: _HPODataClassVars
+
+    @abstractmethod
+    def __call__(self, eval_config: dict[str, int | float | str | bool], fidels: dict[str, int | float]) -> ResultType:
+        raise NotImplementedError
+
+    @abstractmethod
+    def __getitem__(self, key: str) -> dict[str, Any]:
+        raise NotImplementedError
+
+    def _validate(self) -> None:
+        self._validate_class_var()
+        self._check_benchdata_availability()
+
+    @property
+    @abstractmethod
+    def install_instruction(self) -> str:
+        raise NotImplementedError
+
+    @classmethod
+    def _validate_class_var(cls) -> None:
+        if not hasattr(cls, "_CONSTS"):
+            raise NotImplementedError(f"Child class of {cls.__name__} must define _CONSTS.")
 
     @property
     def full_install_instruction(self) -> str:
         return (
-            f"Could not find the dataset at {self._data_dir}.\n"
-            f"Download the dataset and place the file at {self._data_dir}.\n"
+            f"Could not find the dataset at {self._CONSTS.dir}.\n"
+            f"Download the dataset and place the file at {self._CONSTS.dir}.\n"
             "You can download the dataset via:\n"
             f"{self.install_instruction}"
         )
 
-    @property
-    @abstractmethod
-    def install_instruction(self) -> str:
-        raise NotImplementedError
-
     def _check_benchdata_availability(self) -> None:
-        if not os.path.exists(self._data_dir):
+        if not os.path.exists(self._CONSTS.dir):
             raise FileNotFoundError(self.full_install_instruction)
 
 
-class AbstractInterface(metaclass=ABCMeta):
+class AbstractAPI(metaclass=ABCMeta):
     _BENCH_TYPE: ClassVar[str]
-    _DATASET_NAMES_FOR_DIR: ClassVar[tuple[str, ...] | None]
 
     def __init__(self, seed: int | None):
         self._rng = np.random.RandomState(seed)
 
-    def reseed(self, seed: int) -> None:
-        self._rng = np.random.RandomState(seed)
-
     @abstractmethod
     def __call__(
         self,
         eval_config: dict[str, int | float | str | bool],
         *,
-        fidels: dict[str, int | float] = {},
+        fidels: dict[str, int | float] | None = None,
         seed: int | None = None,
         benchdata: AbstractHPOData | None = None,
     ) -> ResultType:
         raise NotImplementedError
 
     @property
     @abstractmethod
+    def dataset_name_for_dir(self) -> str | None:
+        raise NotImplementedError
+
+    @property
+    @abstractmethod
     def config_space(self) -> CS.ConfigurationSpace:
         raise NotImplementedError
 
     @property
     @abstractmethod
     def min_fidels(self) -> dict[str, int | float]:
         # eta ** S <= R/r < eta ** (S + 1) to have S rungs.
@@ -98,7 +130,15 @@
     def max_fidels(self) -> dict[str, int | float]:
         raise NotImplementedError
 
     @property
     @abstractmethod
     def fidel_keys(self) -> list[str]:
         raise NotImplementedError
+
+    def reseed(self, seed: int) -> None:
+        self._rng = np.random.RandomState(seed)
+
+    @classmethod
+    def _validate_class_vars(cls) -> None:
+        if not hasattr(cls, "_BENCH_TYPE"):
+            raise NotImplementedError(f"Child class of {cls.__name__} must define _BENCH_TYPE.")
```

## Comparing `mfhpo_benchmark_api-1.2.0.dist-info/LICENSE` & `mfhpo_benchmark_api-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_benchmark_api-1.2.0.dist-info/METADATA` & `mfhpo_benchmark_api-2.0.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfhpo-benchmark-api
-Version: 1.2.0
+Version: 2.0.0
 Home-page: https://github.com/nabenabe0928/mfhpo-benchmark-api
 Author: nabenabe0928
 Author-email: shuhei.watanabe.utokyo@gmail.com
 Platform: Linux
 Platform: Darwin
 Requires-Python: >=3.8
 License-File: LICENSE
```

## Comparing `mfhpo_benchmark_api-1.2.0.dist-info/RECORD` & `mfhpo_benchmark_api-2.0.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-benchmark_apis/__init__.py,sha256=lStplLjpKjjpRBABYDYpNqzmYRmfa4UsN2en-eLt8go,650
-benchmark_apis/abstract_interface.py,sha256=eXBrviffrrKaofmVdSrKzWf-IYEN8M9qYK1nsQ0dsl0,2689
-benchmark_apis/hpo/abstract_bench.py,sha256=9kNF_E1jO8z1fA4EHQT1yufsAJ9e5MbgHtQSLQQXkjQ,2294
+benchmark_apis/__init__.py,sha256=ME4Wm2lQQvqPfZcGLOwda0bsg5NqSvx-GSBf1hlV3m4,650
+benchmark_apis/abstract_api.py,sha256=LQgiJhe4Pu2MGMpQAuZtlp1rhnLxXnm5xhpbXLZUjNY,3814
+benchmark_apis/hpo/abstract_bench.py,sha256=XxIC6j45_UpmnkWgbZJUCGGTLXUstF4dDR6wowogP80,10074
+benchmark_apis/hpo/continuous_search_spaces.json,sha256=cqN2uwBH9f5kQe97d91oJZoLT4XysR4gg8aoXqAC5QI,795
+benchmark_apis/hpo/dataset_names.json,sha256=mGKQtfxekNO6_DkWlLgY-1SefMzXKhQ56wshZyp476A,1196
 benchmark_apis/hpo/discrete_search_spaces.json,sha256=S8gLxrA_vweXVuPHU-TNfq8C4GrLSQQsxgeMdxEjz58,2975
-benchmark_apis/hpo/hpobench.py,sha256=hHQg6u5lb-7r_iZjHbiKgQc1Wz-hscDTb7dQuLau7cE,6398
-benchmark_apis/hpo/hpolib.py,sha256=g1jOussgTmAsNNcRWDiiLy_O4zXrCtdzlswMvve0MeU,6269
-benchmark_apis/hpo/jahs.py,sha256=iZ0-KzkR1h71lNBt0upH_5lnmadd6UfE--sp3yC2ruk,7783
-benchmark_apis/hpo/lcbench.py,sha256=MzbqMVsCqWnKAkYcbTRY7NLOzXYO5St2BEycSRS4qd4,8491
-benchmark_apis/synthetic/abstract_func.py,sha256=sszss8esQzRjJR9gUfPUUSD7Goiu0nkcXN-_Y22sMa0,4701
+benchmark_apis/hpo/fidel_spaces.json,sha256=BJ3HGEaudHPPfbaG-f3bL3RSQS3Hxlm1TKCjecRsw4k,736
+benchmark_apis/hpo/hpobench.py,sha256=rp9TQzv_ob3tBYOP8R_QToXReuxqE5ghXjEuM75JxUQ,5487
+benchmark_apis/hpo/hpolib.py,sha256=q5NlqGx1BkGzmrK6TRmoi-bNzQdrIH6e2vk_TMGj5aQ,5301
+benchmark_apis/hpo/jahs.py,sha256=ftuwEl2-jPHFRd5PIcMzE4KXRPqiY6-kk5O7mJzbM7E,5354
+benchmark_apis/hpo/lcbench.py,sha256=rbwcn7oSuqVzmBLL_w8yTmX41SgWMMfp4xgOirJVh5k,5690
+benchmark_apis/hpo/lcbench_dataset_ids.json,sha256=3TzWwTsAon10mlYsaOmbYHJq7xgBPLRlU9fq0aL0m0A,948
+benchmark_apis/synthetic/abstract_func.py,sha256=fzO-mxIO_hTlGIeoGU0uXaiqppLh9mn_9CsPBWRoMzk,5060
 benchmark_apis/synthetic/branin.py,sha256=Ff0_W9_cebQYptHjeZG9dBC46aenO8oXDodbMVrtSTs,3727
 benchmark_apis/synthetic/hartmann.py,sha256=iHj6mX5Ms8ybsvFbOBZILB68qmVWkrHOD_Xlay1ZwiU,4593
-mfhpo_benchmark_api-1.2.0.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_benchmark_api-1.2.0.dist-info/METADATA,sha256=fkCcKH5H-IfHkncVzBD8RvYQL04wD2dB2XhYAV6UxqM,564
-mfhpo_benchmark_api-1.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_benchmark_api-1.2.0.dist-info/top_level.txt,sha256=lEJLF938TxZ1sBYcMCtargVhl1LMgTSzQetZwwmQMiM,59
-mfhpo_benchmark_api-1.2.0.dist-info/RECORD,,
+mfhpo_benchmark_api-2.0.0.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_benchmark_api-2.0.0.dist-info/METADATA,sha256=jXDXO3yf14cohO2cAcJsqyGPvGPjUP9Ry7oPYqFIr1k,564
+mfhpo_benchmark_api-2.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mfhpo_benchmark_api-2.0.0.dist-info/top_level.txt,sha256=lEJLF938TxZ1sBYcMCtargVhl1LMgTSzQetZwwmQMiM,59
+mfhpo_benchmark_api-2.0.0.dist-info/RECORD,,
```

