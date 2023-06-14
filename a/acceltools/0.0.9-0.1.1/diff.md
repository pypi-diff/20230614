# Comparing `tmp/acceltools-0.0.9-py3-none-any.whl.zip` & `tmp/acceltools-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 18212 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat       22 b- defN 22-Jun-29 05:54 acceltools/__init__.py
--rw-rw-rw-  2.0 fat      659 b- defN 22-Jun-06 00:52 acceltools/base.py
--rw-rw-rw-  2.0 fat     9186 b- defN 22-Jun-13 05:27 acceltools/ecd.py
--rw-rw-rw-  2.0 fat    28227 b- defN 22-Jun-07 11:40 acceltools/nmr.py
--rw-rw-rw-  2.0 fat     7187 b- defN 22-Jun-28 10:57 acceltools/plot.py
--rw-rw-rw-  2.0 fat     6258 b- defN 22-Jun-06 02:32 acceltools/series.py
--rw-rw-rw-  2.0 fat     1078 b- defN 22-Jun-08 07:49 acceltools/table.py
+Zip file size: 18965 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat       22 b- defN 22-Nov-25 03:17 acceltools/__init__.py
+-rw-rw-rw-  2.0 fat      672 b- defN 22-Aug-23 03:58 acceltools/base.py
+-rw-rw-rw-  2.0 fat     9265 b- defN 22-Aug-23 03:58 acceltools/ecd.py
+-rw-rw-rw-  2.0 fat    29152 b- defN 22-Aug-23 03:58 acceltools/nmr.py
+-rw-rw-rw-  2.0 fat     7041 b- defN 22-Aug-23 03:58 acceltools/plot.py
+-rw-rw-rw-  2.0 fat     7619 b- defN 22-Nov-25 03:05 acceltools/series.py
+-rw-rw-rw-  2.0 fat     1039 b- defN 22-Aug-23 03:58 acceltools/table.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-May-14 04:49 acceltools/future/__init__.py
 -rw-rw-rw-  2.0 fat    14773 b- defN 22-Jun-02 03:40 acceltools/future/doc.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-29 01:57 acceltools/future/mm.py
--rw-rw-rw-  2.0 fat     1059 b- defN 22-Jun-29 05:54 acceltools-0.0.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      556 b- defN 22-Jun-29 05:54 acceltools-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jun-29 05:54 acceltools-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 22-Jun-29 05:54 acceltools-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1170 b- defN 22-Jun-29 05:54 acceltools-0.0.9.dist-info/RECORD
-15 files, 70278 bytes uncompressed, 16288 bytes compressed:  76.8%
+-rw-rw-rw-  2.0 fat     1059 b- defN 22-Nov-25 03:17 acceltools-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      555 b- defN 22-Nov-25 03:17 acceltools-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Nov-25 03:17 acceltools-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 22-Nov-25 03:17 acceltools-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1170 b- defN 22-Nov-25 03:17 acceltools-0.1.1.dist-info/RECORD
+15 files, 72470 bytes uncompressed, 17041 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: acceltools/future/doc.py
 Comment: 
 
 Filename: acceltools/future/mm.py
 Comment: 
 
-Filename: acceltools-0.0.9.dist-info/LICENSE
+Filename: acceltools-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: acceltools-0.0.9.dist-info/METADATA
+Filename: acceltools-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: acceltools-0.0.9.dist-info/WHEEL
+Filename: acceltools-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: acceltools-0.0.9.dist-info/top_level.txt
+Filename: acceltools-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: acceltools-0.0.9.dist-info/RECORD
+Filename: acceltools-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## acceltools/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.9"
+__version__ = "0.1.1"
```

## acceltools/base.py

```diff
@@ -1,25 +1,20 @@
 from typing import Iterable, Union
 
-from accel import Mol
 from accel.base.box import Box
-from accel.base.mols import Mols
+from accel.base.systems import System, Systems
 
 
 class ToolBox:
-    def __init__(self, box: Union[Box, Mols, Iterable[Mol], Mol]):
-        if isinstance(box, Box):
-            self._mols: Mols = box.mols
-        elif isinstance(box, Mols):
-            self._mols: Mols = box
-        elif isinstance(box, Mol):
-            self._mols: Mols = Mols().append(box)
+    def __init__(self, contents: Union[Box, Systems, Iterable[System], System]):
+        if isinstance(contents, Box):
+            self.contents: Systems = contents.get()
+        elif isinstance(contents, Systems):
+            self.contents: Systems = contents
+        elif isinstance(contents, System):
+            self.contents: Systems = Systems()
+            self.contents.append(contents)
         else:
-            self._mols: Mols = Box(box).mols
+            self.contents: Systems = Box(contents).get()
 
-    @property
-    def mols(self):
-        return self._mols.has_state(True)
-
-    @property
-    def allmols(self) -> Mols:
-        return self._mols.has_state(None)
+    def get(self) -> Systems:
+        return self.contents.has_state(True)
```

## acceltools/ecd.py

```diff
@@ -2,70 +2,70 @@
 from copy import deepcopy
 from pathlib import Path
 from typing import Iterable, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from accel.base.box import Box
-from accel.base.mols import Mol, Mols
+from accel.base.systems import System, Systems
 from accel.util.log import logger
 
 from acceltools.base import ToolBox
 
 
 def get_average(
-    mols: Mols, averaged_mols: Mols = None, ecd_key="ecd", weighted_keys=["R_velocity", "R_length", "f"]
-) -> Mols:
-    if averaged_mols is None:
-        averaged_mols = Box().bind(mols).get_average()
-    for ave in averaged_mols:
+    systems: Systems, averaged_systems: Systems = None, ecd_key="ecd", weighted_keys=["R_velocity", "R_length", "f"]
+) -> Systems:
+    if averaged_systems is None:
+        averaged_systems = Box().bind(systems).get_average()
+    for ave in averaged_systems:
         ecd_dict = {}
-        confs = mols.has_state().has_label(ave.name)
+        confs = systems.has_state().has_label(ave.name)
         for idx in range(len(confs)):
             for state_number, state_dict in confs[idx].data[ecd_key].items():
                 w_state = deepcopy(state_dict)
                 for _key in weighted_keys:
                     if _key not in w_state:
                         logger.error(f"weighted key {_key} not found in data {ecd_key}")
                         continue
                     w_state[_key] *= confs[idx].distribution
                 ecd_dict[f"{idx}_{confs[idx].name}_{state_number}"] = w_state
         ave.data["ecd"] = ecd_dict
-    return averaged_mols
+    return averaged_systems
 
 
 class EcdBox(ToolBox):
-    def __init__(self, box: Union[Box, Mols, Iterable[Mol], Mol]):
+    def __init__(self, contents: Union[Box, Systems, Iterable[System], System]):
         self.expt: list[tuple[float]] = []
         self.expt_uv: list[tuple[float]] = []
         self.ecd_key: str = "ecd"
         self.curve_key: str = "ecd_curve"
         self.curve_key_uv: str = "uv_curve"
         self.nm_ev: float = 1239.84193
         self.const: float = 22.97
         self.const_uv: float = 28700.0
         self.calc_start: float = 100
         self.calc_stop: float = 800
         self.calc_step: float = 0.1
-        super().__init__(box)
+        super().__init__(contents)
 
     def load_expt(self, filepath: Union[Path, str], x_column: int = 1, y_column: int = 2, start_row: int = 2):
         with Path(filepath).open() as f:
             ls = [_l for _l in csv.reader(f)]
         self.expt = []
         for _l in ls[(start_row - 1) :]:
             self.expt.append((float(_l[x_column - 1]), float(_l[y_column - 1])))
         return self
 
-    def get_average(self) -> Mols:
-        return get_average(self.mols, ecd_key=self.ecd_key)
+    def get_average(self) -> Systems:
+        return get_average(self.get(), ecd_key=self.ecd_key)
 
     def calc_curve(self, half_width: float = 0.19, shift: float = 0.0, scale: float = 1.0, key: str = "R_velocity"):
         x_values = np.arange(self.calc_start, self.calc_stop, self.calc_step)
-        for _c in self.mols:
+        for _c in self.get():
             y_values = np.zeros(len(x_values))
             for state_num in _c.data[self.ecd_key]:
                 _d: dict[str, Union[float, str]] = _c.data[self.ecd_key][state_num]
                 y_values += (
                     _d["energy"]
                     * _d[key]
                     * np.exp(-1 * np.square(((self.nm_ev / x_values) - _d["energy"]) / half_width))
@@ -74,15 +74,15 @@
             y_values *= scale
             _c.data[self.curve_key] = [(x + shift, y) for x, y in zip(x_values, y_values)]
             logger.info(f"ECD of {_c.name} calculated: half-width {half_width}, shift {shift} and scale {scale}")
         return self
 
     def calc_curve_uv(self, half_width: float = 0.19, shift: float = 0.0, scale: float = 1.0, key: str = "f"):
         x_values = np.arange(self.calc_start, self.calc_stop, self.calc_step)
-        for _c in self.mols:
+        for _c in self.get():
             y_values = np.zeros(len(x_values))
             for state_num in _c.data[self.ecd_key]:
                 _d: dict[str, Union[float, str]] = _c.data[self.ecd_key][state_num]
                 y_values += (
                     _d["energy"]
                     * _d[key]
                     * np.exp(-1 * np.square(((self.nm_ev / x_values) - _d["energy"]) / half_width))
@@ -102,20 +102,20 @@
         with_expt: bool = True,
         with_ent: bool = False,
         with_bar: bool = False,
         transparent: bool = False,
     ):
         if max_strength is None:
             abs_max = 0.0
-            for _c in self.mols:
+            for _c in self.get():
                 x_vals = [abs(xy[1]) for xy in _c.data[self.curve_key] if start <= xy[0] and xy[0] <= stop]
                 abs_max = max([abs_max] + x_vals)
             max_strength = abs_max * 1.1
         Path(directory).mkdir(exist_ok=True)
-        for _c in self.mols:
+        for _c in self.get():
             if max_strength == 0:
                 max_strength = max([abs(xy[1]) for xy in _c.data[self.curve_key] if start <= xy[0] and xy[0] <= stop])
             fig = plt.figure()
             ax = fig.add_subplot(1, 1, 1)
             ax.set_xlim(start, stop)
             ax.set_ylim(-max_strength, max_strength)
             ax.plot(
@@ -165,20 +165,20 @@
         max_strength: float = None,
         with_expt: bool = True,
         with_bar: bool = False,
         transparent: bool = False,
     ):
         if max_strength is None:
             abs_max = 0.0
-            for _c in self.mols:
+            for _c in self.get():
                 x_vals = [abs(xy[1]) for xy in _c.data[self.curve_key_uv] if start <= xy[0] and xy[0] <= stop]
                 abs_max = max([abs_max] + x_vals)
             max_strength = abs_max * 1.1
         Path(directory).mkdir(exist_ok=True)
-        for _c in self.mols:
+        for _c in self.get():
             if max_strength == 0:
                 max_strength = max(
                     [abs(xy[1]) for xy in _c.data[self.curve_key_uv] if start <= xy[0] and xy[0] <= stop]
                 )
             fig = plt.figure()
             ax = fig.add_subplot(1, 1, 1)
             ax.set_xlim(start, stop)
@@ -204,26 +204,26 @@
             plt.savefig(_p, transparent=transparent, dpi=600)
             logger.info(f"UV spectra of {_c.name} plotted")
             plt.close()
         return self
 
     def write_csv(self, directory: Path):
         Path(directory).mkdir(exist_ok=True)
-        for c in self.mols:
+        for c in self.get():
             p = Path(directory).joinpath(c.name).with_suffix(".csv")
             with p.open("w", newline="") as f:
                 w = csv.writer(f)
-                w.writerow(["X (nm)", "Y (Mol-1cm-1)"])
+                w.writerow(["X (nm)", "Y (System-1cm-1)"])
                 w.writerows(c.data[self.curve_key])
             logger.info(f"curve data was exported as {p.name}")
         return self
 
     def write_csv_uv(self, directory: Path):
         Path(directory).mkdir(exist_ok=True)
-        for c in self.mols:
+        for c in self.get():
             p = Path(directory).joinpath(c.name).with_suffix(".csv")
             with p.open("w", newline="") as f:
                 w = csv.writer(f)
-                w.writerow(["X (nm)", "Y (Mol-1cm-1)"])
+                w.writerow(["X (nm)", "Y (System-1cm-1)"])
                 w.writerows(c.data[self.curve_key_uv])
             logger.info(f"curve data was exported as {p.name}")
         return self
```

## acceltools/nmr.py

```diff
@@ -1,15 +1,15 @@
 import csv
 from collections.abc import MutableSequence
 from pathlib import Path
-from typing import Iterator, Union
+from typing import Iterable, Iterator, Union
 
 import numpy as np
 from accel.base.box import Box
-from accel.base.mols import Mol, Mols
+from accel.base.systems import System, Systems
 from accel.util.constants import Elements
 from accel.util.datadict import Data
 from accel.util.log import logger
 from scipy import stats
 
 from acceltools.base import ToolBox
 
@@ -215,31 +215,34 @@
             if _l[3] != "":
                 _peaks[_i].dtopic = _peaks[int(_l[3]) - 1]
             if _l[4] != "":
                 _peaks[_i].root = _peaks[int(_l[4]) - 1]
     elif ver == 2:
         index_list = []
         for _id, _l in enumerate(_ls):
-            index_list.append(_l[0])
+            index_list.append(int(_l[0]))
             _pk = Peak()
-            _pk.val = float(_l[1])
+            if "--" in _l[1] or _l[1].lower() in ["none", "nan", ""]:
+                _pk.val = None
+            else:
+                _pk.val = float(_l[1])
             _pk.name = _l[2]
             _pk.numbers = [int(i) for i in _l[3].split()]
             _pk.is_sp3 = not bool(_l[6])
             _pk.nuclei = _l[7]
             _peaks.append(_pk)
         for _id, _l in enumerate(_ls):
             if _l[4] != "":
-                _peaks[_id].dtopic = _peaks(index_list.index(int(_l[4])))
+                _peaks[_id].dtopic = _peaks[index_list.index(int(_l[4]))]
             if _l[5] != "":
-                _peaks[_id].root = _peaks(index_list.index(int(_l[5])))
+                _peaks[_id].root = _peaks[index_list.index(int(_l[5]))]
     return _peaks
 
 
-def get_tensor(mol: Mol, key: str = "isotropic") -> Peaks:
+def get_tensor(mol: System, key: str = "isotropic") -> Peaks:
     _peaks = Peaks(mol.name)
     for _a in mol.atoms:
         _p = Peak()
         _p.val = _a.data[key]
         _p.numbers = [_a.number]
         _p.nuclei = _a.symbol
         _peaks.append(_p)
@@ -334,16 +337,16 @@
         logger.info(
             f"{swapped.label}: {a_peak.name} and {a_peak.dtopic.name} are swaped"
             + f" according to {a_peak.root.name} and {a_peak.dtopic.root.name}"
         )
     return swapped
 
 
-def export_peak(peaks: Peaks, filepath: Union[str, Path] = None) -> Path:
-    keys = ["Shift", "Name", "Nuclei", "Number", "sp2"]
+def export_peaks(peaks: Peaks, filepath: Union[str, Path] = None) -> Path:
+    keys = ["Value", "Name", "Number", "Nuclei", "sp3"]
     vals_dicts = []
     for _p in peaks:
         dicts = {
             "Shift": _p.val,
             "Name": _p.name,
             "Nuclei": _p.nuclei,
             "Number": _p.numbers,
@@ -378,25 +381,25 @@
         _err = assigned[idx].val - expt[idx].val
         n_probs *= stats.norm.sf(abs(_err - mean) / stdev)
     logger.info(f"Survival function of normal distribution was calculated: {n_probs}")
     return float(n_probs)
 
 
 class NmrBox(ToolBox):
-    def __init__(self, value: Union[Box, Mols]):
+    def __init__(self, contents: Union[Box, Systems, Iterable[System], System]):
         self.expt: Peaks = None
         self.ref: dict[str, float] = None
         self.tensor: list[Peaks] = []
         self._shift: list[Peaks] = []
         self._assigned: list[Peaks] = []
         self._shift_for_analysis: list[Peaks] = []
         self._assigned_for_analysis: list[Peaks] = []
         self.data = Data(self)
         self.analyzing = False
-        super().__init__(value)
+        super().__init__(contents)
 
     @property
     def shift(self) -> list[Peaks]:
         if self.analyzing:
             return self._shift_for_analysis
         return self._shift
 
@@ -435,15 +438,15 @@
         return self
 
     def load_expt(self, experiment_file: Union[str, Path], ver: int = 2):
         self.expt = get_expt(experiment_csv_file=experiment_file, ver=ver)
         return self
 
     def load_tensor(self, tensor_key="isotropic"):
-        for _c in self.mols:
+        for _c in self.get():
             self.tensor.append(get_tensor(_c, key=tensor_key))
         return self
 
     def load_ref(self, reference: Union[str, Path, dict]):
         if isinstance(reference, (str, Path)):
             refs: dict[str, float] = {}
             with Path(reference).open() as f:
@@ -743,7 +746,24 @@
                 ]
             self.data[f"{key}_{nuc}"] = {
                 _l: 100.0 * _val / sum(t_probs[nuc]) for _l, _val in zip(labels, t_probs[nuc])
             }
         t_probs["All"] = [t_probs["C"][idx] * t_probs["H"][idx] * t_probs["N"][idx] for idx in range(len(labels))]
         self.data[f"{key}_All"] = {_l: 100.0 * _val / sum(t_probs["All"]) for _l, _val in zip(labels, t_probs["All"])}
         return self.stop_analysis()
+
+    def export_assigned(self, filepath: Path = None):
+        self.check_assign()
+        keys = ["name", "number", "nuclei", "expt"]
+        rows = [[_p.name, " ".join([str(_n) for _n in _p.numbers]), _p.nuclei, _p.val] for _p in self.expt]
+        for _ps in self.assigned:
+            keys.append(_ps.label)
+            for idx, _r in enumerate(rows):
+                _r.append(_ps[idx].val)
+        if filepath is None:
+            filepath = Path.cwd().joinpath(self.expt.label)
+        elif filepath.is_dir():
+            filepath = filepath.joinpath(self.expt.label)
+        _p = Path(filepath).with_suffix(".csv")
+        with _p.open("w", newline="") as f:
+            csv.writer(f).writerows([keys] + rows)
+        return self
```

## acceltools/plot.py

```diff
@@ -1,184 +1,184 @@
-import copy
-from pathlib import Path
-from typing import Iterable, Union
-
-import matplotlib.pyplot as plt
-from accel.base.box import Box
-from accel.base.mols import Mol, Mols
-from accel.util.log import logger
-from matplotlib.axes import Axes
-
-from acceltools.base import ToolBox
-
-
-def _marker_generator(maker: str = None):
-    if maker is not None:
-        while True:
-            yield maker
-    else:
-        markers = ["o", ",", "v", "^", "<", ">", "8", "p", "*", "h", "H", "D", "d"]
-        i = 0
-        while True:
-            i += 1
-            if i > len(markers):
-                i = 1
-            yield markers[i - 1]
-
-
-class PlotBox(ToolBox):
-    def __init__(self, box: Union[Box, Mols, Iterable[Mol], Mol]):
-        self.path: Path = None
-        super().__init__(box)
-
-    def diagram(
-        self,
-        filepath: Path,
-        diagram_roles: list[str] = ["reactant", "ts", "product"],
-        zero_role_index: int = 0,
-        role_key: str = "diagram_role",
-        connection_key: str = "diagram_connection",
-        non_mimimum: bool = True,
-    ):
-
-        _ze = min(_c.energy for _c in self.mols.has_data(role_key, diagram_roles[zero_role_index]))
-
-        fig = plt.figure(figsize=((2 * len(diagram_roles)) + 0.4, 4.8))
-        ax: Axes = fig.add_subplot(1, 1, 1)
-        ax.set_xlim(0, (len(diagram_roles) + 1) * 2)
-        ax.set_xticks([])
-        x_values = {_key: [(i * 2) + 1, (i * 2) + 2] for i, _key in enumerate(diagram_roles)}
-        ploted_conf: list[Mol] = []
-        non_mimimum_conf: list[list[Mol]] = []
-        for _role in diagram_roles:
-            for _confs in Box(self.mols.has_data(role_key, _role)).mols.labels.values():
-                _confs_orderd = sorted(_confs, key=lambda t: t.energy)
-                ploted_conf.append(_confs_orderd[0])
-                non_mimimum_conf.append(_confs_orderd[1:])
-
-        for _c, _non_min_cs in zip(ploted_conf, non_mimimum_conf):
-            _key = _c.data[role_key]
-            _energy = _c.energy - _ze
-            _connect: list[list[str]] = copy.deepcopy(_c.data.get(connection_key))
-            _role_idx = diagram_roles.index(_key)
-            if _connect is not None and len(_connect) == 2:
-                for _idx in range(len(_connect)):
-                    if isinstance(_connect[_idx], str):
-                        _connect[_idx] = [_connect[_idx]]
-                for _tc in ploted_conf:
-                    if _role_idx == 0:
-                        pass
-                    elif _tc.data[role_key] == diagram_roles[_role_idx - 1] and _tc.label in _connect[0]:
-                        ax.plot(
-                            [x_values[_key][0] - 1, x_values[_key][0]],
-                            [_tc.energy - _ze, _energy],
-                            color="black",
-                            linewidth=0.1,
-                            linestyle="--",
-                        )
-                    if _role_idx == len(diagram_roles) - 1:
-                        pass
-                    elif _tc.data[role_key] == diagram_roles[_role_idx + 1] and _tc.label in _connect[1]:
-                        ax.plot(
-                            [x_values[_key][1], x_values[_key][1] + 1],
-                            [_energy, _tc.energy - _ze],
-                            color="black",
-                            linewidth=0.1,
-                            linestyle="--",
-                        )
-            ax.plot(
-                x_values[_key],
-                [_energy, _energy],
-                color="black",
-                linewidth=1.5,
-                linestyle="-",
-                label=_c.path.stem,
-            )
-            ax.text(x_values[_key][1] + 0.1, _energy, _c.name, fontsize=7, va="center")
-            ax.text(
-                x_values[_key][0] - 0.1,
-                _energy,
-                f"{_energy:.1f}",
-                fontsize=7,
-                va="center",
-                ha="right",
-            )
-            if non_mimimum:
-                for _non_min in _non_min_cs:
-                    _energy = _non_min.energy - _ze
-                    ax.plot(
-                        x_values[_key],
-                        [_energy, _energy],
-                        color="black",
-                        linewidth=0.1,
-                        linestyle="-",
-                    )
-
-        _png = Path(filepath).with_suffix(".png")
-        plt.savefig(_png, transparent=False, dpi=300)
-        plt.close()
-        logger.info(f"{str(_png)} was ploted")
-        self.path = _png
-        return self
-
-    def scatter(
-        self,
-        filepath: Path,
-        x_key: str = None,
-        y_key: str = None,
-        size=10,
-        marker=None,
-        color=True,
-        size_by_energy=False,
-        color_by_energy=False,
-    ):
-        fig = plt.figure()
-        ax: Axes = fig.add_subplot(1, 1, 1)
-        ax.tick_params(direction="in")
-        maker = _marker_generator(marker)
-        _legend = []
-        for label, _confs in self.mols.labels.items():
-            _x = [_c.energy for _c in _confs]
-            ax.set_xlabel("Energy")
-            _y = [_c.energy for _c in _confs]
-            ax.set_ylabel("Energy")
-            if x_key is not None:
-                _x = [_c.data.get(x_key) for _c in _confs]
-                ax.set_xlabel(x_key)
-            if y_key is not None:
-                _y = [_c.data.get(y_key) for _c in _confs]
-                ax.set_ylabel(y_key)
-            if size_by_energy:
-                energies = [_c.energy for _c in _confs]
-                energy_min = min(energies)
-                energy_max = max(energies) - energy_min
-                energies = [1 - ((_e - energy_min) / energy_max) for _e in energies]
-                energies = [(_e * 2) ** 6 for _e in energies]
-                size_used = [float(size) * _e for _e in energies]
-            else:
-                size_used = size
-            if color_by_energy:
-                energies = [_c.energy for _c in _confs]
-                if size_by_energy:
-                    ax.scatter(_x, _y, s=size_used, marker=next(maker), c=energies, alpha=0.5, edgecolors="gray")
-                else:
-                    ax.scatter(_x, _y, s=size_used, marker=next(maker), c=energies, edgecolors="gray")
-            elif color:
-                if size_by_energy:
-                    ax.scatter(_x, _y, s=size_used, marker=next(maker), alpha=0.5, edgecolors="gray")
-                else:
-                    ax.scatter(_x, _y, s=size_used, marker=next(maker))
-            else:
-                ax.scatter(_x, _y, s=size_used, marker=next(maker), c="white", edgecolors="black", linewidths=0.5)
-            _legend.append(label)
-        if len(_legend) != 1:
-            ax.legend(_legend)
-        _png = Path(filepath).with_suffix(".png")
-        ax.set_title(_png.stem)
-        plt.savefig(_png, transparent=False, dpi=300)
-        plt.close()
-        logger.info(f"{str(_png)} was ploted")
-        self.path = _png
-        return self
-
-    def line(self):
-        return self
+import copy
+from pathlib import Path
+from typing import Iterable, Union
+
+import matplotlib.pyplot as plt
+from accel.base.box import Box
+from accel.base.systems import System, Systems
+from accel.util.log import logger
+from matplotlib.axes import Axes
+
+from acceltools.base import ToolBox
+
+
+def _marker_generator(maker: str = None):
+    if maker is not None:
+        while True:
+            yield maker
+    else:
+        markers = ["o", ",", "v", "^", "<", ">", "8", "p", "*", "h", "H", "D", "d"]
+        i = 0
+        while True:
+            i += 1
+            if i > len(markers):
+                i = 1
+            yield markers[i - 1]
+
+
+class PlotBox(ToolBox):
+    def __init__(self, contents: Union[Box, Systems, Iterable[System], System]):
+        self.path: Path = None
+        super().__init__(contents)
+
+    def diagram(
+        self,
+        filepath: Path,
+        diagram_roles: list[str] = ["reactant", "ts", "product"],
+        zero_role_index: int = 0,
+        role_key: str = "diagram_role",
+        connection_key: str = "diagram_connection",
+        non_mimimum: bool = True,
+    ):
+
+        _ze = min(_c.energy for _c in self.get().has_data(role_key, diagram_roles[zero_role_index]))
+
+        fig = plt.figure(figsize=((2 * len(diagram_roles)) + 0.4, 4.8))
+        ax: Axes = fig.add_subplot(1, 1, 1)
+        ax.set_xlim(0, (len(diagram_roles) + 1) * 2)
+        ax.set_xticks([])
+        x_values = {_key: [(i * 2) + 1, (i * 2) + 2] for i, _key in enumerate(diagram_roles)}
+        ploted_conf: list[System] = []
+        non_mimimum_conf: list[list[System]] = []
+        for _role in diagram_roles:
+            for _confs in Box(self.get().has_data(role_key, _role)).get().labels.values():
+                _confs_orderd = sorted(_confs, key=lambda t: t.energy)
+                ploted_conf.append(_confs_orderd[0])
+                non_mimimum_conf.append(_confs_orderd[1:])
+
+        for _c, _non_min_cs in zip(ploted_conf, non_mimimum_conf):
+            _key = _c.data[role_key]
+            _energy = _c.energy - _ze
+            _connect: list[list[str]] = copy.deepcopy(_c.data.get(connection_key))
+            _role_idx = diagram_roles.index(_key)
+            if _connect is not None and len(_connect) == 2:
+                for _idx in range(len(_connect)):
+                    if isinstance(_connect[_idx], str):
+                        _connect[_idx] = [_connect[_idx]]
+                for _tc in ploted_conf:
+                    if _role_idx == 0:
+                        pass
+                    elif _tc.data[role_key] == diagram_roles[_role_idx - 1] and _tc.label in _connect[0]:
+                        ax.plot(
+                            [x_values[_key][0] - 1, x_values[_key][0]],
+                            [_tc.energy - _ze, _energy],
+                            color="black",
+                            linewidth=0.1,
+                            linestyle="--",
+                        )
+                    if _role_idx == len(diagram_roles) - 1:
+                        pass
+                    elif _tc.data[role_key] == diagram_roles[_role_idx + 1] and _tc.label in _connect[1]:
+                        ax.plot(
+                            [x_values[_key][1], x_values[_key][1] + 1],
+                            [_energy, _tc.energy - _ze],
+                            color="black",
+                            linewidth=0.1,
+                            linestyle="--",
+                        )
+            ax.plot(
+                x_values[_key],
+                [_energy, _energy],
+                color="black",
+                linewidth=1.5,
+                linestyle="-",
+                label=_c.path.stem,
+            )
+            ax.text(x_values[_key][1] + 0.1, _energy, _c.name, fontsize=7, va="center")
+            ax.text(
+                x_values[_key][0] - 0.1,
+                _energy,
+                f"{_energy:.1f}",
+                fontsize=7,
+                va="center",
+                ha="right",
+            )
+            if non_mimimum:
+                for _non_min in _non_min_cs:
+                    _energy = _non_min.energy - _ze
+                    ax.plot(
+                        x_values[_key],
+                        [_energy, _energy],
+                        color="black",
+                        linewidth=0.1,
+                        linestyle="-",
+                    )
+
+        _png = Path(filepath).with_suffix(".png")
+        plt.savefig(_png, transparent=False, dpi=300)
+        plt.close()
+        logger.info(f"{str(_png)} was ploted")
+        self.path = _png
+        return self
+
+    def scatter(
+        self,
+        filepath: Path,
+        x_key: str = None,
+        y_key: str = None,
+        size=10,
+        marker=None,
+        color=True,
+        size_by_energy=False,
+        color_by_energy=False,
+    ):
+        fig = plt.figure()
+        ax: Axes = fig.add_subplot(1, 1, 1)
+        ax.tick_params(direction="in")
+        maker = _marker_generator(marker)
+        _legend = []
+        for label, _confs in self.get().labels.items():
+            _x = [_c.energy for _c in _confs]
+            ax.set_xlabel("Energy")
+            _y = [_c.energy for _c in _confs]
+            ax.set_ylabel("Energy")
+            if x_key is not None:
+                _x = [_c.data.get(x_key) for _c in _confs]
+                ax.set_xlabel(x_key)
+            if y_key is not None:
+                _y = [_c.data.get(y_key) for _c in _confs]
+                ax.set_ylabel(y_key)
+            if size_by_energy:
+                energies = [_c.energy for _c in _confs]
+                energy_min = min(energies)
+                energy_max = max(energies) - energy_min
+                energies = [1 - ((_e - energy_min) / energy_max) for _e in energies]
+                energies = [(_e * 2) ** 6 for _e in energies]
+                size_used = [float(size) * _e for _e in energies]
+            else:
+                size_used = size
+            if color_by_energy:
+                energies = [_c.energy for _c in _confs]
+                if size_by_energy:
+                    ax.scatter(_x, _y, s=size_used, marker=next(maker), c=energies, alpha=0.5, edgecolors="gray")
+                else:
+                    ax.scatter(_x, _y, s=size_used, marker=next(maker), c=energies, edgecolors="gray")
+            elif color:
+                if size_by_energy:
+                    ax.scatter(_x, _y, s=size_used, marker=next(maker), alpha=0.5, edgecolors="gray")
+                else:
+                    ax.scatter(_x, _y, s=size_used, marker=next(maker))
+            else:
+                ax.scatter(_x, _y, s=size_used, marker=next(maker), c="white", edgecolors="black", linewidths=0.5)
+            _legend.append(label)
+        if len(_legend) != 1:
+            ax.legend(_legend)
+        _png = Path(filepath).with_suffix(".png")
+        ax.set_title(_png.stem)
+        plt.savefig(_png, transparent=False, dpi=300)
+        plt.close()
+        logger.info(f"{str(_png)} was ploted")
+        self.path = _png
+        return self
+
+    def line(self):
+        return self
```

## acceltools/series.py

```diff
@@ -1,152 +1,180 @@
-import math
-from typing import Iterable, Sequence, Set, Tuple, Union
-
-from accel import Mol
-from accel.base.atoms import Atoms
-from accel.base.box import Box
-from accel.base.mols import Mols
-from accel.base.xyz import get_dihedral
-
-from acceltools.base import ToolBox
-
-
-def _get_angle_set(bonds: Set[Tuple[int]]) -> Set[Tuple[int]]:
-    ang_set = set()
-    for _b in bonds:
-        for _al in [(_b[0], _b[1]), (_b[1], _b[0])]:
-            for _pair_bond in [_pair_b for _pair_b in bonds if _al[0] in _pair_b and _b != _pair_b]:
-                if _al[0] == _pair_bond[0]:
-                    another_atom = _pair_bond[1]
-                else:
-                    another_atom = _pair_bond[0]
-                if another_atom < _al[1]:
-                    ang_set.add((another_atom, _al[0], _al[1]))
-                elif another_atom > _al[1]:
-                    ang_set.add((_al[1], _al[0], another_atom))
-                else:
-                    pass
-    return ang_set
-
-
-def _get_dihedral_set(bonds: Set[Tuple[int]]) -> Set[Tuple[int]]:
-    dihed_set = set()
-    for ang in _get_angle_set(bonds):
-        for _al in [(ang[0], ang[1], ang[2]), (ang[2], ang[1], ang[0])]:
-            for _pair_bond in [_pair_b for _pair_b in bonds if _al[0] in _pair_b and _al[1] not in _pair_b]:
-                if _al[0] == _pair_bond[0]:
-                    another_atom = _pair_bond[1]
-                else:
-                    another_atom = _pair_bond[0]
-                if _al[0] < _al[1]:
-                    dihed_set.add((another_atom, _al[0], _al[1], _al[2]))
-                elif _al[0] > _al[1]:
-                    dihed_set.add((_al[2], _al[1], _al[0], another_atom))
-                else:
-                    pass
-    return dihed_set
-
-
-def _remove_hydrogen(bonds: Set[Tuple[int]], atoms: Atoms) -> Set[Tuple[int]]:
-    non_h_set = set()
-    for _b in bonds:
-        if "H" not in [atoms.get(_b[0]).symbol, atoms.get(_b[1]).symbol]:
-            non_h_set.add(_b)
-    return non_h_set
-
-
-class SeriesBox(ToolBox):
-    def __init__(self, box: Union[Box, Mols, Iterable[Mol], Mol]):
-        self.keys: list[str] = None
-        super().__init__(box)
-
-    def modify_length(
-        self,
-        number_a: int,
-        number_b: int,
-        begin: float,
-        end: float,
-        step: float = 0.1,
-        fix_a: bool = False,
-        fix_b: bool = False,
-        numbers_along_with_a: Sequence[int] = [],
-        numbers_along_with_b: Sequence[int] = [],
-    ):
-        ret_list = []
-        target = begin
-        count = 0
-        while target < end:
-            mc = Box().bind(self.mols).duplicate()
-            mc.modify_length(number_a, number_b, target, fix_a, fix_b, numbers_along_with_a, numbers_along_with_b)
-            for _c in mc.mols:
-                _c.name = f"{_c.name}_{count:03d}"
-            ret_list.extend(mc.mols.to_list())
-            target += step
-            count += 1
-        return Mols().bind(ret_list)
-
-    def calc_length(self, all=False, key: str = "L_", in_label=True, ignore_hydrogen=True):
-        key_list = []
-        for confs in self.mols.labels.values():
-            label_mc = Box(confs)
-            _atoms = label_mc.mols.get().atoms
-            _bonds = _atoms.bonds.keys()
-            if ignore_hydrogen:
-                _bonds = _remove_hydrogen(_bonds, _atoms)
-            for bond in _bonds:
-                tkey = f"{key}{_atoms.get(bond[0])}-{_atoms.get(bond[1])}"
-                label_mc.calc_length(bond[0], bond[1], tkey)
-                key_list.append(tkey)
-        self.keys = key_list
-        return self
-
-    def calc_angle(self, all=False, key: str = "A_", in_label=True, ignore_hydrogen=True):
-        key_list = []
-        for confs in self.mols.labels.values():
-            label_mc = Box(confs)
-            _atoms = label_mc.mols.get().atoms
-            _bonds = _atoms.bonds.keys()
-            if ignore_hydrogen:
-                _bonds = _remove_hydrogen(_bonds, _atoms)
-            for angles in _get_angle_set(_bonds):
-                tkey = f"{key}{_atoms.get(angles[0])}-{_atoms.get(angles[1])}-{_atoms.get(angles[2])}"
-                label_mc.calc_angle(angles[0], angles[1], angles[2], tkey)
-                key_list.append(tkey)
-        self.keys = key_list
-        return self
-
-    def calc_dihedral(self, all=False, key: str = "D_", in_label=True, ignore_hydrogen=True):
-        key_list = []
-        for confs in self.mols.labels.values():
-            label_mc = Box(confs)
-            _atoms = label_mc.mols.get().atoms
-            _bonds = _atoms.bonds.keys()
-            if ignore_hydrogen:
-                _bonds = _remove_hydrogen(_bonds, _atoms)
-            for dhs in _get_dihedral_set(_bonds):
-                tkey = f"{key}{_atoms.get(dhs[0])}-{_atoms.get(dhs[1])}-{_atoms.get(dhs[2])}-{_atoms.get(dhs[3])}"
-                label_mc.calc_dihedral(dhs[0], dhs[1], dhs[2], dhs[3], tkey)
-                key_list.append(tkey)
-        self.keys = key_list
-        return self
-
-    def calc_dihedral_xy(self, all=False, key: str = "D_", in_label=True, ignore_hydrogen=True):
-        key_list = []
-        for confs in self.mols.labels.values():
-            label_mc = Box(confs)
-            _atoms = label_mc.mols.get().atoms
-            _bonds = _atoms.bonds.keys()
-            if ignore_hydrogen:
-                _bonds = _remove_hydrogen(_bonds, _atoms)
-            for dhs in _get_dihedral_set(_bonds):
-                xkey = f"X{key}{_atoms.get(dhs[0])}-{_atoms.get(dhs[1])}-{_atoms.get(dhs[2])}-{_atoms.get(dhs[3])}"
-                ykey = f"Y{key}{_atoms.get(dhs[0])}-{_atoms.get(dhs[1])}-{_atoms.get(dhs[2])}-{_atoms.get(dhs[3])}"
-                for _c in label_mc.mols:
-                    d_degree = get_dihedral(
-                        _c.atoms.get(dhs[0]), _c.atoms.get(dhs[1]), _c.atoms.get(dhs[2]), _c.atoms.get(dhs[3])
-                    )
-                    _c.data[xkey] = math.cos(math.radians(d_degree))
-                    _c.data[ykey] = math.sin(math.radians(d_degree))
-                key_list.append(xkey)
-                key_list.append(ykey)
-        self.keys = key_list
-        return self
+import math
+from pathlib import Path
+from statistics import mean
+from typing import Iterable, Sequence, Set, Tuple, Union
+
+from accel.base.atoms import Atoms
+from accel.base.box import Box
+from accel.base.systems import System, Systems
+from accel.base.tools import change_dir, float_to_str
+from accel.util.log import logger
+
+from acceltools.base import ToolBox
+
+
+def _get_angle_set(bonds: Set[Tuple[int]]) -> Set[Tuple[int]]:
+    ang_set = set()
+    for _b in bonds:
+        for _al in [(_b[0], _b[1]), (_b[1], _b[0])]:
+            for _pair_bond in [_pair_b for _pair_b in bonds if _al[0] in _pair_b and _b != _pair_b]:
+                if _al[0] == _pair_bond[0]:
+                    another_atom = _pair_bond[1]
+                else:
+                    another_atom = _pair_bond[0]
+                if another_atom < _al[1]:
+                    ang_set.add((another_atom, _al[0], _al[1]))
+                elif another_atom > _al[1]:
+                    ang_set.add((_al[1], _al[0], another_atom))
+                else:
+                    pass
+    return ang_set
+
+
+def _get_dihedral_set(bonds: Set[Tuple[int]]) -> Set[Tuple[int]]:
+    dihed_set = set()
+    for ang in _get_angle_set(bonds):
+        for _al in [(ang[0], ang[1], ang[2]), (ang[2], ang[1], ang[0])]:
+            for _pair_bond in [_pair_b for _pair_b in bonds if _al[0] in _pair_b and _al[1] not in _pair_b]:
+                if _al[0] == _pair_bond[0]:
+                    another_atom = _pair_bond[1]
+                else:
+                    another_atom = _pair_bond[0]
+                if _al[0] < _al[1]:
+                    dihed_set.add((another_atom, _al[0], _al[1], _al[2]))
+                elif _al[0] > _al[1]:
+                    dihed_set.add((_al[2], _al[1], _al[0], another_atom))
+                else:
+                    pass
+    return dihed_set
+
+
+def _remove_hydrogen(bonds: Set[Tuple[int]], atoms: Atoms) -> Set[Tuple[int]]:
+    non_h_set = set()
+    for _b in bonds:
+        if "H" not in [atoms.get(_b[0]).symbol, atoms.get(_b[1]).symbol]:
+            non_h_set.add(_b)
+    return non_h_set
+
+
+class SeriesBox(ToolBox):
+    def __init__(self, contents: Union[Box, Systems, Iterable[System], System]):
+        self.keys: list[str] = None
+        super().__init__(contents)
+
+    def modify_length(
+        self,
+        number_a: int,
+        number_b: int,
+        begin: float,
+        end: float,
+        step: float = 0.1,
+        fix_a: bool = False,
+        fix_b: bool = False,
+        numbers_along_with_a: Sequence[int] = [],
+        numbers_along_with_b: Sequence[int] = [],
+    ):
+        ret_list = []
+        target = begin
+        count = 0
+        while target < end:
+            mc = Box().bind(self.get()).duplicate()
+            mc.modify_length(number_a, number_b, target, fix_a, fix_b, numbers_along_with_a, numbers_along_with_b)
+            for c in mc.get():
+                c.name = f"{c.name}_{count:03d}"
+                ret_list.append(c)
+            target += step
+            count += 1
+        return Systems().bind(ret_list)
+
+    def calc_length(self, all=False, key: str = "L_", in_label=True, ignore_hydrogen=True):
+        key_list = []
+        for confs in self.get().labels.values():
+            box = Box(confs)
+            _atoms = confs.get().atoms
+            _bonds = _atoms.bonds.keys()
+            if ignore_hydrogen:
+                _bonds = _remove_hydrogen(_bonds, _atoms)
+            for bond in _bonds:
+                tkey = f"{key}{_atoms.get(bond[0])}-{_atoms.get(bond[1])}"
+                box.calc_length(bond[0], bond[1], tkey)
+                key_list.append(tkey)
+        self.keys = key_list
+        return self
+
+    def calc_angle(self, all=False, key: str = "A_", in_label=True, ignore_hydrogen=True):
+        key_list = []
+        for confs in self.get().labels.values():
+            box = Box(confs)
+            _atoms = confs.get().atoms
+            _bonds = _atoms.bonds.keys()
+            if ignore_hydrogen:
+                _bonds = _remove_hydrogen(_bonds, _atoms)
+            for angles in _get_angle_set(_bonds):
+                tkey = f"{key}{_atoms.get(angles[0])}-{_atoms.get(angles[1])}-{_atoms.get(angles[2])}"
+                box.calc_angle(angles[0], angles[1], angles[2], tkey)
+                key_list.append(tkey)
+        self.keys = key_list
+        return self
+
+    def calc_dihedral(self, all=False, key: str = "D_", in_label=True, ignore_hydrogen=True):
+        key_list = []
+        for confs in self.get().labels.values():
+            box = Box(confs)
+            _atoms = confs.get().atoms
+            _bonds = _atoms.bonds.keys()
+            if ignore_hydrogen:
+                _bonds = _remove_hydrogen(_bonds, _atoms)
+            for dhs in _get_dihedral_set(_bonds):
+                tkey = f"{key}{_atoms.get(dhs[0])}-{_atoms.get(dhs[1])}-{_atoms.get(dhs[2])}-{_atoms.get(dhs[3])}"
+                box.calc_dihedral(dhs[0], dhs[1], dhs[2], dhs[3], tkey)
+                key_list.append(tkey)
+        self.keys = key_list
+        return self
+
+    def calc_dihedral_xy(self, all=False, key: str = "D_", in_label=True, ignore_hydrogen=True):
+        key_list = []
+        for confs in self.get().labels.values():
+            _atoms = confs.get().atoms
+            _bonds = _atoms.bonds.keys()
+            if ignore_hydrogen:
+                _bonds = _remove_hydrogen(_bonds, _atoms)
+            for dhs in _get_dihedral_set(_bonds):
+                xkey = f"X{key}{_atoms.get(dhs[0])}-{_atoms.get(dhs[1])}-{_atoms.get(dhs[2])}-{_atoms.get(dhs[3])}"
+                ykey = f"Y{key}{_atoms.get(dhs[0])}-{_atoms.get(dhs[1])}-{_atoms.get(dhs[2])}-{_atoms.get(dhs[3])}"
+                for c in confs:
+                    d_degree = c.atoms.get_dihedral(dhs[0], dhs[1], dhs[2], dhs[3])
+                    c.data[xkey] = math.cos(math.radians(d_degree))
+                    c.data[ykey] = math.sin(math.radians(d_degree))
+                key_list.append(xkey)
+                key_list.append(ykey)
+        self.keys = key_list
+        return self
+
+    def write_trjxyz(self, output_dir: Path = None, order_key: str = None, centering: bool = True):
+        for label, cs in self.get().labels.items():
+            csls = cs.to_list()
+            if order_key is not None:
+                csls = [c for c in csls if c.data.get(order_key) is not None]
+                csls = sorted(csls, key=lambda c: c.data[order_key])
+            ls = []
+            for c in csls:
+                ls.append(f"{len(c.atoms)}\n")
+                ls.append(f"{c.name}\n")
+                if centering:
+                    centering_vec = [mean([a.xyz[i] for a in c.atoms]) for i in range(3)]
+                    try:
+                        prec = max(max(len(float_to_str(a.xyz[i]).split(".")[1]) for a in c.atoms) for i in range(3))
+                    except IndexError:
+                        logger.error(f"could not resolve the precision in converting to xyz file of {c.name}")
+                        prec = 10
+                    centering_vec = [round(val, prec) for val in centering_vec]
+                for a in c.atoms:
+                    xyz = [a.x, a.y, a.z]
+                    if centering:
+                        xyz = [float_to_str(round(val - centering_vec[i], prec)) for i, val in enumerate(xyz)]
+                    xyz = [float_to_str(val) for val in xyz]
+                    ls.append(f"{a.symbol:<2} {xyz[0]:>15} {xyz[1]:>15} {xyz[2]:>15}\n")
+            with change_dir(cs.get().path, output_dir, label).with_suffix(".xyz").open("w") as f:
+                f.writelines(ls)
+            logger.debug(f"{label}.xyz was exported")
+        return self
```

## acceltools/table.py

```diff
@@ -1,35 +1,35 @@
-from typing import List
-
-import pandas as pd
-from accel.util.log import logger
-
-from acceltools.base import ToolBox
-
-
-class TableBox(ToolBox):
-    def get_df(self, data_list: List[str] = []):
-        df = pd.DataFrame()
-        for _c in self.mols:
-            ser_dict = {}
-            for key in data_list:
-                if key in [
-                    "path",
-                    "name",
-                    "filetype",
-                    "label",
-                    "flag",
-                    "history",
-                    "energy",
-                    "atoms",
-                    "data",
-                    "cache",
-                    "total_charge",
-                    "multiplicity",
-                ]:
-                    ser_dict[key] = getattr(_c, key)
-                else:
-                    ser_dict[key] = _c.data.get(key)
-            _ser = pd.Series(ser_dict, name=_c.name)
-            df = pd.concat([df, pd.DataFrame([_ser])])
-            logger.info(f"data of {_c.name} was added to dataframe")
-        return df
+from typing import List
+
+import pandas as pd
+from accel.util.log import logger
+
+from acceltools.base import ToolBox
+
+
+class TableBox(ToolBox):
+    def get_df(self, data_list: List[str] = []):
+        df = pd.DataFrame()
+        for c in self.get():
+            ser_dict = {}
+            for key in data_list:
+                if key in [
+                    "path",
+                    "name",
+                    "filetype",
+                    "label",
+                    "flag",
+                    "history",
+                    "energy",
+                    "atoms",
+                    "data",
+                    "cache",
+                    "total_charge",
+                    "multiplicity",
+                ]:
+                    ser_dict[key] = getattr(c, key)
+                else:
+                    ser_dict[key] = c.data.get(key)
+            _ser = pd.Series(ser_dict, name=c.name)
+            df = pd.concat([df, pd.DataFrame([_ser])])
+            logger.info(f"data of {c.name} was added to dataframe")
+        return df
```

## Comparing `acceltools-0.0.9.dist-info/LICENSE` & `acceltools-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `acceltools-0.0.9.dist-info/METADATA` & `acceltools-0.1.1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: acceltools
-Version: 0.0.9
+Version: 0.1.1
 Summary: tools for ACCeL
 Home-page: https://github.com/kfchem/acceltools
 Author: Keisuke Fukaya
 Author-email: kfukaya@pu-toyama.ac.jp
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: accel (>=0.0.13)
+Requires-Dist: accel (>=0.1.0)
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: python-docx
 
 UNKNOWN
```

