# Comparing `tmp/humanity_etl-0.0.1rc6.tar.gz` & `tmp/humanity_etl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanity_etl-0.0.1rc6.tar", last modified: Tue Jun 13 15:40:06 2023, max compression
+gzip compressed data, was "humanity_etl-0.1.0.tar", last modified: Wed Jun 14 17:29:39 2023, max compression
```

## Comparing `humanity_etl-0.0.1rc6.tar` & `humanity_etl-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.0.1rc6/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      984 2023-06-08 17:49:58.000000 humanity_etl-0.0.1rc6/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.839053 humanity_etl-0.0.1rc6/humanity_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 humanity_etl-0.0.1rc6/humanity_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-08 17:37:37.000000 humanity_etl-0.0.1rc6/humanity_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      328 2023-06-08 17:11:05.000000 humanity_etl-0.0.1rc6/humanity_etl/humanity_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/humanity_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4841 2023-06-12 19:40:35.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      547 2023-06-12 20:29:22.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5966 2023-06-08 18:01:30.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/humanity_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.0.1rc6/humanity_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4489 2023-06-13 15:39:00.000000 humanity_etl-0.0.1rc6/humanity_etl/tables/timeclocks.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.839053 humanity_etl-0.0.1rc6/humanity_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      520 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      990 2023-06-13 15:39:38.000000 humanity_etl-0.0.1rc6/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.0.1rc6/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.1.0/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1743 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1235 2023-06-14 17:17:02.000000 humanity_etl-0.1.0/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/humanity_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       22 2023-06-14 17:28:48.000000 humanity_etl-0.1.0/humanity_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      155 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      329 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/humanity_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/humanity_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.1.0/humanity_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4840 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      548 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5986 2023-06-14 17:19:56.000000 humanity_etl-0.1.0/humanity_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/humanity_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.1.0/humanity_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4572 2023-06-14 17:18:21.000000 humanity_etl-0.1.0/humanity_etl/tables/timeclocks.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/humanity_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1743 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      530 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-14 17:29:39.000000 humanity_etl-0.1.0/humanity_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      426 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      987 2023-06-14 17:28:48.000000 humanity_etl-0.1.0/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-14 17:29:39.709748 humanity_etl-0.1.0/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.1.0/tests/__init__.py
```

### Comparing `humanity_etl-0.0.1rc6/PKG-INFO` & `humanity_etl-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity_etl
-Version: 0.0.1rc6
+Version: 0.1.0
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -70,24 +70,50 @@
 
 ### Install Packages
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Test
+### Test
 
 ```bash
 make test
 ```
 
-## Format
+### Format
 
 ```bash
 make format
 ```
 
 ```bash
 make lint
 ```
 
+### Version & Release
+
+```bash
+bump2version <major/minor/patch>
+```
+
+```bash
+make release
+```
+
+**note** Don't forget to `git push` with `--tags`
+
+### pre-commit
+
+#### Setup
+
+```bash
+pre-commit install
+```
+
+#### Run all
+
+```bash
+make pre-commit
+```
+
```

### Comparing `humanity_etl-0.0.1rc6/README_PUBLIC.md` & `humanity_etl-0.1.0/README_PUBLIC.md`

 * *Files 25% similar despite different names*

```diff
@@ -54,22 +54,48 @@
 
 ### Install Packages
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Test
+### Test
 
 ```bash
 make test
 ```
 
-## Format
+### Format
 
 ```bash
 make format
 ```
 
 ```bash
 make lint
 ```
+
+### Version & Release
+
+```bash
+bump2version <major/minor/patch>
+```
+
+```bash
+make release
+```
+
+**note** Don't forget to `git push` with `--tags`
+
+### pre-commit
+
+#### Setup
+
+```bash
+pre-commit install
+```
+
+#### Run all
+
+```bash
+make pre-commit
+```
```

### Comparing `humanity_etl-0.0.1rc6/humanity_etl/libs/cnst.py` & `humanity_etl-0.1.0/humanity_etl/libs/cnst.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,9 +103,8 @@
     ),
     "mtl_timeclocks": "https://www.humanity.com/api/v2/timeclocks?access_token={}".format(
         os.environ.get("MTL_ACCESS_TOKEN")
     ),
     "mtl_shifts": "https://www.humanity.com/api/v2/shifts?access_token={}".format(
         os.environ.get("MTL_ACCESS_TOKEN")
     ),
-
 }
```

### Comparing `humanity_etl-0.0.1rc6/humanity_etl/libs/dbg.py` & `humanity_etl-0.1.0/humanity_etl/libs/dbg.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """dbg"""
 
 import os
 from typing import Any, Callable, TypeVar
 
-from loguru import logger
 import pandas as pd
+from loguru import logger
 
 T = TypeVar("T")
 
 
 def dbg(__message: str, *args: Any, **kwargs: Any) -> None:
     """dbg"""
     if os.environ.get("APP_ENV") == "development":
```

### Comparing `humanity_etl-0.0.1rc6/humanity_etl/libs/network.py` & `humanity_etl-0.1.0/humanity_etl/libs/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """network"""
 
 import json
-from typing import Dict, Any
+from typing import Any, Dict
+
 import requests
 
 from humanity_etl.libs.dbg import dbg
 
 
 def get_data(api_url: str, headers: Dict[str, str]) -> Dict[str, Any]:
     """Make a GET request to the Humanity API and return the data."""
```

### Comparing `humanity_etl-0.0.1rc6/humanity_etl/libs/transform.py` & `humanity_etl-0.1.0/humanity_etl/libs/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """transform"""
 
-from typing import Dict, Any
+from typing import Any, Dict
 
 import pandas as pd
 from pandas import DataFrame as PandasDF
 
 from humanity_etl.libs.network import get_data
 
 
@@ -92,15 +92,15 @@
     return change
 
 
 def merge_related_dfs(df_dict: Dict[str, PandasDF]) -> Dict[str, PandasDF]:
     """
     Union the employees and disabled employess associated dataframes
     """
-    merged_dfs = {}
+    merged_dfs: Dict[str,PandasDF] = {}
     for key, df in df_dict.items():
         if key.endswith("_employees") or key.endswith("_employees_disabled"):
             # Get the prefix of the key
             prefix = (
                 key.rsplit("_", 1)[0]
                 if key.endswith("_employees")
                 else key.rsplit("_", 2)[0]
```

### Comparing `humanity_etl-0.0.1rc6/humanity_etl/tables/timeclocks.py` & `humanity_etl-0.1.0/humanity_etl/tables/timeclocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """list"""
 
-from pandas import DataFrame as PandasDF
 import pandas as pd
+from pandas import DataFrame as PandasDF
 
+from humanity_etl.libs.cnst import urls
+from humanity_etl.libs.dbg import print_dataframe_head, write_dataframe_to_csv
 from humanity_etl.libs.transform import (
     framer,
     get_data_for_all_urls,
     map_data_to_dataframe,
     merge_related_dfs,
     merger,
 )
-from humanity_etl.libs.dbg import print_dataframe_head, write_dataframe_to_csv
-from humanity_etl.libs.cnst import urls
 
 
 @write_dataframe_to_csv("timeclocks")
 @print_dataframe_head
 def timeclocks() -> PandasDF:
     """timeclocks dataframe"""
 
@@ -108,15 +108,22 @@
     )
     mtl_program_df = merger(
         mtl_timeclocks_df, mtl_positions_df, mtl_employees_df, mtl_shifts_df, "MTL"
     )
 
     # "UNION" all region dataframes
     humanity_df = pd.concat(
-        [gta_program_df, cgy_program_df, wpg_program_df, edm_program_df, ott_program_df, mtl_program_df]
+        [
+            gta_program_df,
+            cgy_program_df,
+            wpg_program_df,
+            edm_program_df,
+            ott_program_df,
+            mtl_program_df,
+        ]
     )
     humanity_final_df = humanity_df.merge(
         parent_employees_df2, left_on="employee_name", right_on="name", how="left"
     )
 
     # "Coalesce" emails to fill in blanks
     humanity_final_df["employee_email"] = humanity_final_df.email.combine_first(
```

### Comparing `humanity_etl-0.0.1rc6/humanity_etl.egg-info/PKG-INFO` & `humanity_etl-0.1.0/humanity_etl.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity-etl
-Version: 0.0.1rc6
+Version: 0.1.0
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -70,24 +70,50 @@
 
 ### Install Packages
 
 ```bash
 pip install -r requirements.txt
 ```
 
-## Test
+### Test
 
 ```bash
 make test
 ```
 
-## Format
+### Format
 
 ```bash
 make format
 ```
 
 ```bash
 make lint
 ```
 
+### Version & Release
+
+```bash
+bump2version <major/minor/patch>
+```
+
+```bash
+make release
+```
+
+**note** Don't forget to `git push` with `--tags`
+
+### pre-commit
+
+#### Setup
+
+```bash
+pre-commit install
+```
+
+#### Run all
+
+```bash
+make pre-commit
+```
+
```

### Comparing `humanity_etl-0.0.1rc6/humanity_etl.egg-info/SOURCES.txt` & `humanity_etl-0.1.0/humanity_etl.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README_PUBLIC.md
+setup.cfg
 setup.py
 humanity_etl/__init__.py
 humanity_etl/__main__.py
 humanity_etl/humanity_etl.py
 humanity_etl.egg-info/PKG-INFO
 humanity_etl.egg-info/SOURCES.txt
 humanity_etl.egg-info/dependency_links.txt
```

### Comparing `humanity_etl-0.0.1rc6/setup.py` & `humanity_etl-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="humanity_etl",
-    version="0.0.1rc6",
+    version="0.1.0",
     description="Replicate humanity data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
```

