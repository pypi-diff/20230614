# Comparing `tmp/smunger-0.0.8.tar.gz` & `tmp/smunger-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smunger-0.0.8.tar", max compression
+gzip compressed data, was "smunger-0.0.9.tar", max compression
```

## Comparing `smunger-0.0.8.tar` & `smunger-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-02-24 03:29:10.392751 smunger-0.0.8/LICENSE
--rw-r--r--   0        0        0     2863 2023-02-24 03:29:10.392751 smunger-0.0.8/README.md
--rw-r--r--   0        0        0     2977 2023-02-24 03:29:10.396751 smunger-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      857 2023-02-24 03:29:10.396751 smunger-0.0.8/smunger/__init__.py
--rw-r--r--   0        0        0     1723 2023-02-24 03:29:10.396751 smunger-0.0.8/smunger/annotate.py
--rw-r--r--   0        0        0     5606 2023-02-24 03:29:10.396751 smunger-0.0.8/smunger/cli.py
--rw-r--r--   0        0        0       83 2023-02-24 03:29:10.396751 smunger-0.0.8/smunger/console.py
--rw-r--r--   0        0        0     6220 2023-02-24 03:29:10.396751 smunger-0.0.8/smunger/constant.py
--rw-r--r--   0        0        0     3317 2023-02-24 03:29:10.396751 smunger-0.0.8/smunger/io.py
--rw-r--r--   0        0        0     3665 2023-02-24 03:29:10.396751 smunger-0.0.8/smunger/liftover.py
--rw-r--r--   0        0        0     4784 2023-02-24 03:29:10.396751 smunger-0.0.8/smunger/mapheader.py
--rw-r--r--   0        0        0    10463 2023-02-24 03:29:10.396751 smunger-0.0.8/smunger/smunger.py
--rw-r--r--   0        0        0       37 2023-02-24 03:29:10.396751 smunger-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     1456 2023-02-24 03:29:10.396751 smunger-0.0.8/tests/annota_rsid_test.py
--rw-r--r--   0        0        0      269 2023-02-24 03:29:10.396751 smunger-0.0.8/tests/exampledata/catalog.header.json
--rw-r--r--   0        0        0   115228 2023-02-24 03:29:10.396751 smunger-0.0.8/tests/exampledata/catalog.munged.hg38.txt.gz
--rw-r--r--   0        0        0   502403 2023-02-24 03:29:10.400751 smunger-0.0.8/tests/exampledata/catalog.munged.rsid.txt
--rw-r--r--   0        0        0   120144 2023-02-24 03:29:10.400751 smunger-0.0.8/tests/exampledata/catalog.munged.txt.gz
--rw-r--r--   0        0        0     1931 2023-02-24 03:29:10.400751 smunger-0.0.8/tests/exampledata/catalog.munged.txt.gz.tbi
--rw-r--r--   0        0        0   124530 2023-02-24 03:29:10.400751 smunger-0.0.8/tests/exampledata/catalog.txt.gz
--rw-r--r--   0        0        0       72 2023-02-24 03:29:10.400751 smunger-0.0.8/tests/exampledata/test.header.json
--rw-r--r--   0        0        0    41670 2023-02-24 03:29:10.400751 smunger-0.0.8/tests/exampledata/test.munged.txt.gz
--rw-r--r--   0        0        0      738 2023-02-24 03:29:10.400751 smunger-0.0.8/tests/exampledata/test.munged.txt.gz.tbi
--rw-r--r--   0        0        0   789756 2023-02-24 03:29:10.400751 smunger-0.0.8/tests/exampledata/test.txt.gz
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 smunger-0.0.8/setup.py
--rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 smunger-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-28 03:43:21.835687 smunger-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2863 2023-02-28 03:43:21.835687 smunger-0.0.9/README.md
+-rw-r--r--   0        0        0     2977 2023-02-28 03:43:21.835687 smunger-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      857 2023-02-28 03:43:21.835687 smunger-0.0.9/smunger/__init__.py
+-rw-r--r--   0        0        0     1723 2023-02-28 03:43:21.835687 smunger-0.0.9/smunger/annotate.py
+-rw-r--r--   0        0        0     5600 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/cli.py
+-rw-r--r--   0        0        0       83 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/console.py
+-rw-r--r--   0        0        0     6398 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/constant.py
+-rw-r--r--   0        0        0     3854 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/io.py
+-rw-r--r--   0        0        0     3665 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/liftover.py
+-rw-r--r--   0        0        0     5575 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/mapheader.py
+-rw-r--r--   0        0        0    11314 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/smunger.py
+-rw-r--r--   0        0        0       37 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1456 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/annota_rsid_test.py
+-rw-r--r--   0        0        0      269 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/exampledata/catalog.header.json
+-rw-r--r--   0        0        0   115228 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/exampledata/catalog.munged.hg38.txt.gz
+-rw-r--r--   0        0        0   502403 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/exampledata/catalog.munged.rsid.txt
+-rw-r--r--   0        0        0   120144 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/catalog.munged.txt.gz
+-rw-r--r--   0        0        0     1931 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/catalog.munged.txt.gz.tbi
+-rw-r--r--   0        0        0   124530 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/catalog.txt.gz
+-rw-r--r--   0        0        0       72 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/test.header.json
+-rw-r--r--   0        0        0    41670 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/test.munged.txt.gz
+-rw-r--r--   0        0        0      738 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/test.munged.txt.gz.tbi
+-rw-r--r--   0        0        0   789756 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/test.txt.gz
+-rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 smunger-0.0.9/PKG-INFO
```

### Comparing `smunger-0.0.8/LICENSE` & `smunger-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/README.md` & `smunger-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/pyproject.toml` & `smunger-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "smunger"
-version = "0.0.8"
+version = "0.0.9"
 homepage = "https://github.com/jianhua/smunger"
 description = "munger for GWAS summary statistics."
 authors = ["Jianhua Wang <jianhua.mert@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `smunger-0.0.8/smunger/__init__.py` & `smunger-0.0.9/smunger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     munge_z,
 )
 from .liftover import liftover, liftover_file
 from .annotate import annotate_rsid
 
 __author__ = """Jianhua Wang"""
 __email__ = 'jianhua.mert@gmail.com'
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 # Set up logging
 logging.basicConfig(
     level=logging.NOTSET,
     format="%(name)s - %(message)s",
     datefmt="[%X]",
     handlers=[RichHandler(rich_tracebacks=True, show_path=False)],
```

### Comparing `smunger-0.0.8/smunger/annotate.py` & `smunger-0.0.9/smunger/annotate.py`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/smunger/cli.py` & `smunger-0.0.9/smunger/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     after_nrow = len(df)
     save_sumstats(df, outfile, build_index=build_index)
     from smunger.smunger import get_sigdf
 
     df_sig = get_sigdf(df, pval=sigsnps_pval)
     if sigsnps:
         if len(df_sig) > 0:
-            save_sumstats(df_sig, sigsnps, build_index=build_index)
+            save_sumstats(df_sig, sigsnps, build_index=False)
         else:
             console.print('[bold red]No significant SNPs found.[/bold red]')
     non_null_cols = df.columns[df.notnull().any()].tolist()
     report_json = {
         'in_rows': pre_nrow,
         'out_rows': after_nrow,
         'sigsnps': len(df_sig),
```

### Comparing `smunger-0.0.8/smunger/constant.py` & `smunger-0.0.9/smunger/constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     CHR = "CHR"
     BP = "BP"
     RSID = "rsID"
     SNPID = 'SNPID'  # unique snpid, chr-bp-sorted(EA,NEA)
     EA = "EA"
     NEA = "NEA"
     P = "P"
+    NEGLOGP = "-log10P"
     BETA = "BETA"
     OR = "OR"
     ORSE = "ORSE"
     SE = "SE"
     EAF = "EAF"
     MAF = "MAF"
     N = "N"
@@ -30,14 +31,15 @@
 
     CHR = int
     BP = int
     RSID = str
     EA = str
     NEA = str
     P = float
+    NEGLOGP = float
     BETA = float
     OR = float
     ORSE = float
     SE = float
     EAF = float
     MAF = float
     N = int
@@ -79,14 +81,15 @@
     SE_MAX = np.inf
     EAF_MIN = 0
     EAF_MAX = 1
     MAF_MIN = 0
     MAF_MAX = 1
     ORSE_MIN = 0
     ORSE_MAX = np.inf
+    NEGLOGP_MIN = 0
 
 
 COMMON_COLNAMES = {
     'CHR': 'CHR',
     'chr': 'CHR',
     'chromosome': 'CHR',
     '#CHROM': 'CHR',
@@ -291,8 +294,12 @@
     'NonEffectAllele': 'NEA',
     'Freq.A1.ESP.EUR': 'EAF',
     'base_pair_position': 'BP',
     'effect_allle_frequency': 'EAF',
     'base_pair_locations': 'BP',
     'ZScore': 'Zscore',
     'stderr': 'SE',
+    'pval(-log10)': '-log10P',
+    '-log10P': '-log10P',
+    '-log10p': '-log10P',
+    '-log10Pvalue': '-log10P',
 }
```

### Comparing `smunger-0.0.8/smunger/io.py` & `smunger-0.0.9/smunger/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """Read and write data from/to files."""
 
 import gzip
 import logging
 import shutil
 from pathlib import Path
 from subprocess import PIPE, run
-from typing import Optional
+from typing import Optional, Union
 
 import pandas as pd
 
 from .constant import ColName
 
 logger = logging.getLogger('io')
 
 
 def load_sumstats(
-    filename: Path,
+    filename: Union[str, Path],
     sep: Optional[str] = None,
     nrows: Optional[int] = None,
     skiprows: int = 0,
     comment: Optional[str] = None,
     gzipped: Optional[bool] = None,
 ) -> pd.DataFrame:
     """Load summary statistics from a file."""
     # determine whether the file is gzipped
+    if isinstance(filename, str):
+        filename = Path(filename)
     if gzipped is None:
         gzipped = filename.suffix.endswith('gz')
 
     # read the first line of the file to determine the separator
     if sep is None:
         if gzipped:
             with gzip.open(filename, 'rt') as f:
@@ -68,27 +70,27 @@
     if tool_path:
         return tool_path
     else:
         logger.error(f"{tool} is not installed. Please install it first and make sure it is in your PATH.")
         raise ValueError(f"{tool} is not installed. Please install it first and make sure it is in your PATH.")
 
 
-def save_sumstats(sumstats: pd.DataFrame, filename: Path, build_index: bool = True):
+def save_sumstats(sumstats: pd.DataFrame, filename: Union[str, Path], build_index: bool = True):
     """Save summary statistics to a file."""
     # save the summary statistics to a file
     if isinstance(filename, str):
         filename = Path(filename)
     if filename.exists():
         logger.warning(f'File {filename} already exists. Overwriting.')
 
     if filename.suffix == '.gz':
         filename = filename.with_suffix('')
     sumstats = sumstats.sort_values(by=[ColName.CHR, ColName.BP])
     logger.info(f'Saving summary statistics to {filename}')
-    sumstats.to_csv(filename, sep='\t', index=False, header=True)
+    sumstats.to_csv(filename, sep='\t', index=False, header=True, float_format='%g')
 
     # compress the file
     compress(filename)
     # index the file
     if build_index:
         index(str(filename) + '.gz')
 
@@ -106,7 +108,16 @@
     logger.info(f'Indexing {filename} with tabix')
     run(
         [tabix, '-f', '-S', str(skip), '-s', str(start), '-b', str(end), '-e', str(end), filename],
         stdout=PIPE,
         stderr=PIPE,
         check=True,
     )
+
+
+def export_sumstats(filename: Union[str, Path], chrom: Optional[int] = None,
+                    start: Optional[int] = None, end: Optional[int] = None,
+                    rename_headers: Optional[dict] = None,
+                    out_filename: Optional[Union[str, Path]] = None,
+                    gzipped: bool = True) -> pd.DataFrame:
+    """Export summary statistics to a file."""
+    raise NotImplementedError
```

### Comparing `smunger-0.0.8/smunger/liftover.py` & `smunger-0.0.9/smunger/liftover.py`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/smunger/mapheader.py` & `smunger-0.0.9/smunger/mapheader.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,31 @@
                 else:
                     manual_map = input(f"Please input the correct column number for {col}: ")
                     if manual_map == '':
                         continue
                     else:
                         manual_map = df_cols[int(manual_map)]
                         colname_map[manual_map] = col
+    # use -log10(P) if P is not found
+    if ColName.P not in colname_map.values():
+        console.print("P is not found.")
+        for col in [ColName.NEGLOGP]:
+            if col in guess_orignal_out:
+                map_correct = Confirm.ask(
+                    f"Is {guess_orignal_out[col]} the correct column name for {col}?", default=True
+                )
+                if map_correct:
+                    colname_map[guess_orignal_out[col]] = col
+                else:
+                    manual_map = input(f"Please input the correct column number for {col}: ")
+                    if manual_map == '':
+                        continue
+                    else:
+                        manual_map = df_cols[int(manual_map)]
+                        colname_map[manual_map] = col
     return colname_map
 
 
 def map_colnames(df: pd.DataFrame, outfile: Optional[Path] = None) -> dict:
     """Map column names."""
     guessed_map = guess_colnames(df.columns)
     display_df(df, guessed_map)
```

### Comparing `smunger-0.0.8/smunger/smunger.py` & `smunger-0.0.9/smunger/smunger.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,19 @@
         outdf = munge_chr(outdf)
         outdf = munge_bp(outdf)
         outdf = munge_allele(outdf)
         outdf = make_SNPID_unique(outdf)
         if ColName.P in outdf.columns:
             outdf = munge_pvalue(outdf)
             outdf = outdf.sort_values(by=ColName.P)
+        elif ColName.NEGLOGP in outdf.columns:
+            outdf = munge_neglogp(outdf)
+            outdf[ColName.P] = outdf[ColName.NEGLOGP].apply(lambda x: 10 ** (-x))
+            outdf = outdf.sort_values(by=ColName.P)
+        # TODO: use zscore to calculate pvalue, if pvalue is missing and zscore is present
         else:
             pass
         pre_n = outdf.shape[0]
         outdf = outdf.drop_duplicates(subset=ColName.SNPID, keep="first")
         outdf = outdf.sort_values(by=[ColName.CHR, ColName.BP])
         after_n = outdf.shape[0]
         logger.debug(f"Remove {pre_n - after_n} duplicated SNPs.")
@@ -207,14 +212,27 @@
     outdf = outdf[(outdf[ColName.P] > ColRange.P_MIN) & (outdf[ColName.P] < ColRange.P_MAX)]
     after_n = outdf.shape[0]
     logger.debug(f"Remove {pre_n - after_n} rows because of invalid pvalue.")
     outdf[ColName.P] = outdf[ColName.P].astype(ColType.P)
     return outdf
 
 
+def munge_neglogp(df: pd.DataFrame) -> pd.DataFrame:
+    """Munge neglogp column."""
+    outdf = df.copy()
+    pre_n = outdf.shape[0]
+    outdf[ColName.NEGLOGP] = pd.to_numeric(outdf[ColName.NEGLOGP], errors="coerce")
+    outdf = outdf[outdf[ColName.NEGLOGP].notnull()]
+    outdf = outdf[outdf[ColName.NEGLOGP] > ColRange.NEGLOGP_MIN]
+    after_n = outdf.shape[0]
+    logger.debug(f"Remove {pre_n - after_n} rows because of invalid neglogp.")
+    outdf[ColName.NEGLOGP] = outdf[ColName.NEGLOGP].astype(ColType.NEGLOGP)
+    return outdf
+
+
 def munge_beta(df: pd.DataFrame) -> pd.DataFrame:
     """Munge beta column."""
     pre_n = df.shape[0]
     outdf = df.copy()
     outdf[ColName.BETA] = pd.to_numeric(outdf[ColName.BETA], errors="coerce")
     outdf = outdf[outdf[ColName.BETA].notnull()]
     after_n = outdf.shape[0]
```

### Comparing `smunger-0.0.8/tests/annota_rsid_test.py` & `smunger-0.0.9/tests/annota_rsid_test.py`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/tests/exampledata/catalog.munged.hg38.txt.gz` & `smunger-0.0.9/tests/exampledata/catalog.munged.hg38.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/tests/exampledata/catalog.munged.rsid.txt` & `smunger-0.0.9/tests/exampledata/catalog.munged.rsid.txt`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/tests/exampledata/catalog.munged.txt.gz` & `smunger-0.0.9/tests/exampledata/catalog.munged.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/tests/exampledata/catalog.munged.txt.gz.tbi` & `smunger-0.0.9/tests/exampledata/catalog.munged.txt.gz.tbi`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/tests/exampledata/catalog.txt.gz` & `smunger-0.0.9/tests/exampledata/catalog.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/tests/exampledata/test.munged.txt.gz` & `smunger-0.0.9/tests/exampledata/test.munged.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/tests/exampledata/test.munged.txt.gz.tbi` & `smunger-0.0.9/tests/exampledata/test.munged.txt.gz.tbi`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/tests/exampledata/test.txt.gz` & `smunger-0.0.9/tests/exampledata/test.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.8/PKG-INFO` & `smunger-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smunger
-Version: 0.0.8
+Version: 0.0.9
 Summary: munger for GWAS summary statistics.
 Home-page: https://github.com/jianhua/smunger
 License: MIT
 Author: Jianhua Wang
 Author-email: jianhua.mert@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

