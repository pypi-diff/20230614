# Comparing `tmp/tagreader-4.0.3.tar.gz` & `tmp/tagreader-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagreader-4.0.3.tar", max compression
+gzip compressed data, was "tagreader-4.1.1.tar", max compression
```

## Comparing `tagreader-4.0.3.tar` & `tagreader-4.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.0.3/LICENSE
--rw-r--r--   0        0        0     2982 2023-06-09 06:31:44.774759 tagreader-4.0.3/README.md
--rw-r--r--   0        0        0     1565 2023-06-09 06:49:48.996497 tagreader-4.0.3/pyproject.toml
--rw-r--r--   0        0        0      329 2023-06-09 06:24:33.101565 tagreader-4.0.3/tagreader/__init__.py
--rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.0.3/tagreader/__version__.py
--rw-r--r--   0        0        0    17751 2023-06-09 06:24:33.103078 tagreader-4.0.3/tagreader/cache.py
--rw-r--r--   0        0        0    21162 2023-06-09 06:24:33.103962 tagreader-4.0.3/tagreader/clients.py
--rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.0.3/tagreader/logger.py
--rw-r--r--   0        0        0    25064 2023-06-09 06:24:33.105099 tagreader-4.0.3/tagreader/odbc_handlers.py
--rw-r--r--   0        0        0     7755 2023-06-09 06:24:33.105868 tagreader-4.0.3/tagreader/utils.py
--rw-r--r--   0        0        0    33019 2023-06-09 06:24:33.106754 tagreader-4.0.3/tagreader/web_handlers.py
--rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 tagreader-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.1.1/LICENSE
+-rw-r--r--   0        0        0     2779 2023-06-14 10:40:53.495633 tagreader-4.1.1/README.md
+-rw-r--r--   0        0        0     1633 2023-06-14 13:27:23.957086 tagreader-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0      351 2023-06-14 10:40:53.499388 tagreader-4.1.1/tagreader/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.1.1/tagreader/__version__.py
+-rw-r--r--   0        0        0    12723 2023-06-14 10:40:53.499996 tagreader-4.1.1/tagreader/cache.py
+-rw-r--r--   0        0        0    22839 2023-06-14 13:05:07.540054 tagreader-4.1.1/tagreader/clients.py
+-rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.1.1/tagreader/logger.py
+-rw-r--r--   0        0        0    25164 2023-06-14 13:05:07.540885 tagreader-4.1.1/tagreader/odbc_handlers.py
+-rw-r--r--   0        0        0     8215 2023-06-14 13:05:07.541522 tagreader-4.1.1/tagreader/utils.py
+-rw-r--r--   0        0        0    32868 2023-06-14 10:54:03.255470 tagreader-4.1.1/tagreader/web_handlers.py
+-rw-r--r--   0        0        0     4622 1970-01-01 00:00:00.000000 tagreader-4.1.1/PKG-INFO
```

### Comparing `tagreader-4.0.3/LICENSE` & `tagreader-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tagreader-4.0.3/README.md` & `tagreader-4.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,24 +21,20 @@
 to cache results.
 
 ## Requirements
 
 Python >=3.8 with the following packages:
 
   + pandas >= 1.0.0
-  + tables (*)
   + requests
   + requests-kerberos
   + certifi >= 2023.5.7
+  + diskcache
   + pyodbc (**)
 
-*) If tables is not installed, caching of fetched data will be disabled.
-Tables will be installed alongside Tagreader unless the installation is
-known to fail, which is the case for Macs with ARM CPU.
-
 **) If using ODBC connections, you must also install proprietary drivers for
 PI ODBC and/or Aspen IP.21 SQLPlus. These drivers are only available for
 Microsoft Windows. Pyodbc will therefore not be installed for non-Windows
 systems.
 
 ## Installation
```

### Comparing `tagreader-4.0.3/pyproject.toml` & `tagreader-4.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "tagreader"
-version = "4.0.3"
+version = "4.1.1"
 description = "Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems."
 authors = ["Einar S. Idsø <eiids@equinor.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tagreader"}]
 keywords=["Aspen InfoPlus.21", "OSIsoft PI"]
+homepage = "https://github.com/equinor/tagreader-python"
+repository = "https://github.com/equinor/tagreader-python"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: MacOS",
@@ -28,17 +30,17 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = ">=1"
 pyodbc = "^4"
 certifi = "^2023"
 requests = "^2"
 requests-kerberos = "^0"
-tables = { version = "^3", markers = "platform_machine != 'arm64'" }
 jupyter = { version = "^1", optional = true }
 matplotlib = { version = "^3", optional = true }
+diskcache = "^5.6.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3"
 pytest = "^7"
 
 [tool.poetry.extras]
```

### Comparing `tagreader-4.0.3/tagreader/cache.py` & `tagreader-4.1.1/tagreader/cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,222 +1,251 @@
-import os
-import warnings
-from importlib.util import find_spec
-from typing import Dict, List, Literal, Optional, Tuple, Union, cast
+from datetime import datetime, timedelta
+from pathlib import Path
+from typing import Dict, List, Optional, Tuple, Union, cast
 
 import pandas as pd
+import pytz
+from diskcache import Cache
 
+from tagreader.logger import logger
 from tagreader.utils import ReaderType
 
 
 def safe_tagname(tagname: str) -> str:
     tagname = tagname.replace(".", "_")
     tagname = "".join(c for c in tagname if c.isalnum() or c == "_").strip()
     if tagname[0].isnumeric():
         tagname = "_" + tagname  # Conform to NaturalName
     return tagname
 
 
-def timestamp_to_epoch(timestamp: pd.Timestamp) -> int:
-    origin = pd.Timestamp("1970-01-01")
+def timestamp_to_epoch(timestamp: datetime) -> int:
+    origin = datetime(1970, 1, 1)
     if timestamp.tzinfo is not None:
-        timestamp = timestamp.tz_convert("UTC").tz_localize(None)
-    return (timestamp - origin) // pd.Timedelta("1s")
+        timestamp = timestamp.astimezone(pytz.utc).replace(tzinfo=None)
+    return (timestamp - origin) // timedelta(seconds=1)
 
 
-class BucketCache:
-    def __init__(self, filename: str, path: str = ".") -> None:
-        if not find_spec("tables"):
-            warnings.warn("Package 'tables' not installed. Disabling cache.")
+def _infer_pandas_index_freq(df: pd.DataFrame) -> pd.DataFrame:
+    try:
+        if pd.infer_freq(df.index):  # type: ignore[arg-type]
+            df = df.asfreq(pd.infer_freq(df.index))  # type: ignore[arg-type]
+    except (TypeError, ValueError) as e:
+        logger.warning(f"Could not infer frequency of timeseries in Cache. {e}")
+    return df
+
+
+def _drop_duplicates_and_sort_index(df: pd.DataFrame) -> pd.DataFrame:
+    return df[~df.index.duplicated(keep="first")].sort_index()
+
+
+def clean_dataframe(df: pd.DataFrame) -> pd.DataFrame:
+    return _infer_pandas_index_freq(_drop_duplicates_and_sort_index(df))
+
+
+class BaseCache(Cache):  # type: ignore[misc]
+    """
+    Cache works as a Python dictionary with persistence. It is simple to use, and only requires a directory for
+    the cache. The default directory is <current path>/.cache/
+    """
+
+    def __init__(
+        self,
+        directory: Path = Path(".") / ".cache",
+        enable_stats: bool = False,
+    ) -> None:
+        super().__init__(directory=directory.as_posix())
+
+        if enable_stats:
+            self.enable_cache_statistics()
+
+    def enable_cache_statistics(self) -> None:
+        self.stats(enable=True)
+
+    def put(self, key: str, value: pd.DataFrame, expire: Optional[int] = None) -> None:
+        self.add(key=key, value=value, expire=expire)
+
+    def get_metadata(
+        self, key: str, properties: Optional[Union[str, List[str]]]
+    ) -> Optional[Dict[str, Union[str, int, float]]]:
+        if isinstance(properties, str):
+            properties = [properties]
+        _key = f"$metadata${key}"
+        metadata = cast(Optional[Dict[str, Union[str, int, float]]], self.get(_key))
+        if metadata:
+            if properties:
+                return {k: v for (k, v) in metadata.items() if k in properties}
+            return metadata
+        else:
             return None
-        self.filename = os.path.splitext(filename)[0] + ".h5"
-        self.filename = os.path.join(path, self.filename)
 
+    def put_metadata(
+        self,
+        key: str,
+        value: Dict[str, Union[str, int, float]],
+        expire: Optional[int] = None,
+    ) -> Dict[str, Union[str, int, float]]:
+        _key = f"$metadata${key}"
+        combined_value = value
+        if _key in self:
+            existing = self.get(_key)
+            if existing:
+                existing.update(value)
+                combined_value = existing
+            else:
+                combined_value = value
+            self.delete(_key)
+
+        self.add(_key, combined_value, expire=expire)
+        return combined_value
+
+    def delete_metadata(self, key: str) -> None:
+        _key = f"$metadata${key}"
+        self.delete(_key)
+
+
+class BucketCache(BaseCache):
     def _key_path(
         self,
         tagname: str,
         readtype: ReaderType,
-        ts: Union[int, pd.Timedelta],
+        ts: Union[int, timedelta],
         stepped: bool,
         status: bool,
-        starttime: Optional[pd.Timestamp] = None,
-        endtime: Optional[pd.Timestamp] = None,
+        starttime: Optional[datetime] = None,
+        endtime: Optional[datetime] = None,
     ) -> str:
         """Return a string on the form
-        /tagname/readtype[/sample_time][/stepped][/status]/_starttime_endtime
+        $tagname$readtype[$sample_time][$stepped][$status]$_starttime_endtime
         tagname: safe tagname
         sample_time: integer value. Empty for RAW.
         stepped: "stepped" if value was read as stepped. Empty if not.
         status: "status" if value contains status. Empty if not.
         starttime: The starttime of the query that created the bucket.
         endtime: The endtime of the query that created the bucket.
         """
         tagname = safe_tagname(tagname)
 
         ts = (
             int(ts.total_seconds())
-            if readtype != ReaderType.RAW and isinstance(ts, pd.Timedelta)
+            if readtype != ReaderType.RAW and isinstance(ts, timedelta)
             else ts
         )
         timespan = ""
         if starttime is not None:
             starttime_epoch = timestamp_to_epoch(starttime)
-            endtime_epoch = timestamp_to_epoch(endtime)  # type: ignore[arg-type]
-            timespan = f"/_{starttime_epoch}_{endtime_epoch}"
+            endtime_epoch = timestamp_to_epoch(endtime) if endtime else endtime
+            timespan = f"$_{starttime_epoch}_{endtime_epoch}"
 
         keyval = (
-            f"/{tagname}"
-            f"/{readtype.name}"
-            f"{(ts is not None and readtype != ReaderType.RAW) * f'/s{ts}'}"
-            f"{stepped * '/stepped'}"
-            f"{status * '/status'}"
+            f"${tagname}"
+            f"${readtype.name}"
+            f"{(ts is not None and readtype != ReaderType.RAW) * f'$s{ts}'}"
+            f"{stepped * '$stepped'}"
+            f"{status * '$status'}"
             f"{timespan}"
         )
         return keyval
 
-    def store_tag_metadata(
-        self, tagname: str, metadata: Dict[str, Union[str, int]]
-    ) -> None:
-        tagname = safe_tagname(tagname)
-        key = f"/{tagname}"
-        with pd.HDFStore(self.filename, mode="a") as f:
-            if key not in f:
-                f.put(key, pd.DataFrame())
-            origmetadata = {}
-            if "metadata" in f.get_storer(key).attrs:  # type: ignore[operator]
-                origmetadata = f.get_storer(key).attrs.metadata  # type: ignore[operator]
-            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}  # type: ignore[operator]
-
-    def fetch_tag_metadata(
-        self, tagname: str, properties: Union[str, List[str]]
-    ) -> Dict[str, Union[str, int]]:
-        res: Dict[str, Union[str, int]] = {}
-        if not os.path.isfile(self.filename):
-            return res
-        tagname = safe_tagname(tagname)
-        key = f"/{tagname}"
-        if isinstance(properties, str):
-            properties = [properties]
-        with pd.HDFStore(self.filename, mode="r") as f:
-            if key not in f or "metadata" not in f.get_storer(key).attrs:  # type: ignore[operator]
-                return {}
-            metadata = f.get_storer(key).attrs.metadata  # type: ignore[operator]
-        for p in properties:
-            if p in metadata.keys():
-                res[p] = metadata.get(p)
-        return res
-
-    def remove(self, filename: Optional[str] = None) -> None:
-        if not filename:
-            filename = self.filename
-        if os.path.isfile(filename):
-            os.unlink(filename)
-
     def store(
         self,
         df: pd.DataFrame,
         tagname: str,
         readtype: ReaderType,
-        ts: pd.Timedelta,
+        ts: timedelta,
         stepped: bool,
         status: bool,
-        starttime: pd.Timestamp,
-        endtime: pd.Timestamp,
+        starttime: datetime,
+        endtime: datetime,
     ) -> None:
         if df.empty:
             return
 
         intersecting = self.get_intersecting_datasets(
             tagname=tagname,
             readtype=readtype,
             ts=ts,
             stepped=stepped,
             status=status,
             starttime=starttime,
             endtime=endtime,
         )
         if len(intersecting) > 0:
-            with pd.HDFStore(self.filename, mode="a") as f:
-                for dataset in intersecting:
-                    this_start, this_end = self._get_intervals_from_dataset_name(
-                        dataset
-                    )
-                    starttime = min(starttime, this_start)
-                    endtime = max(endtime, this_end)
-                    df = pd.concat([df, f.get(dataset)])  # type: ignore[list-item]
-                    del f[dataset]
-            df = df[~df.index.duplicated(keep="first")].sort_index()
+            for dataset in intersecting:
+                this_start, this_end = self._get_intervals_from_dataset_name(dataset)
+                starttime = min(starttime, this_start if this_start else starttime)
+                endtime = max(endtime, this_end if this_end else endtime)
+                df2 = self.get(dataset)
+                if df2 is not None:
+                    df = pd.concat([df, df2], axis=0)
+                self.delete(dataset)
         key = self._key_path(
             tagname=tagname,
             readtype=readtype,
             ts=ts,
             stepped=stepped,
             status=status,
             starttime=starttime,
             endtime=endtime,
         )
-        with pd.HDFStore(self.filename, mode="a") as f:
-            f.put(key, df, format="table")
+        self.put(key=key, value=clean_dataframe(df))
 
     @staticmethod
     def _get_intervals_from_dataset_name(
         name: str,
-    ) -> Tuple[pd.Timestamp, pd.Timestamp]:
-        name_with_times = name.split("/")[-1]
+    ) -> Tuple[datetime, datetime]:
+        name_with_times = name.split("$")[-1]
         if not name_with_times.count("_") == 2:
             return (None, None)  # type: ignore[return-value]
         _, starttime_epoch, endtime_epoch = name_with_times.split("_")
         starttime = pd.to_datetime(int(starttime_epoch), unit="s").tz_localize("UTC")
         endtime = pd.to_datetime(int(endtime_epoch), unit="s").tz_localize("UTC")
         return starttime, endtime
 
     def get_intersecting_datasets(
         self,
         tagname: str,
         readtype: ReaderType,
-        ts: Union[int, pd.Timedelta],
+        ts: Union[int, timedelta],
         stepped: bool,
         status: bool,
-        starttime: pd.Timestamp,
-        endtime: pd.Timestamp,
+        starttime: datetime,
+        endtime: datetime,
     ) -> List[str]:
-        if not os.path.isfile(self.filename):
+        if not len(self) > 0:
             return []
         intersecting_datasets = []
-        with pd.HDFStore(self.filename, mode="r") as f:
-            for bucket in f.walk(
-                where=self._key_path(
-                    tagname=tagname,
-                    readtype=readtype,
-                    starttime=None,
-                    endtime=None,
-                    ts=ts,
-                    stepped=stepped,
-                    status=status,
+        for dataset in self.iterkeys():
+            target_key = self._key_path(
+                tagname=tagname,
+                readtype=readtype,
+                starttime=None,
+                endtime=None,
+                ts=ts,
+                stepped=stepped,
+                status=status,
+            )
+            if target_key in dataset:
+                starttime_ds, endtime_ds = self._get_intervals_from_dataset_name(
+                    dataset
                 )
-            ):
-                for leaf in bucket[2]:
-                    dataset = bucket[0] + "/" + leaf
-                    starttime_ds, endtime_ds = self._get_intervals_from_dataset_name(
-                        dataset
-                    )
-                    if endtime_ds >= starttime and endtime >= starttime_ds:
-                        intersecting_datasets.append(dataset)
+                if endtime_ds >= starttime and endtime >= starttime_ds:
+                    intersecting_datasets.append(dataset)
         return intersecting_datasets
 
     def get_missing_intervals(
         self,
         tagname: str,
         readtype: ReaderType,
-        ts: Union[int, pd.Timedelta],
+        ts: Union[int, timedelta],
         stepped: bool,
         status: bool,
-        starttime: pd.Timestamp,
-        endtime: pd.Timestamp,
-    ) -> List[Tuple[pd.Timestamp, pd.Timestamp]]:
+        starttime: datetime,
+        endtime: datetime,
+    ) -> List[Tuple[datetime, datetime]]:
         datasets = self.get_intersecting_datasets(
             tagname=tagname,
             readtype=readtype,
             ts=ts,
             stepped=stepped,
             status=status,
             starttime=starttime,
@@ -245,229 +274,104 @@
                     missing_intervals.append((r[0], b[0]))
         return missing_intervals
 
     def fetch(
         self,
         tagname: str,
         readtype: ReaderType,
-        ts: int,
+        ts: Union[int, timedelta],
         stepped: bool,
         status: bool,
-        starttime: pd.Timestamp,
-        endtime: pd.Timestamp,
+        starttime: datetime,
+        endtime: datetime,
     ) -> pd.DataFrame:
         df = pd.DataFrame()
-        if not os.path.isfile(self.filename):
+        if not len(self) > 0:
             return df
 
+        if isinstance(ts, timedelta):
+            ts = int(ts.total_seconds())
+
         datasets = self.get_intersecting_datasets(
             tagname=tagname,
             readtype=readtype,
             ts=ts,
             stepped=stepped,
             status=status,
             starttime=starttime,
             endtime=endtime,
         )
 
-        with pd.HDFStore(self.filename, mode="r") as f:
-            for dataset in datasets:
-                # df = df.append(
-                #     f.select(dataset, where="index >= starttime and index <= endtime")
-                # )
-                df = pd.concat(
-                    [
-                        df,
-                        f.select(  # type: ignore[list-item]
-                            dataset, where="index >= starttime and index <= endtime"
-                        ),
-                    ]
-                )
+        for dataset in datasets:
+            df2 = self.get(dataset)
+            if df2 is not None:
+                df = pd.concat([df, df2.loc[starttime:endtime]], axis=0)  # type: ignore[call-overload, misc]
 
-        return df.sort_index()
+        return clean_dataframe(df)
 
 
-class SmartCache:
-    def __init__(self, filename: str, path: str = ".") -> None:
-        if not find_spec("tables"):
-            warnings.warn("Package 'tables' not installed. Disabling cache.")
-            return None
-        self.filename = os.path.splitext(filename)[0] + ".h5"
-        self.filename = os.path.join(path, self.filename)
-        # self.open(self.filename)
-
-    # def open(self, filename=None):
-    #     if filename is None:
-    #         filename = self.filename
-    #     self.hdfstore = pd.HDFStore(filename)
-    #
-    # def close(self):
-    #     self.hdfstore.close()
-
+class SmartCache(BaseCache):
     @staticmethod
     def key_path(
         df: Union[str, pd.DataFrame],
         readtype: ReaderType,
-        ts: Optional[Union[int, pd.Timedelta]] = None,
+        ts: Optional[Union[int, timedelta]] = None,
     ) -> str:
         """Return a string on the form
-        XXX/sYY/ZZZ where XXX is the ReadType, YY is the interval between samples
+        XXX$sYY$ZZZ where XXX is the ReadType, YY is the interval between samples
         (in seconds) and ZZZ is a safe tagname.
         """
-        name = list(df)[0] if isinstance(df, pd.DataFrame) else df
-        name = safe_tagname(name)  # type: ignore[arg-type]
-        ts = int(ts.total_seconds()) if isinstance(ts, pd.Timedelta) else ts
+        name = str(list(df)[0]) if isinstance(df, pd.DataFrame) else df
+        name = safe_tagname(name)
+        ts = int(ts.total_seconds()) if isinstance(ts, timedelta) else ts
         if readtype != ReaderType.RAW:
             if ts is None:
                 # Determine sample time by reading interval between first two
                 # samples of dataframe.
                 if isinstance(df, pd.DataFrame):
                     interval = int(df[0:2].index.to_series().diff().mean().value / 1e9)  # type: ignore[attr-defined]
                 else:
                     raise TypeError
             else:
                 interval = int(ts)
-            return f"{readtype.name}/s{interval}/{name}"
+            return f"{readtype.name}$s{interval}${name}"
         else:
-            return f"{readtype.name}/{name}"
+            return f"{readtype.name}${name}"
 
     def store(
         self,
         df: pd.DataFrame,
         readtype: ReaderType,
-        ts: Optional[Union[int, pd.Timedelta]] = None,
+        ts: Optional[Union[int, timedelta]] = None,
     ) -> None:
         key = self.key_path(df=df, readtype=readtype, ts=ts)
         if df.empty:
             return  # Weirdness ensues when using empty df in select statement below
-        with pd.HDFStore(self.filename, mode="a") as f:
-            if key in f:
-                idx = f.select(  # noqa: F841
-                    key, where="index in df.index", columns=["index"]
-                ).index
-                f.append(key, df.query("index not in @idx"))
-            else:
-                f.append(key, df)
+        if key in self:
+            df2 = self.get(key)
+            if df2 is not None:
+                df = pd.concat([df, df2], axis=0)
+            self.delete(key=key)
+            self.put(
+                key=key,
+                value=clean_dataframe(df),
+            )
+        else:
+            self.put(key, df)
 
     def fetch(
         self,
         tagname: str,
         readtype: ReaderType,
-        ts: Optional[Union[int, pd.Timestamp]] = None,
-        start_time: Optional[pd.Timestamp] = None,
-        stop_time: Optional[pd.Timestamp] = None,
+        ts: Optional[Union[int, timedelta]] = None,
+        start_time: Optional[datetime] = None,
+        stop_time: Optional[datetime] = None,
     ) -> pd.DataFrame:
-        df = pd.DataFrame()
-        if not os.path.isfile(self.filename):
-            return df
-        key = self.key_path(df=tagname, readtype=readtype, ts=ts)  # type: ignore[arg-type]
-        where = []
+        key = self.key_path(df=tagname, readtype=readtype, ts=ts)
+        df = cast(Optional[pd.DataFrame], self.get(key=key))
+        if df is None:
+            return pd.DataFrame()
         if start_time is not None:
-            where.append("index >= start_time")
+            df = df.loc[df.index >= start_time]
         if stop_time is not None:
-            where.append("index <= stop_time")
-        wheretxt = " and ".join(where)
-        with pd.HDFStore(self.filename, mode="r") as f:
-            if key in f:
-                if wheretxt:
-                    df = f.select(key, where=wheretxt)  # type: ignore[assignment]
-                else:
-                    df = f.select(key)  # type: ignore[assignment]
-        return df.sort_index()
-
-    def store_tag_metadata(
-        self, tagname: str, metadata: Dict[str, Union[str, int]]
-    ) -> None:
-        tagname = safe_tagname(tagname)
-        key = f"/metadata/{tagname}"
-        with pd.HDFStore(self.filename, mode="a") as f:
-            if key not in f:
-                f.put(key, pd.DataFrame())
-            origmetadata = {}
-            if "metadata" in f.get_storer(key).attrs:  # type: ignore[operator]
-                origmetadata = f.get_storer(key).attrs.metadata  # type: ignore[operator]
-            f.get_storer(key).attrs.metadata = {**origmetadata, **metadata}  # type: ignore[operator]
-
-    def fetch_tag_metadata(
-        self, tagname: str, properties: Union[str, List[str]]
-    ) -> Dict[str, Union[str, int]]:
-        res: Dict[str, Union[str, int]] = {}
-        if not os.path.isfile(self.filename):
-            return res
-        tagname = safe_tagname(tagname)
-        key = f"/metadata/{tagname}"
-        if isinstance(properties, str):
-            properties = [properties]
-        with pd.HDFStore(self.filename, mode="r") as f:
-            if key not in f or "metadata" not in f.get_storer(key).attrs:  # type: ignore[operator]
-                return {}
-            metadata = f.get_storer(key).attrs.metadata  # type: ignore[operator]
-        for p in properties:
-            if p in metadata.keys():
-                res[p] = metadata.get(p)
-        return res
-
-    def remove(self, filename: Optional[str] = None) -> None:
-        if not filename:
-            filename = self.filename
-            # self.close()
-        if os.path.isfile(filename):
-            os.unlink(filename)
-
-    def _match_tag(
-        self,
-        key: str,
-        readtype: Optional[Union[List[ReaderType], ReaderType]] = None,
-        ts: Optional[List[Optional[Union[int, pd.Timestamp]]]] = None,
-        tagname: Optional[Union[List[str], str]] = None,
-    ) -> bool:
-        def readtype_to_str(rt):  # type: ignore
-            return getattr(
-                rt, "name", rt
-            )  # if isinstance(rt, ReaderType) always returns False...?
-
-        def timedelta_to_str(t):  # type: ignore[no-untyped-def]
-            if isinstance(t, pd.Timedelta):
-                return str(int(t.total_seconds()))
-            return t
-
-        key = "/" + key.lstrip("/")  # Ensure absolute path:
-        readtype = readtype if isinstance(readtype, list) else [readtype]  # type: ignore[list-item]
-        ts = ts if isinstance(ts, list) else [ts]
-        tagname = tagname if isinstance(tagname, list) else [tagname]  # type: ignore[list-item]
-        readtype = list(map(readtype_to_str, readtype))
-        ts = list(map(timedelta_to_str, ts))
-        if tagname[0] is not None:
-            tagname = list(map(safe_tagname, tagname))
-        # print(f"Readtype: {readtype}, ts: {ts}, tagname: {tagname}")
-        elements = key.split("/")[1:]
-        if len(elements) == 2:
-            elements.insert(1, None)  # type: ignore[arg-type]
-        else:
-            elements[1] = int(  # type: ignore[call-overload]
-                elements[1][1:]
-            )  # Discard the initial s
-        if elements[0] not in readtype and readtype[0] is not None:  # type: ignore[comparison-overlap]
-            # print(f"{elements[0]} not in {readtype}")
-            return False
-        if elements[1] not in ts and ts[0] is not None:
-            # print(f"{elements[1]} not in {ts}")
-            return False
-        if elements[2] not in tagname and tagname[0] is not None:
-            # print(f"{elements[2]} not in {tagname}")
-            return False
-        return True
-
-    def delete_key(
-        self,
-        tagname: Optional[str] = None,
-        readtype: Optional[ReaderType] = None,
-        ts: Optional[Union[int, pd.Timestamp]] = None,
-    ) -> None:
-        with pd.HDFStore(self.filename) as f:
-            for key in f:
-                if self._match_tag(key=key, tagname=tagname, readtype=readtype, ts=ts):  # type: ignore[arg-type]
-                    f.remove(key)  # type: ignore[operator]
-
-    def _get_hdfstore(self, mode: Literal["a", "w", "r", "r+"] = "r") -> pd.HDFStore:
-        f = pd.HDFStore(self.filename, mode=mode)
-        return f
+            df = df.loc[df.index <= stop_time]
+        return df
```

### Comparing `tagreader-4.0.3/tagreader/clients.py` & `tagreader-4.1.1/tagreader/clients.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import os
 import warnings
 from datetime import datetime, timedelta
 from itertools import groupby
 from operator import itemgetter
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pandas as pd
+import pytz
 
 from tagreader.cache import BucketCache, SmartCache
 from tagreader.logger import logger
 from tagreader.utils import (
+    IMSType,
     ReaderType,
+    convert_to_pydatetime,
     ensure_datetime_with_tz,
     find_registry_key,
     find_registry_key_from_name,
     is_windows,
 )
 from tagreader.web_handlers import (
     AspenHandlerWeb,
@@ -30,65 +34,56 @@
 
     from tagreader.odbc_handlers import (
         AspenHandlerODBC,
         PIHandlerODBC,
         list_aspen_sources,
         list_pi_sources,
     )
-    from tagreader.utils import winreg
 
-
-class DuplicateTagsWarning(UserWarning):
-    pass
-
-
-warnings.simplefilter("always", DuplicateTagsWarning)
+NONE_START_TIME = datetime(1970, 1, 1, tzinfo=pytz.UTC)
 
 
 def list_sources(
-    imstype: str,
+    imstype: Union[IMSType, str],
     url: Optional[str] = None,
     auth: Optional[Any] = None,
     verifySSL: bool = True,
 ) -> List[str]:
-    accepted_values = ["piwebapi", "aspenone"]
-    win_accepted_values = ["pi", "aspen", "ip21"]
+    if isinstance(imstype, str):
+        try:
+            imstype = getattr(IMSType, imstype.upper())
+        except AttributeError:
+            raise ValueError(
+                f"imstype needs to be one of {', '.join([v for v in IMSType.__members__.values()])}."
+                f" We suggest to use the tagreader.IMSType enumerator when initiating a client."
+            )
+    accepted_values = [IMSType.PIWEBAPI, IMSType.ASPENONE]
+    win_accepted_values = [IMSType.PI, IMSType.ASPEN, IMSType.IP21]
     if is_windows():
         accepted_values.extend(win_accepted_values)
 
-    if imstype is None or imstype.lower() not in accepted_values:
-        import platform
-
-        raise ValueError(
-            f"Input `imstype` must be one of {accepted_values} when called from {platform.system()} environment."
-        )
-
-    if imstype.lower() == "pi":
+    if imstype == IMSType.PI:
         return list_pi_sources()
-    elif imstype.lower() in ["aspen", "ip21"]:
+    elif imstype in [IMSType.ASPEN, IMSType.IP21]:
         return list_aspen_sources()
-    elif imstype.lower() == "piwebapi":
+    elif imstype == IMSType.PIWEBAPI:
         if auth is None:
             auth = get_auth_pi()
-        if verifySSL is None:
-            verifySSL = True
         return list_piwebapi_sources(url=url, auth=auth, verifySSL=verifySSL)
-    elif imstype.lower() == "aspenone":
+    elif imstype == IMSType.ASPENONE:
         if auth is None:
             auth = get_auth_aspen()
-        if verifySSL is None:
-            verifySSL = True
         return list_aspenone_sources(url=url, auth=auth, verifySSL=verifySSL)
 
 
 def get_missing_intervals(
     df: pd.DataFrame,
-    start_time: pd.Timestamp,
-    stop_time: pd.Timestamp,
-    ts: Optional[Union[int, pd.Timestamp]],
+    start_time: datetime,
+    stop_time: datetime,
+    ts: Optional[timedelta],
     read_type: ReaderType,
 ):
     if (
         read_type == ReaderType.RAW
     ):  # Fixme: How to check for completeness for RAW data?
         return [[start_time, stop_time]]
     seconds = int(ts.total_seconds())
@@ -97,28 +92,31 @@
         return []
     values_in_df = tvec.isin(df.index)
     missing_intervals = []
     for k, g in groupby(enumerate(values_in_df), lambda ix: ix[1]):
         if not k:
             seq = list(map(itemgetter(0), g))
             missing_intervals.append(
-                (pd.Timestamp(tvec[seq[0]]), pd.Timestamp(tvec[seq[-1]]))
+                (
+                    pd.Timestamp(tvec[seq[0]]).to_pydatetime(),
+                    pd.Timestamp(tvec[seq[-1]]).to_pydatetime(),
+                )
             )
             # Should be unnecessary to fetch overlapping points since get_next_timeslice
             # ensures start <= t <= stop
             # missingintervals.append((pd.Timestamp(tvec[seq[0]]),
             #                          pd.Timestamp(tvec[min(seq[-1]+1, len(tvec)-1)])))
     return missing_intervals
 
 
 def get_next_timeslice(
-    start_time: pd.Timestamp,
-    stop_time: pd.Timestamp,
-    ts: Optional[Union[int, pd.Timestamp]],
-    max_steps: Optional[int] = None,
+    start_time: datetime,
+    stop_time: datetime,
+    ts: Optional[timedelta],
+    max_steps: Optional[int],
 ) -> Tuple[datetime, datetime]:
     if max_steps is None:
         calc_stop_time = stop_time
     else:
         calc_stop_time = start_time + ts * max_steps
     calc_stop_time = min(stop_time, calc_stop_time)
     # Ensure we include the last data point.
@@ -136,14 +134,15 @@
     identifying the correct key to use by locating the UUID for Aspen SQLplus
     services located under Aspen SQLplus service component. Then we find the
     host and port based on the path above and the UUID.
     """
 
     if not is_windows():
         return None
+    import winreg
 
     regkey_clsid = winreg.OpenKey(
         winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Classes\Wow6432Node\CLSID"
     )
     regkey, _ = find_registry_key_from_name(
         regkey_clsid, "Aspen SQLplus service component"
     )
@@ -176,14 +175,15 @@
     :param datasource: Name of data source
     :return: host, port
     :type: tuple(string, int)
     """
 
     if not is_windows():
         return None
+    import winreg
 
     try:
         reg_key = winreg.OpenKey(
             winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Wow6432Node\PISystem\PI-SDK"
         )
         reg_key_handles = find_registry_key(reg_key, "ServerHandles")
         reg_site_key = find_registry_key(reg_key_handles, datasource)
@@ -198,35 +198,34 @@
             port = int(winreg.QueryValueEx(reg_site_key, "port")[0])
             return host, port
     except FileNotFoundError:
         return None
 
 
 def get_handler(
-    imstype: str,
+    imstype: Optional[IMSType],
     datasource: str,
-    url: Optional[str] = None,
-    host: Optional[str] = None,
-    port: Optional[int] = None,
-    options: Dict[str, Union[int, float, str]] = {},
-    verifySSL: Optional[bool] = None,
-    auth: Optional[Any] = None,
+    url: Optional[str],
+    host: Optional[str],
+    port: Optional[int],
+    options: Dict[str, Union[int, float, str]],
+    verifySSL: Optional[bool],
+    auth: Optional[Any],
 ):
     if imstype is None:
-        if datasource in list_aspenone_sources():
-            imstype = "aspenone"
-        elif datasource in list_piwebapi_sources():
-            imstype = "piwebapi"
-
-    accepted_imstypes = ["pi", "aspen", "ip21", "piwebapi", "aspenone"]
+        if datasource in list_aspenone_sources(
+            url=None, auth=None, verifySSL=verifySSL
+        ):
+            imstype = IMSType.ASPENONE
+        elif datasource in list_piwebapi_sources(
+            url=None, auth=None, verifySSL=verifySSL
+        ):
+            imstype = IMSType.PIWEBAPI
 
-    if not imstype or imstype.lower() not in accepted_imstypes:
-        raise ValueError(f"`imstype` must be one of {accepted_imstypes}")
-
-    if imstype.lower() == "pi":
+    if imstype == IMSType.PI:
         if not is_windows():
             raise RuntimeError(
                 "ODBC drivers not available for non-Windows environments. "
                 "Try Web API ('piwebapi') instead."
             )
         if "PI ODBC Driver" not in pyodbc.drivers():
             raise RuntimeError(
@@ -241,15 +240,15 @@
                     "Do you have correct permissions?"
                 )
             host, port = hostport
         if port is None:
             port = 5450
         return PIHandlerODBC(host=host, port=port, options=options)
 
-    if imstype.lower() in ["aspen", "ip21"]:
+    if imstype in [IMSType.ASPEN, IMSType.IP21]:
         if not is_windows():
             raise RuntimeError(
                 "ODBC drivers not available for non-Windows environments. "
                 "Try Web API ('aspenone') instead."
             )
         if "AspenTech SQLplus" not in pyodbc.drivers():
             raise RuntimeError(
@@ -264,62 +263,74 @@
                     "Do you have correct permissions?"
                 )
             host, port = hostport
         if port is None:
             port = 10014
         return AspenHandlerODBC(host=host, port=port, options=options)
 
-    if imstype.lower() == "piwebapi":
+    if imstype == IMSType.PIWEBAPI:
         return PIHandlerWeb(
             url=url,
             datasource=datasource,
             options=options,
             verifySSL=verifySSL,
             auth=auth,
         )
 
-    if imstype.lower() in ["aspenone"]:
+    if imstype == IMSType.ASPENONE:
         return AspenHandlerWeb(
             datasource=datasource,
             url=url,
             options=options,
             verifySSL=verifySSL,
             auth=auth,
         )
 
+    raise ValueError(
+        f"Could not infer IMSType for datasource: {datasource}."
+        f"Please specify correct datasource, imstype or host, or refer to the user docs."
+    )
+
 
 class IMSClient:
     def __init__(
         self,
         datasource: str,
-        imstype: Optional[str] = None,
-        tz: str = "Europe/Oslo",
+        imstype: Optional[Union[str, IMSType]] = None,
+        tz: pytz.timezone = pytz.timezone("Europe/Oslo"),
         url: Optional[str] = None,
         host: Optional[str] = None,
         port: Optional[int] = None,
         handler_options: Dict[str, Union[int, float, str]] = {},  # noqa:
         verifySSL: bool = True,
         auth: Optional[Any] = None,
     ):
-        self.handler = None
-        self.datasource = datasource.lower()  # FIXME
+        if isinstance(imstype, str):
+            try:
+                imstype = getattr(IMSType, imstype.upper())
+            except AttributeError:
+                raise ValueError(
+                    f"imstype needs to be one of {', '.join([v for v in IMSType.__members__.values()])}."
+                    f" We suggest to use the tagreader.IMSType enumerator when initiating a client."
+                )
+
         self.tz = tz
         self.handler = get_handler(
             imstype=imstype,
             datasource=datasource,
             url=url,
             host=host,
             port=port,
             options=handler_options,
             verifySSL=verifySSL,
             auth=auth,
         )
-        self.cache = SmartCache(filename=datasource)
+        self.cache = SmartCache(directory=Path(".") / ".cache" / datasource)
 
-    def connect(self):
+    def connect(self) -> None:
         self.handler.connect()
 
     def search_tag(
         self, tag: Optional[str] = None, desc: Optional[str] = None
     ) -> List[Tuple[str, str]]:
         warnings.warn("This function is deprecated. Please call 'search()' instead")
         return self.search(tag=tag, desc=desc)
@@ -333,17 +344,17 @@
         return self.handler._get_tag_metadata(
             tag
         )  # noqa: Should probably expose this as a public method if needed.
 
     def _read_single_tag(
         self,
         tag: str,
-        start_time: Optional[pd.Timestamp],
-        stop_time: Optional[pd.Timestamp],
-        ts: Optional[Union[int, pd.Timestamp]],
+        start_time: Optional[datetime],
+        stop_time: Optional[datetime],
+        ts: timedelta,
         read_type: ReaderType,
         get_status: bool,
         cache: Optional[Union[BucketCache, SmartCache]],
     ):
         if read_type == ReaderType.SNAPSHOT:
             metadata = self._get_metadata(tag)
             df = self.handler.read_tag(
@@ -461,47 +472,45 @@
 
     def get_units(self, tags: Union[str, List[str]]):
         if isinstance(tags, str):
             tags = [tags]
         units = {}
         for tag in tags:
             if self.cache is not None:
-                r = self.cache.fetch_tag_metadata(tagname=tag, properties="unit")
-                if "unit" in r:
+                r = self.cache.get_metadata(key=tag, properties="unit")
+                if r is not None and "unit" in r:
                     units[tag] = r["unit"]
             if tag not in units:
                 unit = self.handler._get_tag_unit(tag)
                 if self.cache is not None and unit is not None:
-                    self.cache.store_tag_metadata(tagname=tag, metadata={"unit": unit})
+                    self.cache.put_metadata(key=tag, value={"unit": unit})
                 units[tag] = unit
         return units
 
     def get_descriptions(self, tags: Union[str, List[str]]) -> Dict[str, str]:
         if isinstance(tags, str):
             tags = [tags]
         descriptions = {}
         for tag in tags:
             if self.cache is not None:
-                r = self.cache.fetch_tag_metadata(tagname=tag, properties="description")
-                if "description" in r:
+                r = self.cache.get_metadata(key=tag, properties="description")
+                if r is not None and "description" in r:
                     descriptions[tag] = r["description"]
             if tag not in descriptions:
                 desc = self.handler._get_tag_description(tag)
                 if self.cache is not None and desc is not None:
-                    self.cache.store_tag_metadata(
-                        tagname=tag, metadata={"description": desc}
-                    )
+                    self.cache.put_metadata(key=tag, value={"description": desc})
                 descriptions[tag] = desc
         return descriptions
 
     def read_tags(
         self,
         tags: Union[str, List[str]],
-        start_time: Optional[Union[datetime, pd.Timestamp, str]],
-        stop_time: Optional[Union[datetime, pd.Timestamp, str]],
+        start_time: Optional[Union[datetime, pd.Timestamp, str]] = None,
+        stop_time: Optional[Union[datetime, pd.Timestamp, str]] = None,
         ts: Optional[Union[timedelta, pd.Timedelta]] = timedelta(seconds=60),
         read_type: ReaderType = ReaderType.INT,
         get_status: bool = False,
     ):
         logger.warn(
             (
                 "This function has been renamed to read() and is deprecated. "
@@ -518,15 +527,15 @@
         )
 
     def read(
         self,
         tags: Union[str, List[str]],
         start_time: Optional[Union[datetime, pd.Timestamp, str]] = None,
         end_time: Optional[Union[datetime, pd.Timestamp, str]] = None,
-        ts: Optional[Union[timedelta, pd.Timedelta, int]] = 60,
+        ts: Union[timedelta, pd.Timedelta, int] = timedelta(seconds=60),
         read_type: ReaderType = ReaderType.INT,
         get_status: bool = False,
     ) -> pd.DataFrame:
         """Reads values for the specified [tags] from the IMS server for the
         time interval from [start_time] to [stop_time] in intervals [ts].
 
         The interval [ts] can be specified as pd.Timedelta or as an integer,
@@ -537,28 +546,58 @@
         All possible values for read_type are defined in the ReaderType class,
         which can be imported as follows:
             from utils import ReaderType
 
         Values for ReaderType.* that should work for all handlers are:
             INT, RAW, MIN, MAX, RNG, AVG, VAR, STD and SNAPSHOT
         """
-
         if isinstance(tags, str):
             tags = [tags]
+        if isinstance(read_type, str):
+            try:
+                read_type = getattr(ReaderType, read_type)
+            except AttributeError:
+                ValueError(
+                    "readtype needs to be of type ReaderType.* or a legal value. Please refer to the docstring."
+                )
         if read_type in [ReaderType.RAW, ReaderType.SNAPSHOT] and len(tags) > 1:
             raise RuntimeError(
                 "Unable to read raw/sampled data for multiple tags since they don't "
                 "share time vector. Read one at a time."
             )
+
+        if isinstance(tags, str):
+            tags = [tags]
+
+        if start_time is None:
+            start_time = NONE_START_TIME
+        elif isinstance(start_time, (str, pd.Timestamp)):
+            try:
+                start_time = convert_to_pydatetime(start_time)
+            except ValueError:
+                start_time = convert_to_pydatetime(start_time)
+        if end_time is None:
+            end_time = datetime.utcnow()
+        elif isinstance(end_time, (str, pd.Timestamp)):
+            end_time = convert_to_pydatetime(end_time)
+
+        if isinstance(ts, pd.Timedelta):
+            ts = ts.to_pytimedelta()
+        elif isinstance(ts, int):
+            ts = timedelta(seconds=ts)
+        elif not isinstance(ts, timedelta):
+            raise ValueError(
+                "ts needs to be either a None, timedelta or and integer (number of seconds)."
+                f" Given type: {type(ts)}"
+            )
+
         if read_type != ReaderType.SNAPSHOT:
             start_time = ensure_datetime_with_tz(start_time, tz=self.tz)
         if end_time:
             end_time = ensure_datetime_with_tz(end_time, tz=self.tz)
-        if not isinstance(ts, pd.Timedelta):
-            ts = pd.Timedelta(ts, unit="s")
 
         oldtags = tags
         tags = list(dict.fromkeys(tags))
         if len(oldtags) > len(tags):
             duplicates = set([x for n, x in enumerate(oldtags) if x in oldtags[:n]])
             logger.warning(
                 f"Duplicate tags found, removed duplicates: {', '.join(duplicates)}"
```

### Comparing `tagreader-4.0.3/tagreader/odbc_handlers.py` & `tagreader-4.1.1/tagreader/odbc_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 import warnings
+from datetime import datetime, timedelta
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pyodbc
+import pytz
 
+from tagreader.logger import logger
 from tagreader.utils import ReaderType, find_registry_key, logging, winreg
 
 logging.basicConfig(
     format=" %(asctime)s %(levelname)s: %(message)s", level=logging.INFO
 )
 
 
@@ -41,15 +44,15 @@
     )
     num_sources, _, _ = winreg.QueryInfoKey(reg_adsa)
     for i in range(0, num_sources):
         source_list.append(winreg.EnumKey(reg_adsa, i))
     return source_list
 
 
-def list_pi_sources():
+def list_pi_sources() -> List[str]:
     source_list = []
     reg_key = winreg.OpenKey(
         winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\Wow6432Node\PISystem\PI-SDK"
     )
     reg_key = find_registry_key(reg_key, "ServerHandles")
     if reg_key is None:
         reg_key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, r"SOFTWARE\PISystem\PI-SDK")
@@ -60,38 +63,38 @@
             source_list.append(winreg.EnumKey(reg_key, i))
     return source_list
 
 
 class AspenHandlerODBC:
     def __init__(
         self,
-        host: Optional[str] = None,
-        port: Optional[int] = None,
-        options: Dict[str, Union[int, float, str]] = {},
+        host: Optional[str],
+        port: Optional[int],
+        options: Dict[str, Union[int, float, str]],
     ):
         self.host = host
         self.port = port
         self.conn = None
         self.cursor = None
         self._max_rows = options.get("max_rows", 100000)
         self._connection_string = options.get("connection_string", None)
 
-    def generate_connection_string(self):
+    def generate_connection_string(self) -> str:
         if self._connection_string is None:
             return f"DRIVER={{AspenTech SQLPlus}};HOST={self.host};PORT={self.port};READONLY=Y;MAXROWS={self._max_rows}"
         else:
             return self._connection_string
 
     @staticmethod
     def generate_read_query(
         tag: str,
         mapdef: Optional[Dict[str, str]],
-        start_time: pd.Timestamp,
-        stop_time: pd.Timestamp,
-        sample_time: Optional[Union[int, pd.Timestamp]],
+        start_time: datetime,
+        stop_time: datetime,
+        sample_time: Optional[timedelta],
         read_type: ReaderType,
         get_status: bool = False,
     ):
         if mapdef is None:
             mapdef = {}
         if read_type in [
             ReaderType.COUNT,
@@ -106,23 +109,25 @@
         # TODO: How to interpret ip_input_quality and ip_value_quality
         # which use a different numeric schema (e.g. -1) than status from
         # history table (0, 1, 2, 4, 5, 6)
         if get_status and read_type == ReaderType.SNAPSHOT:
             raise NotImplementedError
 
         if read_type == ReaderType.SNAPSHOT and stop_time is not None:
-            raise NotImplementedError(
-                "Timestamp not supported for IP.21 ODBC connection using 'SNAPSHOT'. "
-                "Try the web API 'aspenone' instead."
+            stop_time = None
+            logger.warning(
+                "End time is not supported for Aspen ODBC connection using 'SNAPSHOT'."
+                "Try the web API 'piwebapi' instead."
             )
 
         seconds = 0
         if read_type != ReaderType.SNAPSHOT:
-            start_time = start_time.tz_convert("UTC")
-            stop_time = stop_time.tz_convert("UTC")
+            start_time = start_time.astimezone(pytz.UTC)
+            if stop_time:
+                stop_time = stop_time.astimezone(pytz.UTC)
             seconds = int(sample_time.total_seconds())
             if read_type == ReaderType.SAMPLED:
                 seconds = 0
             else:
                 if seconds <= 0:
                     raise NotImplementedError
                     # sample_time = (stop_time-start_time).totalseconds
@@ -205,15 +210,15 @@
     def connect(self):
         connection_string = self.generate_connection_string()
         # The default autocommit=False is not supported by PI odbc driver.
         self.conn = pyodbc.connect(connection_string, autocommit=True)
         self.cursor = self.conn.cursor()
 
     @staticmethod
-    def _generate_query_get_mapdef_for_search(tag):
+    def _generate_query_get_mapdef_for_search(tag: str) -> str:
         query = [
             "SELECT DISTINCT a.name as tagname, m.NAME, m.MAP_DefinitionRecord,",
             "m.MAP_IsDefault, m.MAP_Description, m.MAP_Units, m.MAP_Base, m.MAP_Range",
             "FROM all_records a",
             "LEFT JOIN atmapdef m ON a.definition = m.MAP_DefinitionRecord",
             "WHERE a.name",
         ]
@@ -236,15 +241,15 @@
                 mapdef[t["tagname"]] = [t]
             else:
                 mapdef[t["tagname"]].append(t)
         return mapdef
 
     @staticmethod
     def _generate_query_search_tag(
-        mapdef: Optional[Dict[str, str]], desc: Optional[str] = None
+        mapdef: Optional[Dict[str, str]], desc: Optional[str]
     ):
         if mapdef["MAP_DefinitionRecord"] is None:
             return None
         query = [
             f"SELECT \"{mapdef['MAP_Description']}\"",
             f"FROM {mapdef['MAP_DefinitionRecord']}",
             f"WHERE name = '{mapdef['tagname']}'",
@@ -284,17 +289,18 @@
     def _get_default_mapdef(self, tagname: str) -> Optional[Dict[str, str]]:
         mapdefs = self._get_mapdefs(tagname)
         for mapdef in mapdefs:
             if mapdef["MAP_IsDefault"] == "TRUE":
                 return mapdef
         return None
 
-    def search(
-        self, tag: Optional[str] = None, desc: Optional[str] = None
-    ) -> List[Tuple[str, str]]:
+    def search(self, tag: Optional[str], desc: Optional[str]) -> List[Tuple[str, str]]:
+        if tag is None:
+            raise ValueError("Tag is a required argument")
+
         tag = tag.replace("*", "%") if isinstance(tag, str) else None
         desc = desc.replace("*", "%") if isinstance(desc, str) else None
 
         mapdef = self._get_mapdef_for_search(tag)
 
         res = []
         for tagname in mapdef:  # TODO: Refactor
@@ -347,25 +353,25 @@
         if not res.description:
             res.description = ""
         return res.description
 
     def read_tag(
         self,
         tag: str,
-        start_time: pd.Timestamp,
-        stop_time: pd.Timestamp,
-        sample_time: Optional[Union[int, pd.Timestamp]],
+        start_time: datetime,
+        stop_time: datetime,
+        sample_time: Optional[timedelta],
         read_type: ReaderType,
-        metadata: Optional[Dict[str, str]] = None,
+        metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         (cleantag, mapping) = tag.split(";") if ";" in tag else (tag, None)
         mapdef = dict()
 
-        if mapping is not None:
+        if isinstance(mapping, str):
             mapdef = self._get_specific_mapdef(tagname=cleantag, mapping=mapping)
         query = self.generate_read_query(
             tag=cleantag,
             mapdef=mapdef,
             start_time=start_time,
             stop_time=stop_time,
             sample_time=sample_time,
@@ -404,17 +410,17 @@
                 res = pd.read_sql(query, self.conn)
             return res
 
 
 class PIHandlerODBC:
     def __init__(
         self,
-        host: Optional[str] = None,
-        port: Optional[int] = None,
-        options: Dict[str, Union[int, float, str]] = {},
+        host: Optional[str],
+        port: Optional[int],
+        options: Dict[str, Union[int, float, str]],
     ):
         self.host = host
         self.port = port
         self.conn = None
         self.cursor = None
         self._max_rows = options.get("max_rows", 100000)
         # TODO: Find default das_server under
@@ -422,68 +428,70 @@
         # It seems that is actually not possible anymore.
         # ws3099.statoil.net
         self._das_server = options.get("das_server", "piwebapi.equinor.com")
         self._connection_string = options.get("connection_string", None)
 
         # print(self._das_server)
 
-    def generate_connection_string(self):
+    def generate_connection_string(self) -> str:
         if self._connection_string is None:
             return (
                 f"DRIVER={{PI ODBC Driver}};Server={self._das_server};"
                 "Trusted_Connection=Yes;Command Timeout=1800;Provider Type=PIOLEDB;"
                 f'Provider String={{Data source={self.host.replace(".statoil.net", "")};'
                 "Integrated_Security=SSPI;Time Zone=UTC};"
             )
         else:
             return self._connection_string
 
     @staticmethod
-    def generate_search_query(tag: Optional[str] = None, desc: Optional[str] = None):
+    def generate_search_query(tag: Optional[str], desc: Optional[str]):
         query = ["SELECT tag, descriptor as description FROM pipoint.pipoint2 WHERE"]
         if tag is not None:
             query.extend(["tag LIKE '{tag}'".format(tag=tag.replace("*", "%"))])
         if tag is not None and desc is not None:
             query.extend(["AND"])
         if desc is not None:
             query.extend(
                 ["descriptor LIKE '{desc}'".format(desc=desc.replace("*", "%"))]
             )
         return " ".join(query)
 
     def generate_read_query(
         self,
         tag: str,
-        start_time: pd.Timestamp,
-        stop_time: pd.Timestamp,
-        sample_time: Optional[Union[int, pd.Timestamp]],
+        start_time: datetime,
+        stop_time: datetime,
+        sample_time: Optional[timedelta],
         read_type: ReaderType,
-        metadata: Optional[Dict[str, str]] = None,
+        metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         if read_type in [
             ReaderType.COUNT,
             ReaderType.GOOD,
             ReaderType.BAD,
             ReaderType.TOTAL,
             ReaderType.SUM,
             ReaderType.SHAPEPRESERVING,
         ]:
             raise NotImplementedError
 
         if read_type == ReaderType.SNAPSHOT and stop_time is not None:
-            raise NotImplementedError(
-                "Timestamp not supported for PI ODBC connection using 'SNAPSHOT'."
+            stop_time = None
+            logger.warning(
+                "End time is not supported for PI ODBC connection using 'SNAPSHOT'."
                 "Try the web API 'piwebapi' instead."
             )
 
         seconds = 0
         if read_type != ReaderType.SNAPSHOT:
-            start_time = start_time.tz_convert("UTC")
-            stop_time = stop_time.tz_convert("UTC")
+            start_time = start_time.astimezone(pytz.UTC)
+            if stop_time:
+                stop_time = stop_time.astimezone(pytz.UTC)
             seconds = int(sample_time.total_seconds())
             if ReaderType.SAMPLED == read_type:
                 seconds = 0
             else:
                 if seconds <= 0:
                     pass  # Fixme: Not implemented
                     # sample_time = (stop_time-start_time).totalseconds
@@ -557,17 +565,15 @@
 
     def connect(self):
         connection_string = self.generate_connection_string()
         # The default autocommit=False is not supported by PI odbc driver.
         self.conn = pyodbc.connect(connection_string, autocommit=True)
         self.cursor = self.conn.cursor()
 
-    def search(
-        self, tag: Optional[str] = None, desc: Optional[str] = None
-    ) -> List[Tuple[str, str]]:
+    def search(self, tag: Optional[str], desc: Optional[str]) -> List[Tuple[str, str]]:
         query = self.generate_search_query(tag=tag, desc=desc)
         self.cursor.execute(query)
         return self.cursor.fetchall()
 
     def _get_tag_metadata(self, tag: str) -> Optional[Dict[str, str]]:
         # Returns None if tag not found.
         query = f"SELECT digitalset, engunits, descriptor FROM pipoint.pipoint2 WHERE tag='{tag}'"
@@ -605,19 +611,19 @@
         ]:
             return True
         return False
 
     def read_tag(
         self,
         tag: str,
-        start_time: pd.Timestamp,
-        stop_time: pd.Timestamp,
-        sample_time: Optional[Union[int, pd.Timestamp]],
+        start_time: datetime,
+        stop_time: datetime,
+        sample_time: Optional[timedelta],
         read_type: ReaderType,
-        metadata: Optional[Dict[str, str]] = None,
+        metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         if metadata is None:
             # Tag not found
             # TODO: Handle better and similarly across all handlers.
             return pd.DataFrame()
```

### Comparing `tagreader-4.0.3/tagreader/utils.py` & `tagreader-4.1.1/tagreader/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import enum
 import logging
 import platform
 import warnings
 from datetime import datetime
+from enum import Enum
 from typing import Union
 
 import pandas as pd
 import pytz
 
 
 def is_windows() -> bool:
@@ -61,26 +62,34 @@
                 if str(key_name).lower() == search_key_name:
                     break
         except Exception as err:
             logging.error("{}: {}".format(i, err))
     return key, key_string
 
 
-def ensure_datetime_with_tz(
-    date_stamp: Union[datetime, str, pd.Timestamp],
-    tz: str = "Europe/Oslo",
-) -> pd.Timestamp:
-    if isinstance(date_stamp, str):
+def convert_to_pydatetime(date_stamp: Union[datetime, str, pd.Timestamp]) -> datetime:
+    if isinstance(date_stamp, datetime):
+        return date_stamp
+    elif isinstance(date_stamp, pd.Timestamp):
+        return date_stamp.to_pydatetime()
+    else:
         try:
-            date_stamp = pd.to_datetime(date_stamp, format="ISO8601")
+            return pd.to_datetime(str(date_stamp), format="ISO8601").to_pydatetime()
         except ValueError:
-            date_stamp = pd.to_datetime(date_stamp, dayfirst=True)
+            return pd.to_datetime(str(date_stamp), dayfirst=True).to_pydatetime()
+
+
+def ensure_datetime_with_tz(
+    date_stamp: Union[datetime, str, pd.Timestamp],
+    tz: pytz.timezone = pytz.timezone("Europe/Oslo"),
+) -> datetime:
+    date_stamp = convert_to_pydatetime(date_stamp)
 
     if not date_stamp.tzinfo:
-        date_stamp = pytz.timezone(tz).localize(date_stamp)
+        date_stamp = tz.localize(date_stamp)
 
     return date_stamp
 
 
 def urljoin(*args) -> str:
     """Joins components of URL. Ensures slashes are inserted or removed where
     needed, and does not strip trailing slash of last element.
@@ -244,7 +253,15 @@
             if "statoil.no" in f.read():
                 return True
     else:
         raise OSError(
             f"Unsupported system: {platform.system()}. Please report this as an issue."
         )
     return False
+
+
+class IMSType(str, Enum):
+    PIWEBAPI = "piwebapi"
+    ASPENONE = "aspenone"
+    PI = "pi"
+    ASPEN = "aspen"
+    IP21 = "ip21"
```

### Comparing `tagreader-4.0.3/tagreader/web_handlers.py` & `tagreader-4.1.1/tagreader/web_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import datetime
 import re
 import urllib.parse
-import warnings
 from abc import ABC, abstractmethod
+from datetime import datetime, timedelta
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pytz
 import requests
 import urllib3
 from requests import Response
 from requests_kerberos import OPTIONAL, HTTPKerberosAuth
 
+from tagreader.cache import BaseCache
+from tagreader.logger import logger
 from tagreader.utils import ReaderType, is_mac, is_windows, urljoin
 
 # Requests will use simplejson if it has been installed, so handle both errors here
 try:
     from simplejson.errors import JSONDecodeError
 except ImportError:
     from json.decoder import JSONDecodeError
@@ -42,17 +44,17 @@
 
 def get_url_aspen() -> str:
     # internal url (redirects to dll)
     return r"https://aspenone.api.equinor.com"
 
 
 def list_aspenone_sources(
-    url: Optional[str] = None,
-    auth: Optional[Any] = None,
-    verifySSL: Optional[bool] = None,
+    url: Optional[str],
+    auth: Optional[Any],
+    verifySSL: Optional[bool],
 ) -> List[str]:
     if url is None:
         url = get_url_aspen()
 
     if auth is None:
         auth = get_auth_aspen()
 
@@ -75,17 +77,17 @@
         print("Not found")
     elif res.status_code == 401:
         print("Not authorized")
     res.raise_for_status()
 
 
 def list_piwebapi_sources(
-    url: Optional[str] = None,
-    auth: Optional[Any] = None,
-    verifySSL: Optional[bool] = None,
+    url: Optional[str],
+    auth: Optional[Any],
+    verifySSL: Optional[bool],
 ) -> List[str]:
     if url is None:
         url = get_url_pi()
 
     if auth is None:
         auth = get_auth_pi()
 
@@ -109,33 +111,34 @@
         print("Not authorized")
     res.raise_for_status()
 
 
 class BaseHandlerWeb(ABC):
     def __init__(
         self,
-        datasource: Optional[str] = None,
-        url: Optional[str] = None,
-        auth: Optional[Any] = None,
-        verifySSL: Optional[bool] = None,
+        datasource: Optional[str],
+        url: Optional[str],
+        auth: Optional[Any],
+        verifySSL: Optional[bool],
     ):
         self.datasource = datasource
         self.base_url = url
         self.session = requests.Session()
         self.session.auth = auth if auth is not None else get_auth_aspen()
         if verifySSL is False:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         self.session.verify = verifySSL if verifySSL is not None else get_verifySSL()
 
-    def fetch(self, url, params=None) -> Response:
+    def fetch(
+        self, url, params: Optional[Union[str, Dict[str, str]]] = None
+    ) -> Response:
         if not self.session.verify:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
         res = self.session.get(url, params=params)
-        res.raise_for_status()
         return res
 
     def connect(self):
         try:
             self.verify_connection(self.datasource)
         except requests.ConnectionError:
             raise ConnectionError(
@@ -146,19 +149,19 @@
     def verify_connection(self, datasource: str):
         ...
 
 
 class AspenHandlerWeb(BaseHandlerWeb):
     def __init__(
         self,
-        datasource: Optional[str] = None,
-        url: Optional[str] = None,
-        auth: Optional[Any] = None,
-        verifySSL: Optional[bool] = None,
-        options: Dict[str, Any] = {},
+        datasource: Optional[str],
+        url: Optional[str],
+        auth: Optional[Any],
+        verifySSL: Optional[bool],
+        options: Dict[str, Any],
     ):
         if url is None:
             url = get_url_aspen()
         if auth is None:
             auth = get_auth_aspen()
         super().__init__(
             datasource=datasource,
@@ -171,34 +174,34 @@
 
     @staticmethod
     def generate_connection_string(host, *_, **__):
         raise NotImplementedError
 
     @staticmethod
     def generate_search_query(
-        tag: Optional[str] = None,
-        desc: Optional[str] = None,
-        datasource: Optional[str] = None,
+        tag: Optional[str],
+        desc: Optional[str],
+        datasource: Optional[str],
     ) -> Dict[str, Any]:
         if not datasource:
             raise ValueError("Data source is required argument")
         # Aspen Web API expects single space instead of consecutive spaces.
         tag = " ".join(tag.split())
         params = {"datasource": datasource, "tag": tag, "max": 100, "getTrendable": 0}
         return params
 
     def generate_read_query(
         self,
         tagname: str,
         mapname: Optional[str],
-        start_time: pd.Timestamp,
-        stop_time: pd.Timestamp,
-        sample_time: Optional[Union[int, pd.Timestamp]],
+        start_time: datetime,
+        stop_time: datetime,
+        sample_time: Optional[timedelta],
         read_type: ReaderType,
-        metadata: Optional[Any] = None,
+        metadata: Any,
     ):
         # Maxpoints is used for Actual (raw) and Bestfit (shapepreserving).
         # Probably need to handle this in another way at some point
         maxpoints = self._max_rows
         stepped = 0
         outsiders = 0
 
@@ -256,15 +259,15 @@
             query += f"<S>{stepped}</S>"
         if read_type not in [
             ReaderType.RAW,
             ReaderType.SHAPEPRESERVING,
             ReaderType.SNAPSHOT,
         ]:
             query += (
-                f"<P>{int(sample_time.total_seconds())}</P>"
+                f"<P>{int(sample_time.total_seconds()) if sample_time else 0}</P>"
                 "<PU>3</PU>"  # Period Unit: 0=day, 1=hour, 2=min, 3=sec
             )
         if read_type not in [
             ReaderType.RAW,
             ReaderType.SHAPEPRESERVING,
             ReaderType.INT,
             ReaderType.SNAPSHOT,
@@ -298,15 +301,15 @@
         j = r.json()
         for item in j["data"]:
             if item["n"] == datasource:
                 return True
         return False
 
     @staticmethod
-    def split_tagmap(tagmap):
+    def split_tagmap(tagmap) -> Tuple[Optional[str], ...]:
         return tuple(tagmap.split(";") if ";" in tagmap else (tagmap, None))
 
     def generate_get_unit_query(self, tag: str):
         tagname, _ = self.split_tagmap(tag)
         parts = [
             '<Q allQuotes="1" attributeData="1">',
             "<Tag>",
@@ -355,17 +358,15 @@
     def _get_default_mapname(self, tagname: str):
         (tagname, _) = self.split_tagmap(tagname)
         allmaps = self._get_maps(tagname)
         for k, v in allmaps.items():
             if v:
                 return k
 
-    def search(
-        self, tag: Optional[str] = None, desc: Optional[str] = None
-    ) -> List[Tuple[str, str]]:
+    def search(self, tag: Optional[str], desc: Optional[str]) -> List[Tuple[str, str]]:
         if tag is None:
             raise ValueError("Tag is a required argument")
 
         tag = tag.replace("%", "*") if isinstance(tag, str) else None
         # Prepare for regex
         desc = desc.replace("%", "*") if isinstance(desc, str) else None
         desc = desc.replace("*", ".*") if isinstance(desc, str) else None
@@ -449,19 +450,19 @@
         except Exception:
             desc = ""
         return desc
 
     def read_tag(
         self,
         tag: str,
-        start_time: Optional[pd.Timestamp],
-        stop_time: Optional[pd.Timestamp],
-        sample_time: Optional[Union[int, pd.Timestamp]],
+        start_time: Optional[datetime],
+        stop_time: Optional[datetime],
+        sample_time: Optional[timedelta],
         read_type: ReaderType,
-        metadata: Optional[Dict[str, str]] = None,
+        metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         if read_type not in [
             ReaderType.INT,
             ReaderType.MIN,
             ReaderType.MAX,
             ReaderType.RNG,
@@ -513,15 +514,15 @@
             # pre-process
             import json
 
             txt = res.text.replace('"v":nan', '"v":NaN').replace('"v":-nan', '"v":NaN')
             j = json.loads(txt)
 
         if "er" in j["data"][0]["samples"][0]:
-            warnings.warn(j["data"][0]["samples"][0]["es"])
+            logger.warning(j["data"][0]["samples"][0]["es"])
             return pd.DataFrame(columns=[tag])
         if get_status:
             # The "l" field maps 1:1 to ODBC status field values 0, 1, 2, 4, 5, 6
             df = (
                 pd.DataFrame.from_dict(j["data"][0]["samples"])
                 .drop(labels=["s", "V"], axis="columns")
                 .rename(columns={"t": "Timestamp", "v": "Value", "l": "Status"})
@@ -539,15 +540,18 @@
         df["Timestamp"] = pd.to_datetime(df["Timestamp"], unit="ms", origin="unix")
         df = df.set_index("Timestamp", drop=True).tz_localize("UTC")
         df.index.name = "time"
         return df.rename(columns={"Value": tag, "Status": tag + "::status"})
 
     @staticmethod
     def generate_sql_query(
-        connection_string=None, datasource=None, query=None, max_rows=100000
+        connection_string: Optional[str],
+        datasource: Optional[str],
+        query: Optional[str],
+        max_rows: int = 100000,
     ):
         if connection_string is not None:
             connstr = f'<SQL c="{connection_string}" m="{max_rows}" to="30" s="1">'
         else:
             connstr = (
                 f'<SQL t="SQLplus" ds="{datasource}" '
                 'dso="CHARINT=N;CHARFLOAT=N;CHARTIME=N;CONVERTERRORS=N" '
@@ -572,60 +576,61 @@
                 "CHARTIME=N;CONVERTERRORS=N"
             )
 
     def query_sql(self, query: str, parse: bool = True) -> Union[str, pd.DataFrame]:
         url = urljoin(self.base_url, "SQL")
         if self._connection_string is None:
             params = self.generate_sql_query(
-                datasource=self.datasource, query=query, max_rows=self._max_rows
+                datasource=self.datasource,
+                query=query,
+                max_rows=self._max_rows,
+                connection_string=None,
             )
         else:
             params = self.generate_sql_query(
                 connection_string=self._connection_string,
                 query=query,
                 max_rows=self._max_rows,
+                datasource=None,
             )
         res = self.fetch(url, params=params)
         # For now just return result as text regardless of value of parse
         if parse:
             raise NotImplementedError(
                 "Use parse=False to receive and handle text result instead"
             )
         return res.text
 
 
 class PIHandlerWeb(BaseHandlerWeb):
     def __init__(
         self,
-        url: Optional[str] = None,
-        datasource: Optional[str] = None,
-        auth: Optional[Any] = None,
-        verifySSL: Optional[bool] = None,
-        options: Dict[str, Union[int, float, str]] = {},
+        url: Optional[str],
+        datasource: Optional[str],
+        auth: Optional[Any],
+        verifySSL: bool,
+        options: Dict[str, Union[int, float, str]],
     ):
+        self._max_rows = options.get("max_rows", 10000)
         if url is None:
             url = get_url_pi()
         if auth is None:
             auth = get_auth_pi()
         super().__init__(
             url=url,
             datasource=datasource,
             auth=auth,
             verifySSL=verifySSL,
         )
         self._max_rows = options.get("max_rows", 10000)
-        self.webidcache = {}
+        self.webidcache = BaseCache(directory=Path(".") / ".cache" / datasource)
 
     @staticmethod
-    def _time_to_UTC_string(time: pd.Timestamp) -> str:
-        timecast_format_query = "%d-%b-%y %H:%M:%S"
-        if isinstance(time, datetime.datetime):
-            return time.astimezone(pytz.UTC).strftime(timecast_format_query)
-        else:
-            return time.tz_convert("UTC").strftime(timecast_format_query)
+    def _time_to_UTC_string(time: datetime) -> str:
+        return time.astimezone(pytz.UTC).strftime("%d-%b-%y %H:%M:%S")
 
     @staticmethod
     def generate_connection_string(host, *_, **__):
         raise NotImplementedError
 
     @staticmethod
     def escape(s: str) -> str:
@@ -653,17 +658,17 @@
                     " ": r"\ ",
                 }
             )
         )
 
     @staticmethod
     def generate_search_query(
-        tag: Optional[str] = None,
-        desc: Optional[str] = None,
-        datasource: Optional[str] = None,
+        tag: Optional[str],
+        desc: Optional[str],
+        datasource: Optional[str],
     ) -> Dict[str, str]:
         q = []
         if tag is not None:
             q.extend([f"name:{PIHandlerWeb.escape(tag)}"])
         if desc is not None:
             q.extend([f"description:{PIHandlerWeb.escape(desc)}"])
         query = " AND ".join(q)
@@ -673,19 +678,19 @@
             params["scope"] = f"pi:{datasource}"
 
         return params
 
     def generate_read_query(
         self,
         tag: str,
-        start_time: pd.Timestamp,
-        stop_time: pd.Timestamp,
-        sample_time: Optional[Union[int, pd.Timestamp]],
+        start_time: datetime,
+        stop_time: datetime,
+        sample_time: timedelta,
         read_type: ReaderType,
-        metadata: Optional[Dict[str, str]] = None,
+        metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ) -> Tuple[str, Dict[str, str]]:
         if read_type in [
             ReaderType.COUNT,
             ReaderType.GOOD,
             ReaderType.BAD,
             ReaderType.TOTAL,
@@ -847,15 +852,15 @@
                 first = j["Items"][0]
                 for item in j["Items"][1:]:
                     if item != first:
                         raise AssertionError(
                             f"Received {len(j['Items'])} results when trying to find unique WebId for {tag}."
                         )
             elif len(j["Items"]) == 0:
-                warnings.warn(f"Tag {tag} not found")
+                logger.warning(f"Tag {tag} not found")
                 return None
 
             webid = j["Items"][0]["WebId"]
             self.webidcache[tag] = webid
         return self.webidcache[tag]
 
     @staticmethod
@@ -870,19 +875,19 @@
         ]:
             return True
         return False
 
     def read_tag(
         self,
         tag: str,
-        start_time: Optional[pd.Timestamp] = None,
-        stop_time: Optional[pd.Timestamp] = None,
-        sample_time: Optional[Union[int, pd.Timestamp]] = None,
-        read_type: ReaderType = ReaderType.INTERPOLATED,
-        metadata: Optional[Dict[str, str]] = None,
+        start_time: Optional[datetime],
+        stop_time: Optional[datetime],
+        sample_time: timedelta,
+        read_type: ReaderType,
+        metadata: Optional[Dict[str, str]],
         get_status: bool = False,
     ):
         webid = self.tag_to_webid(tag)
         if not webid:
             return pd.DataFrame()
 
         (url, params) = self.generate_read_query(
```

### Comparing `tagreader-4.0.3/PKG-INFO` & `tagreader-4.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: tagreader
-Version: 4.0.3
+Version: 4.1.1
 Summary: Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems.
+Home-page: https://github.com/equinor/tagreader-python
 License: MIT
 Keywords: Aspen InfoPlus.21,OSIsoft PI
 Author: Einar S. Idsø
 Author-email: eiids@equinor.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -25,21 +26,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: notebooks
 Requires-Dist: certifi (>=2023,<2024)
+Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: jupyter (>=1,<2) ; extra == "notebooks"
 Requires-Dist: matplotlib (>=3,<4) ; extra == "notebooks"
 Requires-Dist: pandas (>=1)
 Requires-Dist: pyodbc (>=4,<5)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: requests-kerberos (>=0,<1)
-Requires-Dist: tables (>=3,<4) ; platform_machine != "arm64"
+Project-URL: Repository, https://github.com/equinor/tagreader-python
 Description-Content-Type: text/markdown
 
 # tagreader-python <!-- omit in toc -->
 
 ![GitHub Build Status](https://github.com/equinor/tagreader-python/workflows/Test/badge.svg)
 [![Devops Build Status](https://dev.azure.com/EIIDS/tagreader/_apis/build/status/equinor.tagreader-python?branchName=master)](https://dev.azure.com/EIIDS/tagreader/_build/latest?definitionId=5&branchName=master)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tagreader) 
@@ -61,24 +63,20 @@
 to cache results.
 
 ## Requirements
 
 Python >=3.8 with the following packages:
 
   + pandas >= 1.0.0
-  + tables (*)
   + requests
   + requests-kerberos
   + certifi >= 2023.5.7
+  + diskcache
   + pyodbc (**)
 
-*) If tables is not installed, caching of fetched data will be disabled.
-Tables will be installed alongside Tagreader unless the installation is
-known to fail, which is the case for Macs with ARM CPU.
-
 **) If using ODBC connections, you must also install proprietary drivers for
 PI ODBC and/or Aspen IP.21 SQLPlus. These drivers are only available for
 Microsoft Windows. Pyodbc will therefore not be installed for non-Windows
 systems.
 
 ## Installation
```

