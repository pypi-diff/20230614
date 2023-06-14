# Comparing `tmp/stringcalc-0.1.0.dev7.tar.gz` & `tmp/stringcalc-0.1.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringcalc-0.1.0.dev7.tar", last modified: Mon Mar 27 19:02:15 2023, max compression
+gzip compressed data, was "stringcalc-0.1.0.dev8.tar", last modified: Wed Jun 14 03:07:40 2023, max compression
```

## Comparing `stringcalc-0.1.0.dev7.tar` & `stringcalc-0.1.0.dev8.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0      862 2023-03-22 21:57:03.372415 stringcalc-0.1.0.dev7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1974 2022-04-25 16:28:20.965299 stringcalc-0.1.0.dev7/.gitignore
--rw-r--r--   0        0        0      786 2023-03-22 21:57:03.401915 stringcalc-0.1.0.dev7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1090 2022-04-25 16:28:20.965799 stringcalc-0.1.0.dev7/LICENSE
--rw-r--r--   0        0        0      601 2023-03-27 18:04:37.236255 stringcalc-0.1.0.dev7/README.md
--rw-r--r--   0        0        0     3524 2023-03-27 18:03:35.117846 stringcalc-0.1.0.dev7/docs/prior-art.md
--rw-r--r--   0        0        0     1476 2023-03-22 21:57:03.402415 stringcalc-0.1.0.dev7/pyproject.toml
--rw-r--r--   0        0        0       77 2023-03-27 19:01:38.443643 stringcalc-0.1.0.dev7/stringcalc/__init__.py
--rw-r--r--   0        0        0    12011 2023-03-27 17:24:58.452201 stringcalc-0.1.0.dev7/stringcalc/cli.py
--rw-r--r--   0        0        0   124808 2023-03-24 20:14:28.941212 stringcalc-0.1.0.dev7/stringcalc/data/daddario-tension.csv
--rw-r--r--   0        0        0     3545 2023-03-22 21:57:03.404915 stringcalc-0.1.0.dev7/stringcalc/frets.py
--rw-r--r--   0        0        0     8501 2023-03-22 21:57:03.405416 stringcalc-0.1.0.dev7/stringcalc/tension.py
--rw-r--r--   0        0        0     2261 2023-03-22 21:57:03.406416 stringcalc-0.1.0.dev7/tests/test_frets.py
--rw-r--r--   0        0        0     2927 2023-03-24 20:14:28.942211 stringcalc-0.1.0.dev7/tests/test_string.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 stringcalc-0.1.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0     1533 2023-06-14 03:03:08.620029 stringcalc-0.1.0.dev8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1974 2022-04-25 16:28:20.965299 stringcalc-0.1.0.dev8/.gitignore
+-rw-r--r--   0        0        0      786 2023-05-31 22:35:00.127306 stringcalc-0.1.0.dev8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1090 2022-04-25 16:28:20.965799 stringcalc-0.1.0.dev8/LICENSE
+-rw-r--r--   0        0        0      608 2023-05-31 22:01:53.642624 stringcalc-0.1.0.dev8/README.md
+-rw-r--r--   0        0        0     3524 2023-03-27 18:03:35.117846 stringcalc-0.1.0.dev8/docs/prior-art.md
+-rw-r--r--   0        0        0     1446 2023-06-14 03:03:08.623529 stringcalc-0.1.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-14 03:06:55.308398 stringcalc-0.1.0.dev8/stringcalc/__init__.py
+-rw-r--r--   0        0        0    12011 2023-03-28 16:06:30.394364 stringcalc-0.1.0.dev8/stringcalc/cli.py
+-rw-r--r--   0        0        0       30 2023-06-14 03:03:08.624030 stringcalc-0.1.0.dev8/stringcalc/data/__init__.py
+-rw-r--r--   0        0        0     1762 2023-06-14 03:03:08.624529 stringcalc-0.1.0.dev8/stringcalc/data/aquila-nng.csv
+-rw-r--r--   0        0        0   124808 2023-03-24 20:14:28.941212 stringcalc-0.1.0.dev8/stringcalc/data/daddario-tension.csv
+-rw-r--r--   0        0        0      288 2023-06-14 03:03:08.625029 stringcalc-0.1.0.dev8/stringcalc/data/worth.csv
+-rw-r--r--   0        0        0     3576 2023-06-14 03:03:08.626029 stringcalc-0.1.0.dev8/stringcalc/frets.py
+-rw-r--r--   0        0        0    11202 2023-06-14 03:03:08.627030 stringcalc-0.1.0.dev8/stringcalc/tension.py
+-rw-r--r--   0        0        0     2260 2023-06-14 03:03:08.627529 stringcalc-0.1.0.dev8/tests/test_frets.py
+-rw-r--r--   0        0        0     3124 2023-06-14 03:03:08.628529 stringcalc-0.1.0.dev8/tests/test_string.py
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 stringcalc-0.1.0.dev8/PKG-INFO
```

### Comparing `stringcalc-0.1.0.dev7/.gitignore` & `stringcalc-0.1.0.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev7/.pre-commit-config.yaml` & `stringcalc-0.1.0.dev8/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,26 @@
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-yaml
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: "v3.3.1"
+    rev: "v3.4.0"
     hooks:
       - id: pyupgrade
-        args: [--py38-plus]
+        args: [--py39-plus]
 
   - repo: https://github.com/PyCQA/isort
     rev: "5.12.0"
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: "23.1.0"
+    rev: "23.3.0"
     hooks:
       - id: black
 
   - repo: https://github.com/csachs/pyproject-flake8
     rev: "v6.0.0.post1"
     hooks:
       - id: pyproject-flake8 # pflake8
```

### Comparing `stringcalc-0.1.0.dev7/LICENSE` & `stringcalc-0.1.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev7/README.md` & `stringcalc-0.1.0.dev8/README.md`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-# stringcalc
-
-*Calculations for [string instrument](https://en.wikipedia.org/wiki/String_instrument)s' strings*
-
-[![CI workflow status](https://github.com/zmoon/stringcalc/actions/workflows/ci.yml/badge.svg)](https://github.com/zmoon/stringcalc/actions/workflows/ci.yml)
-[![Version on PyPI](https://img.shields.io/pypi/v/stringcalc.svg)](https://pypi.org/project/stringcalc/)
-[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
+# stringcalc
+
+*Calculations for [string instrument](https://en.wikipedia.org/wiki/String_instrument)s' strings*
+
+[![CI workflow status](https://github.com/zmoon/stringcalc/actions/workflows/ci.yml/badge.svg)](https://github.com/zmoon/stringcalc/actions/workflows/ci.yml)
+[![Version on PyPI](https://img.shields.io/pypi/v/stringcalc.svg)](https://pypi.org/project/stringcalc/)
+[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
```

### Comparing `stringcalc-0.1.0.dev7/docs/prior-art.md` & `stringcalc-0.1.0.dev8/docs/prior-art.md`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev7/pyproject.toml` & `stringcalc-0.1.0.dev8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 [project]
 name = "stringcalc"
 authors = [{name = "zmoon", email = "zmoon92@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
-requires-python = "~=3.8"
+requires-python = "~=3.9"
 dependencies = [
     "numpy >=1.21",
     "pandas",
-    "pint",
-    # "pyabc2 @ https://github.com/zmoon/PyABC2/archive/main.zip",
+    "pint >=0.22",
     "pyabc2",
 ]
 
 [project.urls]
 Home = "https://github.com/zmoon/stringcalc"
 Source = "https://github.com/zmoon/stringcalc"
 
@@ -31,14 +30,17 @@
 dev = [
     "ipython",
 ]
 cli = [
     "rich",
     "typer",
 ]
+doc = [
+    "matplotlib",
+]
 
 [project.scripts]
 stringcalc = "stringcalc.cli:app"
 
 [tool.flit.sdist]
 exclude = ["data/"]
```

### Comparing `stringcalc-0.1.0.dev7/stringcalc/cli.py` & `stringcalc-0.1.0.dev8/stringcalc/cli.py`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev7/stringcalc/data/daddario-tension.csv` & `stringcalc-0.1.0.dev8/stringcalc/data/daddario-tension.csv`

 * *Files identical despite different names*

### Comparing `stringcalc-0.1.0.dev7/stringcalc/frets.py` & `stringcalc-0.1.0.dev8/stringcalc/frets.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,11 +119,11 @@
         su_si = "in"
     elif units.lower() in {"mm"}:
         su_l = su_si = "mm"
     else:
         raise ValueError(f"invalid `units` {units!r}")
 
     print(f'L = {L}" (scale length)')
-    print(df.to_string(float_format=float_format))
+    print(df.to_string(float_format=float_format))  # type: ignore[call-overload]
     l = max(len(s) for s in df.attrs["col_desc"])  # noqa: E741
     for k, v in df.attrs["col_desc"].items():
         print(f"{k:{l+2}}{v}{'' if k == 'n' else f' ({su_si})'}")
```

### Comparing `stringcalc-0.1.0.dev7/stringcalc/tension.py` & `stringcalc-0.1.0.dev8/stringcalc/tension.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,36 +7,134 @@
 """
 from __future__ import annotations
 
 import math
 import re
 import warnings
 from functools import lru_cache
-from pathlib import Path
 from typing import NamedTuple
 
 import pandas as pd
 
-HERE = Path(__file__).parent
-DATA = HERE / "data"
+
+def _get_data():
+    from importlib.resources import files
+
+    from . import data
+
+    return files(data)
+
+
+DATA = _get_data()
+
+
+@lru_cache(1)
+def load_data() -> pd.DataFrame:
+    """Load all string data.
+
+    Use the individual `load_*_data` functions for more control.
+    """
+    import itertools
+
+    daddario = load_daddario_data()
+    aquila = load_aquila_data()
+    worth = load_worth_data().drop(columns="rho")
+
+    # Check no overlap in group IDs
+    # TODO: move to test suite?
+    for a, b in itertools.product(
+        [
+            set(daddario.group_id.cat.categories),
+            set(aquila.group_id.cat.categories),
+            set(worth.group_id.cat.categories),
+        ],
+        repeat=2,
+    ):
+        if a is b:
+            continue
+        if a & b:
+            raise AssertionError(f"Group IDs {a & b} found in multiple datasets.")
+
+    df = pd.concat(
+        [
+            daddario,
+            aquila,
+            worth,
+        ],
+        ignore_index=True,
+    )
+
+    for name in ["group", "group_id"]:
+        df[name] = df[name].astype("category")
+
+    return df
 
 
 @lru_cache(2)
-def load_data(*, drop_sample_tensions=True):
+def load_daddario_data(*, drop_sample_tensions: bool = True) -> pd.DataFrame:
     """Load the data (currently only D'Addario) needed for the calculations."""
 
-    df = pd.read_csv(DATA / "daddario-tension.csv", header=0)
-    # TODO: use importlib.resources
+    df = pd.read_csv(DATA.joinpath("daddario-tension.csv"), header=0).convert_dtypes()
 
     if drop_sample_tensions:
         df = df.drop(columns=["notes", "tens"])
 
     # Set categorical columns
-    df = df.convert_dtypes()
-    for name in ["category", "group", "id_pref", "group_id"]:
+    for name in ["category", "group", "id_pref", "id_suff", "group_id"]:
+        df[name] = df[name].astype("category")
+
+    return df
+
+
+@lru_cache
+def load_aquila_data(*, nng_density: float = 1300, drop_gauge_eqvs: bool = True) -> pd.DataFrame:
+    """Load Aquila NNG (New Nylgut) data.
+
+    Parameters
+    ----------
+    nng_density
+        Assumed density of Aquila NNG strings, in kg/m3.
+        They are supposed to be the same density as gut.
+        https://www.cs.helsinki.fi/u/wikla/mus/Calcs/wwwscalc.html says gut is 1276 kg/m3;
+        I have seen 1300 elsewhere.
+    """
+    import numpy as np
+
+    df = pd.read_csv(DATA.joinpath("aquila-nng.csv"), header=0).convert_dtypes()
+
+    # Compute UW
+    # TODO: use Pint
+    df["uw"] = nng_density * 2.205 / 1e6 * (2.54**3) * (np.pi * df.gauge**2 / 4)
+
+    # Set group ID (used to select string type)
+    df["group"] = "Aquila New Nylgut"
+    df["group_id"] = "NNG"
+    for name in ["group", "group_id"]:
+        df[name] = df[name].astype("category")
+
+    # Include gauge equivalents?
+    gauge_eqv_cols = [col for col in df.columns if col.startswith("gauge_")]
+    if drop_gauge_eqvs:
+        df = df.drop(columns=gauge_eqv_cols)
+    else:
+        df = df.rename(columns={col: col.replace("gauge_", "gauge_eqv_") for col in gauge_eqv_cols})
+
+    return df
+
+
+@lru_cache(1)
+def load_worth_data() -> pd.DataFrame:
+    """Load Worth fluorocarbon data."""
+
+    df = pd.read_csv(DATA.joinpath("worth.csv"), header=0).convert_dtypes()
+
+    # Set group ID (used to select string type)
+    df["group"] = "Worth Fluorocarbon"
+    df["group_id"] = "WFC"
+    for name in ["group", "group_id"]:
         df[name] = df[name].astype("category")
 
     return df
 
 
 _re_string_spec = re.compile(
     r"(?P<L>[\.0-9]+)"
@@ -171,15 +269,15 @@
     # i.e., it is gravity in the units of the RHS (seconds and inches)
     # gc = (9.80665 m s-2) * (3.28084 ft m-1) * (12 in ft-1)
     #    = 386.09 in s-2  (technically [in lbm lbf-1 s-2])
     #
     # At g0, 1 lbm exerts a force of 1 lbf => lbf = g0 lbm = 32.174 lbm ft s-2
     # https://en.wikipedia.org/wiki/Gc_(engineering)
 
-    UW = float(rows.uw)
+    UW = float(rows.uw.iloc[0])
     F = Pitch.from_name(pitch).etf
 
     T = UW * (2 * L * F) ** 2 / 386.09
 
     return T
```

### Comparing `stringcalc-0.1.0.dev7/tests/test_frets.py` & `stringcalc-0.1.0.dev8/tests/test_frets.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         -0.1,
         [-2, -1],
         [-1, 0, 1],
     ],
 )
 def test_d_et_invalid(n):
     with pytest.raises(ValueError, match="input fret numbers should be positive"):
-        frets.distance_et(n=-1, L=25)
+        frets.distance_et(n=n, L=25)
 
 
 @pytest.mark.parametrize(
     "ab, d, expected",
     [
         ((0, 2), 2, 18.332),
         ((2, None), 16.3316, 18.332),
```

### Comparing `stringcalc-0.1.0.dev7/tests/test_string.py` & `stringcalc-0.1.0.dev8/tests/test_string.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pytest
 
 from stringcalc.tension import (
     _STRING_TYPE_ALIASES,
     String,
     gauge,
+    load_data,
     suggest_gauge,
     tension,
     unit_weight,
 )
 
 
 @pytest.mark.parametrize(
@@ -112,7 +113,14 @@
     all_aliases = list(
         itertools.chain.from_iterable(aliases for aliases in _STRING_TYPE_ALIASES.values())
     )
     verbose_keys = _STRING_TYPE_ALIASES.keys()
     all_aliases_set = set(all_aliases)
     assert len(all_aliases) == len(all_aliases_set)
     assert len(all_aliases + list(verbose_keys)) == len(all_aliases_set | verbose_keys)
+
+
+def test_load_data_categories():
+    df = load_data()
+
+    for name in ["category", "group", "id_pref", "id_suff", "group_id"]:
+        assert df[name].dtype == "category"
```

### Comparing `stringcalc-0.1.0.dev7/PKG-INFO` & `stringcalc-0.1.0.dev8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: stringcalc
-Version: 0.1.0.dev7
+Version: 0.1.0.dev8
 Summary: Calculations for instrument strings
 Author-email: zmoon <zmoon92@gmail.com>
-Requires-Python: ~=3.8
+Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy >=1.21
 Requires-Dist: pandas
-Requires-Dist: pint
+Requires-Dist: pint >=0.22
 Requires-Dist: pyabc2
 Requires-Dist: rich ; extra == "cli"
 Requires-Dist: typer ; extra == "cli"
 Requires-Dist: ipython ; extra == "dev"
+Requires-Dist: matplotlib ; extra == "doc"
 Requires-Dist: mypy ; extra == "test"
 Requires-Dist: pandas-stubs ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Project-URL: Home, https://github.com/zmoon/stringcalc
 Project-URL: Source, https://github.com/zmoon/stringcalc
 Provides-Extra: cli
 Provides-Extra: dev
+Provides-Extra: doc
 Provides-Extra: test
 
 # stringcalc
 
 *Calculations for [string instrument](https://en.wikipedia.org/wiki/String_instrument)s' strings*
 
 [![CI workflow status](https://github.com/zmoon/stringcalc/actions/workflows/ci.yml/badge.svg)](https://github.com/zmoon/stringcalc/actions/workflows/ci.yml)
```

