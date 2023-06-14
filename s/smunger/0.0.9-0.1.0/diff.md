# Comparing `tmp/smunger-0.0.9.tar.gz` & `tmp/smunger-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smunger-0.0.9.tar", max compression
+gzip compressed data, was "smunger-0.1.0.tar", max compression
```

## Comparing `smunger-0.0.9.tar` & `smunger-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1070 2023-02-28 03:43:21.835687 smunger-0.0.9/LICENSE
--rw-r--r--   0        0        0     2863 2023-02-28 03:43:21.835687 smunger-0.0.9/README.md
--rw-r--r--   0        0        0     2977 2023-02-28 03:43:21.835687 smunger-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      857 2023-02-28 03:43:21.835687 smunger-0.0.9/smunger/__init__.py
--rw-r--r--   0        0        0     1723 2023-02-28 03:43:21.835687 smunger-0.0.9/smunger/annotate.py
--rw-r--r--   0        0        0     5600 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/cli.py
--rw-r--r--   0        0        0       83 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/console.py
--rw-r--r--   0        0        0     6398 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/constant.py
--rw-r--r--   0        0        0     3854 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/io.py
--rw-r--r--   0        0        0     3665 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/liftover.py
--rw-r--r--   0        0        0     5575 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/mapheader.py
--rw-r--r--   0        0        0    11314 2023-02-28 03:43:21.839687 smunger-0.0.9/smunger/smunger.py
--rw-r--r--   0        0        0       37 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/__init__.py
--rw-r--r--   0        0        0     1456 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/annota_rsid_test.py
--rw-r--r--   0        0        0      269 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/exampledata/catalog.header.json
--rw-r--r--   0        0        0   115228 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/exampledata/catalog.munged.hg38.txt.gz
--rw-r--r--   0        0        0   502403 2023-02-28 03:43:21.839687 smunger-0.0.9/tests/exampledata/catalog.munged.rsid.txt
--rw-r--r--   0        0        0   120144 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/catalog.munged.txt.gz
--rw-r--r--   0        0        0     1931 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/catalog.munged.txt.gz.tbi
--rw-r--r--   0        0        0   124530 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/catalog.txt.gz
--rw-r--r--   0        0        0       72 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/test.header.json
--rw-r--r--   0        0        0    41670 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/test.munged.txt.gz
--rw-r--r--   0        0        0      738 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/test.munged.txt.gz.tbi
--rw-r--r--   0        0        0   789756 2023-02-28 03:43:21.843687 smunger-0.0.9/tests/exampledata/test.txt.gz
--rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 smunger-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-14 06:12:39.224249 smunger-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2863 2023-06-14 06:12:39.224249 smunger-0.1.0/README.md
+-rw-r--r--   0        0        0     3017 2023-06-14 06:12:39.228249 smunger-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      992 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/__init__.py
+-rw-r--r--   0        0        0     2558 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/annotate.py
+-rw-r--r--   0        0        0     6804 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/cli.py
+-rw-r--r--   0        0        0       83 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/console.py
+-rw-r--r--   0        0        0     6818 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/constant.py
+-rw-r--r--   0        0        0     5060 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/io.py
+-rw-r--r--   0        0        0     3993 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/liftover.py
+-rw-r--r--   0        0        0     5611 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/mapheader.py
+-rw-r--r--   0        0        0     3742 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/plots.py
+-rw-r--r--   0        0        0    12800 2023-06-14 06:12:39.228249 smunger-0.1.0/smunger/smunger.py
+-rw-r--r--   0        0        0       37 2023-06-14 06:12:39.228249 smunger-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-14 06:12:39.228249 smunger-0.1.0/tests/annota_rsid_test.py
+-rw-r--r--   0        0        0      269 2023-06-14 06:12:39.228249 smunger-0.1.0/tests/exampledata/catalog.header.json
+-rw-r--r--   0        0        0   115228 2023-06-14 06:12:39.228249 smunger-0.1.0/tests/exampledata/catalog.munged.hg38.txt.gz
+-rw-r--r--   0        0        0   502256 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/catalog.munged.rsid.txt
+-rw-r--r--   0        0        0   120144 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/catalog.munged.txt.gz
+-rw-r--r--   0        0        0     1931 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/catalog.munged.txt.gz.tbi
+-rw-r--r--   0        0        0   124530 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/catalog.txt.gz
+-rw-r--r--   0        0        0       72 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/test.header.json
+-rw-r--r--   0        0        0    41670 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/test.munged.txt.gz
+-rw-r--r--   0        0        0      738 2023-06-14 06:12:39.232249 smunger-0.1.0/tests/exampledata/test.munged.txt.gz.tbi
+-rw-r--r--   0        0        0   789756 2023-06-14 06:12:39.236249 smunger-0.1.0/tests/exampledata/test.txt.gz
+-rw-r--r--   0        0        0     5207 1970-01-01 00:00:00.000000 smunger-0.1.0/PKG-INFO
```

### Comparing `smunger-0.0.9/LICENSE` & `smunger-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smunger-0.0.9/README.md` & `smunger-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `smunger-0.0.9/pyproject.toml` & `smunger-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "smunger"
-version = "0.0.9"
+version = "0.1.0"
 homepage = "https://github.com/jianhua/smunger"
 description = "munger for GWAS summary statistics."
 authors = ["Jianhua Wang <jianhua.mert@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -47,14 +47,16 @@
 mkdocs-material-extensions = {version = "^1.1.1", optional = true}
 jupyter = { version = "^1.0.0", optional = true }
 pandas = "^1.5.3"
 rich = "^13.3.1"
 liftover = "^1.1.16"
 requests = "^2.28.2"
 pytabix = "^0.1"
+scipy = "^1.10.1"
+matplotlib = "^3.7.1"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
```

### Comparing `smunger-0.0.9/smunger/__init__.py` & `smunger-0.1.0/smunger/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 
 from rich.logging import RichHandler
 
 from .console import console
 from .constant import ColAllowNA, ColName, ColRange, ColType
-from .io import load_sumstats, save_sumstats
+from .io import load_sumstats, save_sumstats, check_header, export_sumstats
 from .mapheader import map_colnames
 from .smunger import (
     make_SNPID_unique,
     extract_cols,
     munge,
     munge_allele,
     munge_beta,
@@ -18,22 +18,24 @@
     munge_chr,
     munge_eaf,
     munge_maf,
     munge_or,
     munge_pvalue,
     munge_se,
     munge_z,
+    harmonize,
 )
 from .liftover import liftover, liftover_file
-from .annotate import annotate_rsid
+from .annotate import annotate_rsid, annotate_rsid_file
+from .plots import qqplot, get_qq_df, manhattan, get_manh_df, qqman
 
 __author__ = """Jianhua Wang"""
 __email__ = 'jianhua.mert@gmail.com'
-__version__ = '0.0.9'
+__version__ = '0.1.0'
 
 # Set up logging
 logging.basicConfig(
-    level=logging.NOTSET,
+    level=logging.WARNING,
     format="%(name)s - %(message)s",
     datefmt="[%X]",
     handlers=[RichHandler(rich_tracebacks=True, show_path=False)],
 )
```

### Comparing `smunger-0.0.9/smunger/annotate.py` & `smunger-0.1.0/tests/annota_rsid_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-"""Module for annotating a file with the results of a Smunger run."""
-
-import logging
 import tabix
 import pandas as pd
-from smunger.constant import ColName
+import logging
 
-logger = logging.getLogger('annotate')
+logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
+file = '/f/jianhua/Resources/rs2pos/pos2rsid.txt.gz'
+tb = tabix.open(file)
+outfile = '~/catalog.munged.rsid.txt'
 
-def annotate_rsid(
-    infile: str,
-    outfile: str,
-    database: str,
-    chunksize: int = 2000000,
-    rsid_col: str = ColName.RSID,
-    chrom_col: str = ColName.CHR,
-    pos_col: str = ColName.BP,
-) -> None:
-    """Annotate a file with rsids."""
-    tb = tabix.open(database)
-    ith = 0
-    for df in pd.read_csv(infile, sep='\t', chunksize=100000):
-        for chrom, chr_df in df.groupby(chrom_col):
-            chr_df = chr_df.sort_values(pos_col)
-            for i in range(chr_df[pos_col].min(), chr_df[pos_col].max(), chunksize):
-                chunk_df = chr_df[(chr_df[pos_col] >= i) & (chr_df[pos_col] < i + chunksize)].copy()
-                if len(chunk_df) == 0:
-                    continue
-                rsid_map = pd.DataFrame(
-                    columns=['chr', 'bp', 'rsid', 'ref', 'alt'], data=tb.query('1', i - 1, i + chunksize)
-                )
-                rsid_map = rsid_map.drop_duplicates(subset=['bp'])
-                rsid_map['bp'] = rsid_map['bp'].astype(int)
-                rsid_map = pd.Series(data=rsid_map['rsid'].values, index=rsid_map['bp'].values)
-                chunk_df[rsid_col] = chunk_df[pos_col].map(rsid_map)
-                logging.info(f'Processing {chrom}:{i}-{i + chunksize}, chunk No.{ith}, {len(chunk_df)} rows.')
-                ith += 1
-                if ith == 1:
-                    chunk_df.to_csv(outfile, sep='\t', index=False, mode='w')
-                else:
-                    chunk_df.to_csv(outfile, sep='\t', index=False, mode='a', header=False)
+chunksize = 2000000
+ith = 0
+for df in pd.read_csv('~/catalog.munged.txt.gz', sep='\t', chunksize=100000):
+    for chrom, chr_df in df.groupby('CHR'):
+        chr_df = chr_df.sort_values('BP')
+        for i in range(chr_df['BP'].min(), chr_df['BP'].max(), chunksize):
+            chunk_df = chr_df[(chr_df['BP'] >= i) & (chr_df['BP'] < i + chunksize)].copy()
+            if len(chunk_df) == 0:
+                continue
+            rsid_map = pd.DataFrame(
+                columns=['chr', 'bp', 'rsid', 'ref', 'alt'], data=tb.query('1', i - 1, i + chunksize)
+            )
+            rsid_map = rsid_map.drop_duplicates(subset=['bp'])
+            rsid_map['bp'] = rsid_map['bp'].astype(int)
+            rsid_map = pd.Series(data=rsid_map['rsid'].values, index=rsid_map['bp'].values)
+            chunk_df['rsID'] = chunk_df['BP'].map(rsid_map)
+            logging.info(f'Processing {chrom}:{i}-{i + chunksize}, chunk No.{ith}, {len(chunk_df)} rows.')
+            ith += 1
+            if ith == 1:
+                chunk_df.to_csv(outfile, sep='\t', index=False, mode='w')
+            else:
+                chunk_df.to_csv(outfile, sep='\t', index=False, mode='a', header=False)
```

### Comparing `smunger-0.0.9/smunger/cli.py` & `smunger-0.1.0/smunger/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         logging.info('Verbose mode is on.')
     else:
         logging.getLogger().setLevel(logging.INFO)
 
 
 @app.command()
 def mapheader(
-    infile: Path = typer.Argument(..., help='Input summary statistics.'),
+    infile: str = typer.Argument(..., help='Input summary statistics.'),
     outfile: Path = typer.Argument(..., help='Output file, json.'),
     sep: str = typer.Option(None, '--sep', '-s', help='Separator of the input file.'),
     nrows: int = typer.Option(5, '--nrows', '-n', help='Number of rows to display.'),
     skiprows: int = typer.Option(0, '--skiprows', '-k', help='Number of rows to skip.'),
     comment: str = typer.Option(None, '--comment', '-c', help='Comment character.'),
     gzipped: bool = typer.Option(None, '--gzipped', '-z', help='Input file is gzipped.'),
 ):
@@ -47,23 +47,23 @@
 
     df = load_sumstats(infile, nrows=nrows, sep=sep, skiprows=skiprows, comment=comment, gzipped=gzipped)
     map_colnames(df, outfile=outfile)
 
 
 @app.command()
 def munge(
-    infile: Path = typer.Argument(..., help='Input summary statistics.'),
-    outfile: Path = typer.Argument(..., help='Output munged summary statistics.'),
+    infile: str = typer.Argument(..., help='Input summary statistics.'),
+    outfile: str = typer.Argument(..., help='Output munged summary statistics.'),
     colmap: str = typer.Argument(..., help='Column map file, json.'),
     sep: str = typer.Option(None, '--sep', '-s', help='Separator of the input file.'),
     skiprows: int = typer.Option(0, '--skiprows', '-k', help='Number of rows to skip.'),
     comment: str = typer.Option(None, '--comment', '-c', help='Comment character.'),
     gzipped: bool = typer.Option(None, '--gzipped', '-z', help='Input file is gzipped.'),
     build_index: bool = typer.Option(True, '--build-index', '-b', help='Build tabix index.'),
-    sigsnps: Path = typer.Option(None, '--sigsnps', '-S', help='save significant SNPs to file.'),
+    sigsnps: str = typer.Option(None, '--sigsnps', '-S', help='save significant SNPs to file.'),
     sigsnps_pval: float = typer.Option(5e-8, '--sigsnps-pval', '-P', help='p-value threshold for significant SNPs.'),
     report: str = typer.Option(None, '--report', '-R', help='save report to file.'),
 ):
     """Munge summary statistics."""
     import smunger
     from smunger.io import load_sumstats, save_sumstats
 
@@ -91,14 +91,42 @@
     if report:
         import json
 
         with open(report, 'w') as f:
             json.dump(report_json, f, indent=4)
 
 
+@app.command()
+def extract(
+    infile: str = typer.Argument(..., help='Input summary statistics.'),
+    outfile: str = typer.Argument(..., help='Output munged summary statistics.'),
+    rename_headers: str = typer.Option(None, '--rename-headers', '-r', help='Rename headers, json.'),
+    chrom: int = typer.Option(None, '--chrom', '-c', help='Chromosome.'),
+    start: int = typer.Option(None, '--start', '-s', help='Start position.'),
+    end: int = typer.Option(None, '--end', '-e', help='End position.'),
+    no_bgzip: bool = typer.Option(True, '--no-bgzip', '-z', help='Do not bgzip output file.'),
+):
+    """Extract columns."""
+    from smunger.io import export_sumstats
+    import json
+    if rename_headers:
+        headers_map = json.loads(rename_headers)
+    else:
+        headers_map = None
+    export_sumstats(
+        filename=infile,
+        out_filename=outfile,
+        rename_headers=headers_map,
+        chrom=chrom,
+        start=start,
+        end=end,
+        bgzipped=no_bgzip,
+    )
+
+
 class Build(str, Enum):
     """Genome Builds."""
 
     hg17 = 'hg17'
     hg18 = 'hg18'
     hg19 = 'hg19'
     hg38 = 'hg38'
@@ -124,16 +152,18 @@
     infile: str = typer.Argument(..., help='Input summary statistics.'),
     outfile: str = typer.Argument(..., help='Output munged summary statistics.'),
     database: str = typer.Option(..., '--database', '-d', help='Database.'),
     chunksize: int = typer.Option(2000000, '--chunksize', '-c', help='Chunk size.'),
     rsidcol: str = typer.Option('rsID', '--rsidcol', '-r', help='rsid column.'),
     chromcol: str = typer.Option('CHR', '--chromcol', '-C', help='chromosome column.'),
     poscol: str = typer.Option('BP', '--poscol', '-p', help='position column.'),
+    eacol: str = typer.Option('EA', '--eacol', '-e', help='effect allele column.'),
+    neacol: str = typer.Option('NEA', '--neacol', '-n', help='non-effect allele column.'),
 ):
     """Annotate rsid."""
-    from smunger.annotate import annotate_rsid
+    from smunger.annotate import annotate_rsid_file
 
-    annotate_rsid(infile, outfile, database, chunksize, rsidcol, chromcol, poscol)
+    annotate_rsid_file(infile, outfile, database, chunksize, rsidcol, chromcol, poscol, eacol, neacol)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `smunger-0.0.9/smunger/constant.py` & `smunger-0.1.0/smunger/constant.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,40 @@
     MAF = "MAF"
     N = "N"
     Z = "Z"
     INFO = "INFO"
     OUTCOLS = ['CHR', 'BP', 'rsID', 'EA', 'NEA', 'EAF', 'MAF', 'BETA', 'SE', 'P']
 
 
+chrom_len = {
+    1: 249250621,
+    2: 243199373,
+    3: 198022430,
+    4: 191154276,
+    5: 180915260,
+    6: 171115067,
+    7: 159138663,
+    8: 146364022,
+    9: 141213431,
+    10: 135534747,
+    11: 135006516,
+    12: 133851895,
+    13: 115169878,
+    14: 107349540,
+    15: 102531392,
+    16: 90354753,
+    17: 81195210,
+    18: 78077248,
+    19: 59128983,
+    20: 63025520,
+    21: 48129895,
+    22: 51304566,
+}
+
+
 class ColType:
     """Define column types."""
 
     CHR = int
     BP = int
     RSID = str
     EA = str
```

### Comparing `smunger-0.0.9/smunger/io.py` & `smunger-0.1.0/smunger/io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """Read and write data from/to files."""
 
 import gzip
 import logging
 import shutil
+import os
 from pathlib import Path
 from subprocess import PIPE, run
-from typing import Optional, Union
+from typing import Optional
 
 import pandas as pd
-
+import tabix
 from .constant import ColName
+from .smunger import munge
 
 logger = logging.getLogger('io')
 
 
 def load_sumstats(
-    filename: Union[str, Path],
+    filename: str,
     sep: Optional[str] = None,
     nrows: Optional[int] = None,
     skiprows: int = 0,
     comment: Optional[str] = None,
     gzipped: Optional[bool] = None,
 ) -> pd.DataFrame:
     """Load summary statistics from a file."""
     # determine whether the file is gzipped
-    if isinstance(filename, str):
-        filename = Path(filename)
     if gzipped is None:
-        gzipped = filename.suffix.endswith('gz')
+        gzipped = filename.endswith('gz')
 
     # read the first line of the file to determine the separator
     if sep is None:
         if gzipped:
             with gzip.open(filename, 'rt') as f:
                 line = f.readline()
         else:
@@ -48,14 +48,24 @@
     logger.info(f'loading data from {filename}')
     # determine the separator, automatically if not specified
     return pd.read_csv(
         filename, sep=sep, nrows=nrows, skiprows=skiprows, comment=comment, compression='gzip' if gzipped else None
     )
 
 
+def check_header(filename) -> bool:
+    """Check if the header of a file contains the required columns."""
+    header = load_sumstats(filename, nrows=5)
+    if list(header.columns) != list(ColName.OUTCOLS):
+        logger.error(f'Header of {filename} does not contain the required columns.')
+        raise ValueError(f'Header of {filename} does not contain the required columns.')
+    else:
+        return True
+
+
 def check_tool(tool: str) -> str:
     """
     Check if tool is installed.
 
     Parameters
     ----------
     tool : str
@@ -70,36 +80,36 @@
     if tool_path:
         return tool_path
     else:
         logger.error(f"{tool} is not installed. Please install it first and make sure it is in your PATH.")
         raise ValueError(f"{tool} is not installed. Please install it first and make sure it is in your PATH.")
 
 
-def save_sumstats(sumstats: pd.DataFrame, filename: Union[str, Path], build_index: bool = True):
+def save_sumstats(sumstats: pd.DataFrame, filename: str, build_index: bool = True, bgzipped: bool = True):
     """Save summary statistics to a file."""
     # save the summary statistics to a file
-    if isinstance(filename, str):
-        filename = Path(filename)
-    if filename.exists():
+    filename_path = Path(filename)
+    if filename_path.exists():
         logger.warning(f'File {filename} already exists. Overwriting.')
 
-    if filename.suffix == '.gz':
-        filename = filename.with_suffix('')
+    if filename_path.suffix == '.gz':
+        filename_path = filename_path.with_suffix('')
     sumstats = sumstats.sort_values(by=[ColName.CHR, ColName.BP])
-    logger.info(f'Saving summary statistics to {filename}')
-    sumstats.to_csv(filename, sep='\t', index=False, header=True, float_format='%g')
+    logger.info(f'Saving summary statistics to {filename_path}')
+    sumstats.to_csv(filename_path, sep='\t', index=False, header=True, float_format='%g')
 
     # compress the file
-    compress(filename)
+    if bgzipped:
+        compress(str(filename_path))
     # index the file
-    if build_index:
-        index(str(filename) + '.gz')
+    if build_index and bgzipped:
+        index(str(filename_path) + '.gz')
 
 
-def compress(filename: Path):
+def compress(filename: str):
     """Compress a file with bgzip."""
     bgzip = check_tool('bgzip')
     logger.info(f'Compressing {filename} with bgzip')
     run([bgzip, '-f', str(filename)], stdout=PIPE, stderr=PIPE, check=True)
 
 
 def index(filename: str, start: int = 1, end: int = 2, skip: int = 1):
@@ -110,14 +120,35 @@
         [tabix, '-f', '-S', str(skip), '-s', str(start), '-b', str(end), '-e', str(end), filename],
         stdout=PIPE,
         stderr=PIPE,
         check=True,
     )
 
 
-def export_sumstats(filename: Union[str, Path], chrom: Optional[int] = None,
-                    start: Optional[int] = None, end: Optional[int] = None,
-                    rename_headers: Optional[dict] = None,
-                    out_filename: Optional[Union[str, Path]] = None,
-                    gzipped: bool = True) -> pd.DataFrame:
+def export_sumstats(
+    filename: str,
+    chrom: Optional[int] = None,
+    start: Optional[int] = None,
+    end: Optional[int] = None,
+    rename_headers: Optional[dict] = None,
+    out_filename: Optional[str] = None,
+    bgzipped: bool = True,
+) -> pd.DataFrame:
     """Export summary statistics to a file."""
-    raise NotImplementedError
+    if chrom and start and end:
+        logger.info(f'Loading summary statistics from {filename} for {chrom}:{start}-{end}')
+        if not os.path.exists(filename + '.tbi'):
+            raise FileNotFoundError(f'Index file {filename}tbi does not exist. Please index the file first.')
+        else:
+            tb = tabix.open(filename)
+            indf = pd.DataFrame(columns=ColName.OUTCOLS, data=tb.query(str(chrom), start, end))
+            indf = munge(indf)
+    else:
+        logger.info(f'Loading summary statistics from {filename}')
+        indf = load_sumstats(filename)
+    if rename_headers:
+        logger.info(f'Renaming headers to {rename_headers}')
+        indf = indf[list(rename_headers.keys())].copy()
+        indf = indf.rename(columns=rename_headers)
+    if out_filename:
+        save_sumstats(indf, out_filename, build_index=False, bgzipped=bgzipped)
+    return indf
```

### Comparing `smunger-0.0.9/smunger/liftover.py` & `smunger-0.1.0/smunger/liftover.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,20 +77,26 @@
     inbuild: str,
     outbuild: str,
     chrom_col: str = ColName.CHR,
     pos_col: str = ColName.BP,
 ) -> pd.DataFrame:
     """Liftover summary statistics from one genome build to another."""
     lo = get_lifter(inbuild, outbuild)
-    df[outbuild] = df[[chrom_col, pos_col]].apply(lambda x: lo.query(x[0], x[1]), axis=1)
-    df[chrom_col] = df[outbuild].apply(lambda x: x[0][0] if len(x) > 0 else 0)
-    df[pos_col] = df[outbuild].apply(lambda x: x[0][1] if len(x) > 0 else 0)
+    df = df.rename(columns={chrom_col: ColName.CHR, pos_col: ColName.BP})
+    df = munge_chr(df)
+    df = munge_bp(df)
+    df[ColName.CHR] = 'chr' + df[ColName.CHR].astype(str)
+    df[ColName.CHR] = df[ColName.CHR].str.replace('chr23', 'chrX')
+    df[outbuild] = df[[ColName.CHR, ColName.BP]].apply(lambda x: lo.query(x[0], x[1]), axis=1)
+    df[ColName.CHR] = df[outbuild].apply(lambda x: x[0][0] if len(x) > 0 else 0)
+    df[ColName.BP] = df[outbuild].apply(lambda x: x[0][1] if len(x) > 0 else 0)
     df.drop(outbuild, axis=1, inplace=True)
     df = munge_chr(df)
     df = munge_bp(df)
+    df = df.rename(columns={ColName.CHR: chrom_col, ColName.BP: pos_col})
     return df
 
 
 def liftover_file(
     infile: str,
     outfile: str,
     inbuild: str,
```

### Comparing `smunger-0.0.9/smunger/mapheader.py` & `smunger-0.1.0/smunger/mapheader.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                         continue
                     else:
                         manual_map = df_cols[int(manual_map)]
                         colname_map[manual_map] = col
     # use -log10(P) if P is not found
     if ColName.P not in colname_map.values():
         console.print("P is not found.")
-        for col in [ColName.NEGLOGP]:
+        for col in [ColName.NEGLOGP]:  # TODO: use NEGLOGP if it is found
             if col in guess_orignal_out:
                 map_correct = Confirm.ask(
                     f"Is {guess_orignal_out[col]} the correct column name for {col}?", default=True
                 )
                 if map_correct:
                     colname_map[guess_orignal_out[col]] = col
                 else:
```

### Comparing `smunger-0.0.9/smunger/smunger.py` & `smunger-0.1.0/smunger/smunger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """Main module."""
 
 import json
 import logging
 from typing import Union
 
+import numpy as np
 import pandas as pd
 
 from smunger.constant import ColName, ColRange, ColType
 
 logger = logging.getLogger('munger')
 
 
-def make_SNPID_unique(sumstat: pd.DataFrame) -> pd.DataFrame:
+def make_SNPID_unique(
+    sumstat: pd.DataFrame,
+    chrom_col: str = ColName.CHR,
+    pos_col: str = ColName.BP,
+    ea_col: str = ColName.EA,
+    nea_col: str = ColName.NEA,
+) -> pd.DataFrame:
     """
     Make the SNPID unique.
 
     The unique SNPID is chr-bp-sorted(EA,NEA)
 
     Parameters
     ----------
@@ -24,56 +31,61 @@
 
     Returns
     -------
     pd.DataFrame
         The summary statistics with unique SNPID.
     """
     df = sumstat.copy()
-    allele_df = df[[ColName.EA, ColName.NEA]].copy()
+    allele_df = df[[ea_col, nea_col]].copy()
     b = allele_df.values
     b.sort(axis=1)
-    allele_df[[ColName.EA, ColName.NEA]] = b
+    allele_df[[ea_col, nea_col]] = b
     allele_df[ColName.SNPID] = (
-        df[ColName.CHR].astype(str)
+        df[chrom_col].astype(str)
         + "-"
-        + df[ColName.BP].astype(str)
+        + df[pos_col].astype(str)
         + "-"
-        + allele_df[ColName.EA]
+        + allele_df[ea_col]
         + "-"
-        + allele_df[ColName.NEA]
+        + allele_df[nea_col]
     )
+    if ColName.SNPID in df.columns:
+        df.drop(ColName.SNPID, axis=1, inplace=True)
     df.insert(loc=0, column=ColName.SNPID, value=allele_df[ColName.SNPID].values)  # type: ignore
     return df
 
 
 def extract_cols(df: pd.DataFrame, colname_map: Union[dict, str]) -> pd.DataFrame:
     """Map column names."""
     # map column names
     if isinstance(colname_map, str):
         with open(colname_map, 'r') as f:
             colname_map = json.load(f)
-    outdf = df.rename(columns=colname_map).copy()  # type: ignore
-    mapped_cols = list(colname_map.values())  # type: ignore
-    outdf = outdf[mapped_cols]
+    colname_map = dict(colname_map)  # type: ignore
+    colname_map = {k: v for k, v in colname_map.items() if k in df.columns}
+    outdf = df.rename(columns=colname_map).copy()
+    mapped_cols = list(colname_map.values())
+    outdf = outdf[mapped_cols]  # type: ignore
     outdf = rm_col_allna(outdf)
     return outdf
 
 
-def checl_colnames(df: pd.DataFrame) -> pd.DataFrame:
+def check_colnames(df: pd.DataFrame) -> pd.DataFrame:
     """Check column names, fill None if not presents."""
     outdf = df.copy()
     for col in ColName.OUTCOLS:
         if col not in outdf.columns:
             outdf[col] = None
     return outdf[ColName.OUTCOLS]
 
 
 def rm_col_allna(df: pd.DataFrame) -> pd.DataFrame:
     """Remove columns that are all NA."""
     outdf = df.copy()
+    outdf = outdf.replace('', None)
     for col in outdf.columns:
         if outdf[col].isnull().all():
             logger.debug(f"Remove column {col} because it is all NA.")
             outdf.drop(col, axis=1, inplace=True)
     return outdf
 
 
@@ -86,14 +98,15 @@
         raise ValueError("Missing P column.")
     return outdf
 
 
 def munge(df: pd.DataFrame) -> pd.DataFrame:
     """Munge the summary statistics."""
     outdf = df.copy()
+    outdf = rm_col_allna(outdf)
     if all(
         [
             ColName.CHR in outdf.columns,
             ColName.BP in outdf.columns,
             ColName.EA in outdf.columns,
             ColName.NEA in outdf.columns,
         ]
@@ -140,15 +153,15 @@
         outdf = munge_z(outdf)
 
     if ColName.EAF in outdf.columns:
         outdf = munge_eaf(outdf)
         outdf[ColName.MAF] = outdf[ColName.EAF]
     if ColName.MAF in outdf.columns:
         outdf = munge_maf(outdf)
-    outdf = checl_colnames(outdf)
+    outdf = check_colnames(outdf)
     return outdf
 
 
 def munge_rsid(df: pd.DataFrame) -> pd.DataFrame:
     """Munge rsID column."""
     outdf = df.copy()
     outdf[ColName.RSID] = outdf[ColName.RSID].astype(ColType.RSID)
@@ -312,7 +325,39 @@
     outdf = outdf[outdf[ColName.MAF].notnull()]
     outdf[ColName.MAF] = outdf[ColName.MAF].apply(lambda x: 1 - x if x > 0.5 else x)
     outdf = outdf[(outdf[ColName.MAF] >= ColRange.MAF_MIN) & (outdf[ColName.MAF] <= ColRange.MAF_MAX)]
     after_n = outdf.shape[0]
     logger.debug(f"Remove {pre_n - after_n} rows because of invalid maf.")
     outdf[ColName.MAF] = outdf[ColName.MAF].astype(ColType.MAF)
     return outdf
+
+
+def calculate_lambda(df: pd.DataFrame) -> float:
+    """Calculate lambda."""
+    from scipy import stats
+
+    observed = np.median((df[ColName.BETA] / df[ColName.SE]) ** 2)
+    lambda_gc = observed / stats.chi2.ppf(0.5, 1)
+    return lambda_gc  # type: ignore
+
+
+def harmonize(sumstat1, sumstat2) -> pd.DataFrame:
+    """Harmonize two sumstats."""
+    sumstat1 = make_SNPID_unique(sumstat1)
+    sumstat2 = make_SNPID_unique(sumstat2)
+    merged = pd.merge(sumstat1, sumstat2, on=ColName.SNPID, how="inner", suffixes=("_1", "_2"))
+    merged[f'{ColName.BETA}_2'] = merged[f'{ColName.BETA}_2'].where(
+        merged[f'{ColName.EA}_1'] == merged[f'{ColName.EA}_2'], -merged[f'{ColName.BETA}_2']
+    )
+    del merged[f'{ColName.EA}_2']
+    del merged[f'{ColName.NEA}_2']
+    del merged[f'{ColName.CHR}_2']
+    del merged[f'{ColName.BP}_2']
+    merged = merged.rename(
+        columns={
+            f'{ColName.EA}_1': ColName.EA,
+            f'{ColName.NEA}_1': ColName.NEA,
+            f'{ColName.CHR}_1': ColName.CHR,
+            f'{ColName.BP}_1': ColName.BP,
+        }
+    )
+    return merged
```

### Comparing `smunger-0.0.9/tests/exampledata/catalog.munged.hg38.txt.gz` & `smunger-0.1.0/tests/exampledata/catalog.munged.hg38.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.9/tests/exampledata/catalog.munged.rsid.txt` & `smunger-0.1.0/tests/exampledata/catalog.munged.rsid.txt`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 1	1022423	rs114326054	G	A			-0.0462	0.0521	0.3755
 1	1023145	rs3737727	G	A			0.0031	0.0252	0.9024
 1	1023310	rs11260589	C	T			-0.0075	0.0253	0.7654
 1	1023788	rs12132100	C	T			0.0095	0.0259	0.7137
 1	1025270	rs72631896	C	T			0.0078	0.0351	0.824
 1	1025301	rs9442400	C	T			0.0511	0.0337	0.1298
 1	10000006	rs186077422	G	A			-0.0385	0.1421	0.7864
-1	10000179	rs1221011233	AAAAAAAC	A			-0.2343	0.1199	0.05072
+1	10000179	rs149841286	AAAAAAAC	A			-0.2343	0.1199	0.05072
 1	10000400	rs1237370	T	A			-0.0546	0.0238	0.02159
 1	10000476	rs182770070	T	A			-0.0241	0.0899	0.7887
 1	10001401	rs60132751	C	T			-0.0836	0.0365	0.02192
 1	10001675	rs187778946	G	A			-0.2552	0.1585	0.1075
 1	10001911	rs140852334	C	T			0.0121	0.0907	0.8942
 1	10001980	rs1220424	T	A			-0.0081	0.0198	0.6811
 1	10001981	rs111999762	T	A			-0.0569	0.0419	0.1743
@@ -184,15 +184,15 @@
 1	10046460	rs12136213	G	A			0.0107	0.0198	0.5901
 1	10046812	rs57702810	C	T			-0.056	0.0917	0.5414
 1	10046897	rs138222412	G	A			0.0523	0.102	0.6084
 1	10047003	rs142153896	G	C			0.2805	0.1251	0.025
 1	10047519	rs150233209	G	A			0.0434	0.0431	0.3133
 1	10047693	rs144209151	G	A			-0.027	0.0507	0.5945
 1	10047747	rs12060375	C	A			-0.074	0.0398	0.06319
-1	10047793	rs376301071	GAGA	G			0.0563	0.0405	0.1652
+1	10047793	rs150398864	GAGA	G			0.0563	0.0405	0.1652
 1	10048119	rs12091993	G	A			-0.0207	0.0509	0.6837
 1	10048150	rs150672738	G	T			-0.0754	0.0466	0.1054
 1	10048151	rs139490379	G	T			-0.076	0.0498	0.1268
 1	10048490	rs116364879	G	T			-0.0221	0.0509	0.6633
 1	10048875	rs149694992	C	T			-0.0802	0.0398	0.04405
 1	10049177	rs12140058	G	T			-0.0059	0.0222	0.7916
 1	10049352	rs61782884	C	T			0.0566	0.0421	0.1782
@@ -243,15 +243,15 @@
 1	10068175	rs11578833	G	A			-0.0195	0.0713	0.7846
 1	10068428	rs147735686	G	A			0.2129	0.1337	0.1113
 1	10068477	rs11121514	G	A			-0.0046	0.0242	0.8498
 1	10068579	rs113023880	G	A			-0.0283	0.0387	0.4639
 1	10068602	rs138897380	G	A			-0.1879	0.1177	0.1103
 1	10069714	rs145946129	C	T			-0.1495	0.1086	0.1686
 1	10069756	rs3013788	G	A			-0.0016	0.0222	0.9435
-1	10069792	rs756715124	ATT	A			-0.0733	0.0431	0.08936
+1	10069792	rs146403712	ATT	A			-0.0733	0.0431	0.08936
 1	10070036	rs74681101	G	T			0.0341	0.0508	0.5014
 1	10070822	rs150809370	G	A			0.0361	0.051	0.4791
 1	10070866	rs78604748	TC	T			-0.0022	0.0248	0.9293
 1	10071301	rs3003376	C	T			0.0024	0.0223	0.915
 1	10071787	rs77984683	C	T			0.2088	0.1199	0.08179
 1	10072597	rs3123522	C	T			0.0018	0.0222	0.9359
 1	10074011	rs185744054	G	A			0.1013	0.174	0.5604
@@ -309,15 +309,15 @@
 1	10097208	rs113826563	G	C			-0.04	0.0417	0.3385
 1	10097571	rs79583882	C	T			-0.119	0.1586	0.4529
 1	10097604	rs116287312	G	A			-0.0456	0.0506	0.3677
 1	10097672	rs6693449	G	A			0.0016	0.0218	0.9402
 1	10098028	rs116782657	C	A			0.0704	0.053	0.1845
 1	10098850	rs76200681	C	T			-0.0464	0.0507	0.3602
 1	10098987	rs11804755	G	A			-0.0222	0.1191	0.8521
-1	10099151	rs1204676206	AAAAC	A			0.0469	0.0394	0.2335
+1	10099151	rs142086424	AAAAC	A			0.0469	0.0394	0.2335
 1	10100469	rs146824468	C	T			-0.0473	0.0507	0.3505
 1	10100739	rs143663738	G	A			-0.1088	0.1116	0.3297
 1	10101273	rs74875629	G	A			0.0443	0.0509	0.3833
 1	10102209	rs79383368	G	A			0.0459	0.0508	0.3657
 1	10102691	rs115625504	C	T			0.0404	0.047	0.3895
 1	10103131	rs11804193	C	A			0.0129	0.0284	0.6497
 1	10103577	rs150809853	C	T			0.0457	0.0459	0.3196
@@ -348,15 +348,15 @@
 1	10117444	rs77559290	C	T			-0.034	0.0598	0.5697
 1	10117876	rs78739590	G	A			0.0753	0.1863	0.6859
 1	10118448	rs139852529	G	A			0.0441	0.1018	0.6645
 1	10118731	rs142864591	GT	G			0.0404	0.047	0.3899
 1	10118778	rs74051807	C	T			-0.0642	0.0368	0.0812
 1	10119723	rs140572802	C	T			-0.046	0.0506	0.3631
 1	10119822	rs74669740	G	A			-0.0984	0.0869	0.2574
-1	10121315	rs866181620	AGTTT	A			0.1178	0.1031	0.2529
+1	10121315	rs148389459	AGTTT	A			0.1178	0.1031	0.2529
 1	10121399	rs116661119	G	A			-0.0535	0.05	0.2851
 1	10121799	rs148905031	G	A			-0.104	0.1168	0.3731
 1	10122157	rs148032713	G	A			0.0545	0.067	0.4159
 1	10122261	rs35646986	C	T			0.0591	0.0533	0.2682
 1	10122678	rs61462323	C	T			-0.0411	0.047	0.3817
 1	10122779	rs61650275	G	C			-0.0067	0.0231	0.7705
 1	10123001	rs58453167	C	T			0.043	0.046	0.3498
@@ -411,17 +411,17 @@
 1	10146380	rs60208411	C	T			0.066	0.0273	0.01574
 1	10146978	rs111893655	C	T			0.046	0.047	0.3275
 1	10147644	rs72861431	G	C			-0.0445	0.047	0.3435
 1	10147999	rs78508549	C	T			0.049	0.0589	0.4057
 1	10148545	rs4388708	C	T			-0.053	0.057	0.3526
 1	10148798	rs113586345	C	T			-0.0491	0.0375	0.1901
 1	10149529	rs74051808	C	T			0.0622	0.034	0.06714
-1	10150184	rs766754424	TG	T			0.0046	0.0253	0.8562
+1	10150184	rs111297331	TG	T			0.0046	0.0253	0.8562
 1	10150402	rs141780625	G	T			0.1215	0.1578	0.4413
-1	10152280	rs1366712013	C	CTT			-0.0065	0.0257	0.8004
+1	10152280	rs138009294	C	CTT			-0.0065	0.0257	0.8004
 1	10152882	rs6676280	G	A			-0.0029	0.0221	0.8968
 1	10152945	rs114627513	T	A			0.0496	0.0507	0.3279
 1	10153153	rs11801988	G	A			0.039	0.0469	0.4057
 1	10153189	rs114192263	G	A			-0.1258	0.1614	0.4356
 1	10153685	rs142599147	C	A			-0.054	0.1737	0.7558
 1	10154460	rs113304383	C	T			0.0683	0.0638	0.2839
 1	10154574	rs11121516	C	T			0.0165	0.0245	0.4995
@@ -463,15 +463,15 @@
 1	10171318	rs72861453	C	T			0.0372	0.0466	0.4255
 1	10171571	rs114817195	C	T			0.128	0.1571	0.415
 1	10171741	rs116148775	G	A			-0.0482	0.0508	0.343
 1	10171831	rs148366536	G	A			0.1479	0.1572	0.3469
 1	10172650	rs11808311	G	A			0.0369	0.0467	0.4287
 1	10173140	rs79271891	T	A			-0.1267	0.1595	0.4268
 1	10173378	rs142972445	G	C			-0.2072	0.0998	0.03789
-1	10173837	rs1403388296	C	CT			0.0483	0.0508	0.3416
+1	10173837	rs199707934	C	CT			0.0483	0.0508	0.3416
 1	10174189	rs4543799	G	A			-0.0169	0.0244	0.488
 1	10175384	rs147650975	G	T			0.0487	0.0472	0.3022
 1	10175610	rs116458741	T	A			-0.0487	0.0507	0.3375
 1	10175982	rs75225462	G	A			0.0024	0.0647	0.9705
 1	10176608	rs76862201	G	A			-0.05	0.0507	0.3239
 1	10176994	rs140545247	G	A			-0.0661	0.0878	0.4518
 1	10177790	rs3762290	G	A			0.0174	0.0242	0.4722
@@ -623,15 +623,15 @@
 1	10214443	rs78737349	T	A			0.0256	0.048	0.5937
 1	10214805	rs72864116	C	T			0.0258	0.0543	0.6341
 1	10215183	rs115983170	G	T			0.0446	0.0502	0.374
 1	10215207	rs12122985	G	C			0.0262	0.045	0.5611
 1	10215291	rs76119640	G	C			0.0454	0.0865	0.5997
 1	10216027	rs116800840	G	T			-0.0069	0.0463	0.8811
 1	10216068	rs146866855	C	A			0.1063	0.1562	0.4962
-1	10216246	rs1301170807	GA	G			-0.0344	0.0401	0.3921
+1	10216246	rs143137503	GA	G			-0.0344	0.0401	0.3921
 1	10216390	rs7522444	G	C			0.0365	0.0402	0.3645
 1	10216391	rs61782933	G	A			-0.0257	0.0966	0.7905
 1	10216545	rs145909236	G	A			0.0463	0.05	0.3549
 1	10216859	rs79015239	G	T			0.0969	0.1562	0.535
 1	10217086	rs79286153	T	A			0.043	0.0498	0.3873
 1	10217218	rs139505257	G	A			-0.3046	0.2614	0.2439
 1	10217268	rs115486804	G	A			-0.0478	0.0501	0.3406
@@ -705,15 +705,15 @@
 1	10234125	rs115992551	T	A			0.0254	0.0498	0.6105
 1	10234359	rs191002648	G	A			0.1254	0.1193	0.2931
 1	10234529	rs11121525	C	T			-0.0124	0.025	0.6183
 1	10234588	rs11806008	G	A			-0.0145	0.025	0.5617
 1	10234708	rs35252601	C	T			0.1835	0.1404	0.1913
 1	10235313	rs79982090	C	T			0.0148	0.0519	0.7758
 1	10235435	rs193209561	C	T			-0.0551	0.162	0.734
-1	10235438	rs34575664	G	A			-0.1277	0.046	0.005449
+1	10235438	rs74605718	G	A			-0.1277	0.046	0.005449
 1	10235525	rs188532332	C	T			0.0185	0.0892	0.836
 1	10235712	rs7354817	T	A			-0.0048	0.0171	0.778
 1	10235736	rs12129751	T	A			-0.0114	0.0374	0.7593
 1	10235946	rs2180184	C	T			0.0114	0.0171	0.5054
 1	10235961	rs114189111	T	A			-0.0891	0.1739	0.6085
 1	10235968	rs115384680	G	A			0.1298	0.0936	0.1657
 1	10236039	rs6541080	G	A			-0.0095	0.0167	0.568
@@ -773,15 +773,15 @@
 1	10253036	rs6660928	G	A			-0.0012	0.0172	0.9461
 1	100000012	rs10875231	G	T			-0.0355	0.019	0.06185
 1	100000827	rs6678176	C	T			-0.0456	0.0176	0.009574
 1	100000843	rs78286437	C	T			0.0697	0.0372	0.06129
 1	100000989	rs146963890	ATC	A			0.0695	0.0388	0.07307
 1	100001138	rs144406489	G	A			-0.0328	0.0576	0.5698
 1	100001201	rs76909621	G	T			-0.0265	0.0272	0.33
-1	100002155	rs762760390	GTTAGT	G			-0.0249	0.0278	0.3695
+1	100002155	rs147727421	GTTAGT	G			-0.0249	0.0278	0.3695
 1	100002490	rs78642210	C	T			-0.0743	0.0367	0.04278
 1	100002713	rs77140576	C	T			-0.0316	0.027	0.2426
 1	100002714	rs113470118	G	A			0.0774	0.0373	0.03806
 1	100002882	rs7545818	G	T			0.0455	0.0176	0.009816
 1	100002991	rs75635821	G	A			-0.029	0.0271	0.2858
 1	100003204	rs78948828	G	T			0.0769	0.0373	0.03923
 1	100003419	rs114427610	C	T			0.0352	0.0474	0.4579
@@ -822,15 +822,15 @@
 1	100012384	rs74385136	G	C			-0.0694	0.0364	0.05683
 1	100012794	rs12059609	G	A			0.0266	0.0234	0.2561
 1	100012891	rs115410119	G	A			-0.0754	0.0366	0.03956
 1	100012917	rs186620577	G	T			0.2572	0.1765	0.145
 1	100013279	rs17120646	C	T			-0.0274	0.0234	0.2429
 1	100013600	rs17404017	T	A			-0.046	0.058	0.4272
 1	100013724	rs114190542	G	A			-0.0765	0.0367	0.0373
-1	100013848	rs889355602	TTTG	T			-0.1129	0.1909	0.5542
+1	100013848	rs200344241	TTTG	T			-0.1129	0.1909	0.5542
 1	100014490	rs76335995	G	T			0.0246	0.0264	0.3524
 1	100015192	rs35907285	C	CT			-0.0212	0.0221	0.3373
 1	100015354	rs2392044	G	A			-0.044	0.0176	0.01257
 1	100015373	rs2392043	C	T			0.0444	0.0176	0.01179
 1	100015528	rs11166270	G	A			-0.0455	0.0176	0.009802
 1	100015703	rs17404045	C	T			0.0263	0.0164	0.1083
 1	100015728	rs76835333	G	A			-0.0209	0.0274	0.4458
@@ -893,15 +893,15 @@
 1	100031574	rs17120680	C	T			0.1099	0.0386	0.004443
 1	100031734	rs76075449	C	T			0.0331	0.0374	0.3772
 1	100032054	rs77406825	C	T			0.0261	0.0371	0.4819
 1	100032277	rs115829890	C	T			-0.2815	0.1226	0.02165
 1	100032527	rs2027357	G	C			-0.0009	0.018	0.9601
 1	100032836	rs7513849	G	A			-0.0012	0.0179	0.9449
 1	100033364	rs1890754	G	T			-0.0078	0.0174	0.6532
-1	100033517	rs150891802	GA	G			0.0597	0.0428	0.1629
+1	100033517	rs35382957	GA	G			0.0597	0.0428	0.1629
 1	100034143	rs76922334	G	C			0.0673	0.0974	0.4898
 1	100034766	rs141027395	C	T			0.0314	0.2115	0.8822
 1	100035028	rs66698137	C	T			0.0613	0.0429	0.1535
 1	100035200	rs76877570	G	A			-0.049	0.0386	0.204
 1	100035346	rs114562369	G	C			-0.0814	0.0815	0.3178
 1	100035395	rs1339859	G	A			0.0323	0.0386	0.403
 1	100036060	rs4581299	T	A			-0.0024	0.0168	0.8846
@@ -1038,15 +1038,15 @@
 1	100065413	rs57850168	C	T			-0.0122	0.0387	0.752
 1	100065568	rs7536479	G	A			0.0221	0.0216	0.3075
 1	100065823	rs114323737	G	A			0.0809	0.0606	0.1815
 1	100066094	rs882982	G	A			-0.0002	0.0171	0.9919
 1	100067082	rs114691320	C	A			0.0522	0.0458	0.2543
 1	100067690	rs71659202	G	T			0.0497	0.0757	0.5116
 1	100067902	rs4908329	C	T			-0.0036	0.0165	0.8291
-1	100068864	rs1040842402	TC	T			-0.0083	0.0267	0.755
+1	100068864	rs34504219	TC	T			-0.0083	0.0267	0.755
 1	100068912	rs12406024	C	T			0.0061	0.019	0.7485
 1	100069554	rs6678322	T	A			-0.0002	0.0163	0.9908
 1	100069727	rs115029389	C	T			-0.0606	0.0448	0.1757
 1	100069801	rs12025301	G	A			0.0084	0.0243	0.7289
 1	100070039	rs79159903	G	A			-0.0657	0.0446	0.1408
 1	100070074	rs190574074	C	T			-0.0155	0.1562	0.9211
 1	100070931	rs12749229	G	A			0.0079	0.0243	0.7447
@@ -1108,15 +1108,15 @@
 1	100087162	rs834979	G	A			0.0204	0.0195	0.2948
 1	100087539	rs11166284	T	A			0.0077	0.0163	0.6358
 1	100088022	rs12036093	G	A			0.0376	0.0752	0.6168
 1	100088186	rs834978	G	A			-0.0213	0.0197	0.2794
 1	100088517	rs34781954	C	T			-0.0266	0.0293	0.3642
 1	100088528	rs116315008	G	A			0.0638	0.0449	0.1549
 1	100088531	rs834977	G	C			-0.0077	0.0187	0.6803
-1	100088590	rs144907696	AAC	A			-0.0027	0.0234	0.9093
+1	100088590	rs35784659	AAC	A			-0.0027	0.0234	0.9093
 1	100088697	rs140529105	C	T			0.0636	0.0447	0.1548
 1	100090180	rs57734683	T	A			0.0428	0.047	0.3625
 1	100090493	rs115213840	C	T			0.0057	0.0416	0.8917
 1	100090761	rs192122552	C	T			0.0308	0.1529	0.8405
 1	100090958	rs200873961	GGTGTATTAGAT	G			0.0799	0.1255	0.5241
 1	100090999	rs17405380	G	A			-0.0499	0.031	0.1073
 1	100091422	rs77409183	C	T			-0.0314	0.036	0.3833
@@ -1170,25 +1170,25 @@
 1	100103934	rs11166285	C	T			-0.0017	0.0238	0.9419
 1	100104030	rs181737949	C	T			-0.1061	0.1154	0.3581
 1	100104759	rs75957230	T	A			-0.1405	0.1242	0.258
 1	100105385	rs834961	G	A			-0.0057	0.0182	0.7542
 1	100105433	rs115284829	G	A			0.0695	0.0484	0.1508
 1	100105818	rs834960	G	T			0.0078	0.0238	0.7428
 1	100106063	rs67438058	T	A			-0.0043	0.0237	0.8549
-1	100106308	rs748090947	GT	G			0.0797	0.0498	0.1092
+1	100106308	rs200860825	GT	G			0.0797	0.0498	0.1092
 1	100107021	rs835003	C	T			0.0065	0.0237	0.7835
 1	100107260	rs17405754	C	T			0.0049	0.016	0.7591
 1	100107407	rs835002	C	T			-0.0065	0.0238	0.7859
 1	100108187	rs68031125	C	T			0.0027	0.0237	0.9086
 1	100108661	rs12743626	G	C			0.0093	0.0233	0.6881
 1	100108685	rs835000	C	T			0.0087	0.0234	0.7086
 1	100108794	rs834999	G	T			-0.0086	0.0234	0.7134
 1	100108802	rs77673766	G	C			-0.0432	0.0852	0.6124
 1	100108831	rs1338573	G	C			0.0017	0.0237	0.9435
-1	100109052	rs1029354296	C	CA			0.0089	0.0233	0.7036
+1	100109052	rs5776481	C	CA			0.0089	0.0233	0.7036
 1	100109414	rs834998	G	A			0.0093	0.0234	0.6901
 1	100109782	rs114574535	C	T			0.0908	0.0503	0.07121
 1	100109869	rs115040600	T	A			-0.0842	0.0511	0.09967
 1	100109949	rs7550217	G	T			0.0058	0.0234	0.8037
 1	100109996	rs200126406	AT	A			0.0021	0.0726	0.9769
 1	100111425	rs116419334	G	A			0.0136	0.1032	0.8952
 1	100111956	rs834997	G	A			0.0098	0.0181	0.5901
@@ -1251,33 +1251,33 @@
 1	100138226	rs191435206	G	A			-0.1641	0.1219	0.1783
 1	100138827	rs55840341	AT	A			-0.1266	0.0376	0.000772
 1	100139143	rs61784993	C	A			-0.0066	0.017	0.6959
 1	100139291	rs12035402	C	A			0.0392	0.0418	0.3481
 1	100139730	rs7524870	C	T			0.0227	0.022	0.3017
 1	100140414	rs4908003	T	A			0.0628	0.0364	0.08407
 1	100140509	rs7549467	G	A			-0.1446	0.1852	0.4349
-1	100140638	rs142337711	C	CTA			0.1333	0.177	0.4513
+1	100140638	rs10585286	C	CTA			0.1333	0.177	0.4513
 1	100140890	rs12747606	C	A			-0.0514	0.0676	0.4467
 1	100142183	rs12025746	G	A			0.0367	0.0416	0.3777
-1	100142339	rs938981076	TA	T			0.0384	0.0418	0.3582
+1	100142339	rs71708491	TA	T			0.0384	0.0418	0.3582
 1	100142436	rs12058890	G	A			0.1261	0.184	0.4932
 1	100142481	rs12022677	T	A			-0.0406	0.0417	0.3296
 1	100142586	rs12063713	G	C			-0.1275	0.1842	0.489
 1	100142602	rs12063715	G	A			-0.1217	0.1841	0.5085
 1	100142648	rs76085216	G	T			-0.1216	0.184	0.5089
 1	100142667	rs78270457	T	A			-0.1216	0.184	0.5089
 1	100142791	rs201013610	TC	T			0.1171	0.1839	0.5244
 1	100143040	rs11166290	C	T			-0.1187	0.1839	0.5185
 1	100143062	rs11166291	G	A			0.1214	0.1841	0.5095
 1	100143163	rs6577118	C	T			0.0321	0.0681	0.6378
 1	100143392	rs11166292	G	A			-0.1179	0.1839	0.5213
 1	100143458	rs1981193	G	A			0.0169	0.0167	0.3139
 1	100143603	rs1981192	G	T			-0.0128	0.0165	0.4394
 1	100143653	rs1338577	G	T			0.0115	0.0173	0.5075
-1	100143796	rs866882343	TTA	T			-0.118	0.1839	0.521
+1	100143796	rs142661105	TTA	T			-0.118	0.1839	0.521
 1	100144221	rs200532959	C	CA			-0.0248	0.0541	0.6465
 1	100144226	rs150940722	C	T			-0.1413	0.139	0.3091
 1	100144363	rs7540358	C	T			-0.0104	0.0173	0.5462
 1	100144598	rs150120519	G	A			0.0407	0.0921	0.6583
 1	100144727	rs75454387	C	T			-0.1414	0.1842	0.4426
 1	100144728	rs181159932	G	A			-0.3525	0.2556	0.1679
 1	100145028	rs17120889	G	C			-0.0402	0.0417	0.3349
@@ -1323,15 +1323,15 @@
 1	100149918	rs6698880	G	A			0.0017	0.049	0.973
 1	100149952	rs12136177	C	T			-0.0747	0.0393	0.05749
 1	100150022	rs12126052	C	T			0.0737	0.0393	0.06054
 1	100150077	rs6701684	C	T			0.0128	0.0478	0.7893
 1	100150097	rs112057007	TTTTG	T			0.0194	0.0535	0.7166
 1	100150121	rs11166294	C	T			-0.0028	0.0485	0.954
 1	100150499	rs11166295	C	A			0.0176	0.0474	0.7101
-1	100150722	rs1023074022	ATCTG	A			-0.017	0.0473	0.7191
+1	100150722	rs71679248	ATCTG	A			-0.017	0.0473	0.7191
 1	100150824	rs1890410	G	A			0.0177	0.0472	0.7072
 1	100151037	rs1890409	G	A			0.0188	0.0473	0.6916
 1	100151103	rs17120904	C	T			-0.0743	0.0393	0.0585
 1	100151397	rs12124956	G	A			-0.0736	0.0392	0.06074
 1	100151476	rs11166296	G	C			0.0178	0.0473	0.7058
 1	100151586	rs11166297	G	A			0.0167	0.0473	0.7238
 1	100151691	rs12132726	G	C			0.0737	0.0393	0.06059
@@ -1412,15 +1412,15 @@
 1	100175242	rs12135581	G	A			0.0535	0.0409	0.1908
 1	100175373	rs72956489	C	A			0.0525	0.0409	0.1999
 1	100175621	rs12139029	G	A			-0.0523	0.0412	0.2049
 1	100175698	rs12139063	G	T			-0.0494	0.0418	0.2371
 1	100175758	rs12135762	G	A			0.0421	0.0421	0.3175
 1	100175764	rs12139091	G	A			-0.0395	0.0421	0.3477
 1	100175766	rs12117081	C	A			-0.0333	0.0418	0.4254
-1	100175909	rs113724705	TCTGG	T			0.0527	0.0409	0.1976
+1	100175909	rs113503212	TCTGG	T			0.0527	0.0409	0.1976
 1	100176084	rs12117907	C	A			-0.0532	0.0409	0.1941
 1	100176834	rs147448322	C	T			0.0009	0.064	0.989
 1	100177184	rs190461581	G	A			0.1256	0.1595	0.4311
 1	100177273	rs147690820	C	A			0.0185	0.1083	0.8646
 1	100177526	rs12141159	G	A			-0.06	0.0415	0.1484
 1	100177723	rs41285732	C	T			0.1482	0.0954	0.1202
 1	100178708	rs72956490	C	A			0.0579	0.0412	0.16
@@ -1582,15 +1582,15 @@
 1	100211444	rs7545648	G	C			-0.033	0.0172	0.05488
 1	100211841	rs10875251	C	T			0.0982	0.1145	0.391
 1	100212553	rs1591775	C	T			0.0235	0.017	0.1664
 1	100213113	rs148199377	T	A			-0.0749	0.0964	0.437
 1	100213115	rs6577132	C	T			-0.0235	0.017	0.1654
 1	100213466	rs7528854	G	T			0.0247	0.017	0.1458
 1	100213741	rs189501640	C	T			0.0901	0.1593	0.5718
-1	100213907	rs763242199	AG	A			-0.0141	0.03	0.6382
+1	100213907	rs61004190	AG	A			-0.0141	0.03	0.6382
 1	100214391	rs1416237	T	A			0.0243	0.017	0.1519
 1	100214487	rs1416236	C	T			0.0249	0.017	0.1415
 1	100214578	rs1416235	G	A			0.0365	0.0195	0.06141
 1	100214634	rs4908016	C	T			-0.0179	0.03	0.5514
 1	100214694	rs149645321	G	T			0.0732	0.0959	0.445
 1	100214725	rs10158169	G	A			0.0241	0.017	0.156
 1	100214777	rs11166324	G	C			0.0366	0.0195	0.06083
@@ -1681,23 +1681,23 @@
 1	100237108	rs34504716	G	A			0.0197	0.0467	0.6738
 1	100237542	rs11166329	G	T			0.0362	0.0185	0.05018
 1	100238053	rs12094925	C	T			-0.0173	0.03	0.5635
 1	100239135	rs61783017	G	T			-0.0499	0.0417	0.231
 1	100239486	rs4908019	C	A			-0.0171	0.03	0.5681
 1	100240050	rs12038936	G	A			-0.0352	0.0186	0.05801
 1	100240070	rs12039637	G	A			-0.0366	0.0186	0.04871
-1	100240247	rs757147902	AAGT	A			-0.0108	0.0299	0.7175
+1	100240247	rs71698804	AAGT	A			-0.0108	0.0299	0.7175
 1	100241763	rs9729152	C	T			0.0363	0.0186	0.05059
 1	100242048	rs10875257	C	A			0.0093	0.0299	0.7554
 1	100242497	rs12039676	G	T			0.0367	0.0188	0.05125
 1	100242500	rs12046903	G	C			-0.0364	0.0188	0.05291
 1	100242635	rs4908022	C	A			-0.024	0.017	0.1569
 1	100243664	rs12568896	C	A			-0.0282	0.0171	0.1003
 1	100243895	rs4907889	C	T			0.0264	0.0171	0.1234
-1	100243972	rs777766212	GAAGAT	G			-0.0115	0.0299	0.7007
+1	100243972	rs146916256	GAAGAT	G			-0.0115	0.0299	0.7007
 1	100244236	rs4907890	C	A			0.0147	0.03	0.6246
 1	100244302	rs4907891	C	T			-0.0273	0.0172	0.1123
 1	100244371	rs72723782	G	A			-0.1082	0.0539	0.04462
 1	100244581	rs17121179	G	T			-0.0292	0.0171	0.08848
 1	100244929	rs35277688	G	A			0.0255	0.0484	0.5981
 1	100245597	rs12561837	C	T			-0.026	0.0171	0.1297
 1	100246110	rs150357261	C	A			-0.033	0.0573	0.5645
@@ -1714,15 +1714,15 @@
 1	100249550	rs931519	C	A			0.0055	0.0253	0.828
 1	100250197	rs931520	G	A			0.0662	0.0336	0.04897
 1	100250208	rs114555778	C	T			-0.0179	0.0616	0.7716
 1	100250226	rs17121189	G	A			0.0604	0.0358	0.09217
 1	100250522	rs12749851	G	A			0.0196	0.0467	0.6752
 1	100250586	rs12749991	G	A			0.0163	0.0487	0.7381
 1	100250863	rs72723788	G	T			0.0986	0.054	0.06791
-1	100251575	rs1382716835	C	CA			0.0324	0.0268	0.2278
+1	100251575		C	CA			0.0324	0.0268	0.2278
 1	100251818	rs150726939	C	T			-0.0052	0.1114	0.963
 1	100252145	rs12137801	C	T			0.024	0.0271	0.377
 1	100252217	rs10875258	C	T			-0.0414	0.0815	0.6117
 1	100252387	rs72723789	C	T			0.0267	0.0237	0.2597
 1	100252863	rs201733676	TTTTTC	T			0.1113	0.0549	0.04255
 1	100253103	rs966579	C	A			-0.0198	0.0172	0.2493
 1	100253142	rs116595337	T	A			0.133	0.0637	0.0368
@@ -1749,15 +1749,15 @@
 1	100258529	rs1979709	G	C			-0.0049	0.0167	0.7704
 1	100259555	rs182936914	G	A			0.15	0.1319	0.2554
 1	100259643	rs12732878	C	T			0.0857	0.0398	0.03127
 1	100259720	rs1976249	G	C			-0.0291	0.0221	0.1881
 1	100259754	rs1976250	G	C			-0.0292	0.0221	0.1856
 1	100260019	rs10159242	C	A			-0.1038	0.0544	0.05626
 1	100260307	rs6701853	C	A			-0.0016	0.0167	0.9258
-1	100260408	rs942941986	GT	G			-0.0688	0.0274	0.01191
+1	100260408	rs36169233	GT	G			-0.0688	0.0274	0.01191
 1	100260640	rs36185331	G	T			-0.0397	0.0304	0.1905
 1	100260805	rs141651484	C	T			-0.1029	0.0543	0.05787
 1	100260844	rs116823926	T	A			-0.0079	0.0564	0.888
 1	100260945	rs60154241	C	T			0.054	0.0243	0.02605
 1	100261125	rs9728927	G	T			-0.0325	0.0197	0.09814
 1	100261148	rs200023968	GT	G			0.1024	0.0543	0.05924
 1	100261604	rs112965759	G	A			-0.0417	0.0303	0.168
@@ -1886,15 +1886,15 @@
 1	100282966	rs72725923	C	T			0.091	0.0541	0.09211
 1	100283708	rs143904320	C	T			-0.0494	0.0946	0.6019
 1	100284575	rs144239734	T	A			-0.0778	0.0758	0.3047
 1	100284982	rs190266457	G	A			0.745	0.2676	0.005361
 1	100285072	rs188193051	C	T			-0.0173	0.0938	0.8537
 1	100285168	rs34896283	C	T			-0.0171	0.0171	0.3174
 1	100285446	rs6669386	G	A			0.0203	0.0166	0.2217
-1	100285675	rs565237870	GA	G			0.0134	0.0975	0.891
+1	100285675	rs201953466	GA	G			0.0134	0.0975	0.891
 1	100285720	rs6680760	G	C			-0.0185	0.0166	0.2658
 1	100286036	rs6657345	C	T			-0.0172	0.0166	0.2999
 1	100286199	rs4908028	G	C			0.0911	0.054	0.09181
 1	100286234	rs4907896	C	T			0.0178	0.0166	0.284
 1	100286552	rs3920022	T	A			-0.0093	0.0169	0.5832
 1	100286604	rs79675270	G	A			-0.0444	0.0392	0.2573
 1	100286774	rs151196013	C	A			0.0807	0.0611	0.1866
@@ -2010,15 +2010,15 @@
 1	100320046	rs12744819	C	T			0.0696	0.0848	0.4119
 1	100320084	rs6701460	C	T			-0.0252	0.0213	0.2356
 1	100320260	rs146647362	C	T			-0.0496	0.0633	0.4331
 1	100320435	rs72725944	G	A			0.0144	0.0347	0.678
 1	100320706	rs146811455	G	A			0.0685	0.0636	0.2812
 1	100321029	rs143536494	C	T			-0.0714	0.0601	0.2347
 1	100321314	rs185911921	G	A			-0.0278	0.1863	0.8815
-1	100321975	rs1386565489	C	CTTTCT			0.0101	0.0626	0.8717
+1	100321975	rs199914213	C	CTTTCT			0.0101	0.0626	0.8717
 1	100322135	rs7526847	G	A			0.0793	0.068	0.2439
 1	100322255	rs144763873	G	A			0.0764	0.0606	0.2075
 1	100322347	rs148557268	G	C			-0.1166	0.0538	0.03038
 1	100322381	rs141970507	C	T			-0.0041	0.0735	0.956
 1	100322478	rs186911941	G	A			-0.0816	0.0601	0.1743
 1	100322574	rs190405644	T	A			0.0705	0.0616	0.2521
 1	100322583	rs684047	C	T			-0.0022	0.0162	0.8918
@@ -2126,15 +2126,15 @@
 1	100343073	rs2291637	T	A			-0.0254	0.016	0.1128
 1	100343153	rs2291638	G	A			0.0311	0.0166	0.06066
 1	100343254	rs141043166	G	A			0.0213	0.0811	0.7929
 1	100343778	rs11166363	G	A			0.0293	0.0161	0.06786
 1	100344312	rs3753490	G	T			0.0066	0.0225	0.7687
 1	100344394	rs3753491	G	A			-0.0239	0.0161	0.1371
 1	100344496	rs3753492	G	A			0.0452	0.0373	0.2258
-1	100344919	rs773308235	TC	T			-0.0069	0.0225	0.7581
+1	100344919	rs142035948	TC	T			-0.0069	0.0225	0.7581
 1	100345409	rs2392077	G	C			0.0257	0.016	0.1083
 1	100345455	rs115666491	C	A			-0.0393	0.0698	0.5733
 1	100345825	rs11166364	G	A			0.0593	0.075	0.429
 1	100345975	rs12035706	C	T			-0.0427	0.0374	0.2545
 1	100346741	rs3736296	C	T			0.0287	0.016	0.07308
 1	100347419	rs76321904	C	T			-0.0685	0.067	0.3062
 1	100347463	rs1389381	C	A			-0.0078	0.0225	0.7288
@@ -2197,15 +2197,15 @@
 1	100365560	rs138672978	G	A			-0.0764	0.0597	0.2007
 1	100365677	rs11166370	G	C			0.0297	0.016	0.06419
 1	100365797	rs2769699	C	T			-0.0392	0.0171	0.02145
 1	100365848	rs17121583	C	T			-0.0685	0.0557	0.2183
 1	100365849	rs12734255	G	A			0.042	0.0596	0.4809
 1	100366141	rs572231	G	A			0.0359	0.0697	0.6065
 1	100366982	rs116352317	G	T			-0.062	0.0613	0.3121
-1	100367317	rs1356371251	TG	T			-0.0322	0.0701	0.6455
+1	100367317	rs200158049	TG	T			-0.0322	0.0701	0.6455
 1	100367379	rs2769698	C	T			0.038	0.0161	0.01793
 1	100367386	rs139393425	ATATT	A			0.0746	0.056	0.1828
 1	100367728	rs141673830	C	CTGAG			-0.036	0.0481	0.4541
 1	100367891	rs659030	G	A			-0.0585	0.0345	0.0903
 1	100368382	rs834575	C	T			0.0605	0.0393	0.1232
 1	100368640	rs17121609	G	A			0.024	0.0161	0.1359
 1	100368888	rs74540181	G	A			-0.0032	0.0225	0.8884
@@ -2234,15 +2234,15 @@
 1	100375209	rs7552875	T	A			-0.0433	0.0171	0.01134
 1	100375347	rs12039074	G	A			0.0214	0.0161	0.1822
 1	100375407	rs67893284	G	A			0.0013	0.0225	0.9528
 1	100375408	rs115202423	G	A			-0.0607	0.0541	0.262
 1	100375580	rs12039154	G	A			0.023	0.0161	0.1528
 1	100376448	rs2274570	G	A			-0.0344	0.016	0.03159
 1	100376456	rs1541041	T	A			-0.0347	0.016	0.03005
-1	100376943	rs757823341	AAT	A			-0.0019	0.0225	0.931
+1	100376943	rs34936033	AAT	A			-0.0019	0.0225	0.931
 1	100377295	rs77905995	G	A			0.0333	0.0475	0.4835
 1	100377443	rs148473095	G	A			0.0301	0.0682	0.6593
 1	100377744	rs17121622	C	T			0.0626	0.0392	0.1101
 1	100377789	rs3818568	C	T			-0.0019	0.0225	0.932
 1	100377894	rs190328362	G	A			0.1514	0.2099	0.4708
 1	100377973	rs28730706	C	T			0.0413	0.0681	0.5443
 1	100378367	rs6692695	T	A			0.0227	0.0161	0.1578
@@ -2350,15 +2350,15 @@
 1	100410444	rs116524536	C	T			-0.0396	0.1086	0.7154
 1	100410458	rs11166379	C	A			0.0024	0.0448	0.9569
 1	100410636	rs2149193	G	A			-0.0204	0.0164	0.214
 1	100411287	rs1541044	C	T			-0.0126	0.0221	0.5692
 1	100412034	rs11317846	GA	G			-0.0677	0.0391	0.08344
 1	100412250	rs147652927	G	C			0.0561	0.0678	0.4078
 1	100412320	rs76403172	G	A			-0.0707	0.0392	0.07151
-1	100413062	rs865898108	GAT	G			-0.022	0.0556	0.6918
+1	100413062	rs200624013	GAT	G			-0.022	0.0556	0.6918
 1	100413075	rs12117631	C	A			-0.0033	0.0448	0.9412
 1	100413213	rs6694655	C	T			-0.0243	0.0163	0.1372
 1	100413246	rs116210755	G	A			-0.0242	0.0563	0.6669
 1	100413698	rs80115574	C	T			0.0725	0.0391	0.06408
 1	100414049	rs6661865	G	A			0.0656	0.0393	0.09512
 1	100414740	rs1571351	C	T			-0.0397	0.0175	0.02352
 1	100415553	rs145889827	G	A			-0.0435	0.0677	0.5203
@@ -2376,17 +2376,17 @@
 1	100417765	rs7364413	G	A			0.0472	0.0181	0.008871
 1	100417773	rs114008113	C	T			-0.0236	0.0373	0.5263
 1	100418080	rs12066300	C	A			-0.0198	0.0376	0.5986
 1	100419288	rs149658721	G	A			-0.0696	0.0391	0.07523
 1	100419556	rs7518805	G	A			-0.0126	0.0199	0.5244
 1	100419867	rs7521627	C	T			-0.0118	0.0199	0.5538
 1	100419898	rs146634653	C	CA			0.0048	0.0973	0.9608
-1	100420015	rs1481644823	GA	G			0.0207	0.0375	0.5808
+1	100420015	rs139219470	GA	G			0.0207	0.0375	0.5808
 1	100420049	rs7529633	G	A			0.0071	0.022	0.7487
-1	100420055	rs1179675204	TA	T			-0.05	0.0676	0.4593
+1	100420055	rs200139033	TA	T			-0.05	0.0676	0.4593
 1	100420287	rs114979382	C	T			-0.0661	0.0566	0.2425
 1	100420330	rs192423871	T	A			-0.065	0.2945	0.8254
 1	100420559	rs12128514	G	A			-0.0235	0.0379	0.5351
 1	100421285	rs7525268	T	A			0.0064	0.0328	0.8447
 1	100421591	rs56232549	C	T			0.0622	0.0947	0.5112
 1	100421918	rs12078506	C	T			0.0038	0.0329	0.9074
 1	100421945	rs187080892	C	T			-0.0925	0.104	0.3734
@@ -2417,15 +2417,15 @@
 1	100426671	rs12071626	T	A			0.0101	0.033	0.7594
 1	100426672	rs6701353	T	A			0.0668	0.0384	0.08151
 1	100426978	rs6701658	G	A			-0.0038	0.0329	0.9091
 1	100427268	rs183407568	G	A			-0.0055	0.1056	0.9587
 1	100427400	rs116116174	G	C			0.0028	0.033	0.932
 1	100427467	rs148928085	TTTAAA	T			0.0209	0.0379	0.5826
 1	100427640	rs193061855	G	A			-0.0097	0.1022	0.9243
-1	100427756	rs780335412	TTTAAATA	T			-0.0707	0.039	0.07001
+1	100427756	rs143767524	TTTAAATA	T			-0.0707	0.039	0.07001
 1	100427787	rs76090318	C	T			-0.0703	0.039	0.07163
 1	100427842	rs6667554	G	C			-0.0145	0.0173	0.4005
 1	100427856	rs187960034	G	A			-0.0448	0.0676	0.5079
 1	100428242	rs115996005	C	T			0.0467	0.0845	0.5807
 1	100428752	rs79122115	T	A			-0.0604	0.1241	0.6266
 1	100428761	rs1541043	C	T			-0.003	0.0198	0.881
 1	100428784	rs11166382	C	A			0.0025	0.0198	0.899
@@ -2571,15 +2571,15 @@
 1	100470502	rs144653792	G	A			-0.0638	0.0391	0.1032
 1	100470665	rs142789523	G	A			-0.054	0.0693	0.4363
 1	100470789	rs190902725	C	T			0.2333	0.2785	0.4021
 1	100470844	rs481660	G	A			-0.0711	0.0388	0.06662
 1	100470878	rs139697691	G	T			0.055	0.0693	0.4274
 1	100470955	rs11805704	C	T			-0.0175	0.0377	0.6422
 1	100471243	rs11166392	G	A			0.0204	0.0374	0.5855
-1	100471378	rs960766735	C	CT			0.0456	0.0689	0.5087
+1	100471378	rs200521707	C	CT			0.0456	0.0689	0.5087
 1	100471566	rs564562	C	T			0.0469	0.0259	0.07076
 1	100472358	rs114485948	C	T			0.054	0.0694	0.4362
 1	100472604	rs534252	G	A			0.0277	0.0221	0.2107
 1	100473283	rs201494624	GTC	G			-0.0597	0.0693	0.389
 1	100473306	rs113658116	G	A			0.0519	0.1125	0.6444
 1	100473361	rs79969776	C	T			-0.0548	0.0694	0.4299
 1	100473427	rs526128	T	A			-0.0277	0.0221	0.2118
@@ -2630,15 +2630,15 @@
 1	100484824	rs115233992	G	T			-0.0541	0.0693	0.4356
 1	100485537	rs80194374	G	C			0.0544	0.0694	0.4332
 1	100485624	rs11166394	C	A			0.0172	0.0376	0.6472
 1	100485988	rs531174	G	T			-0.0485	0.026	0.06221
 1	100486485	rs148246061	G	A			0.2228	0.1121	0.04691
 1	100487421	rs510370	C	T			0.0701	0.0391	0.07299
 1	100487529	rs115458903	C	T			0.0575	0.0693	0.407
-1	100487702	rs761378588	C	CAT			0.0731	0.0386	0.05846
+1	100487702	rs142913547	C	CAT			0.0731	0.0386	0.05846
 1	100487763	rs115532474	C	A			0.0581	0.0693	0.4021
 1	100488044	rs76983464	C	T			-0.097	0.1039	0.3506
 1	100488177	rs482466	C	T			-0.0256	0.0221	0.2466
 1	100489128	rs12129713	G	T			0.0196	0.0377	0.6041
 1	100489264	rs561735	C	A			-0.0689	0.039	0.07766
 1	100490151	rs145699799	G	A			0.0573	0.07	0.4129
 1	100490410	rs147661822	C	T			-0.0517	0.0696	0.4579
@@ -2659,15 +2659,15 @@
 1	100493934	rs115495492	G	C			0.0701	0.0391	0.07291
 1	100494644	rs145659310	G	A			-0.1017	0.1902	0.593
 1	100494652	rs511487	G	A			0.0731	0.0386	0.05869
 1	100494686	rs116560578	C	T			0.0619	0.0692	0.3712
 1	100495392	rs568089	C	T			0.0497	0.026	0.0559
 1	100497091	rs510463	G	T			0.0701	0.039	0.0723
 1	100497358	rs114665354	T	A			0.0652	0.0688	0.3435
-1	100497672	rs142850619	AATTG	A			0.0283	0.0221	0.2009
+1	100497672	rs57056028	AATTG	A			0.0283	0.0221	0.2009
 1	100498035	rs12143017	C	T			-0.0176	0.0376	0.6394
 1	100498371	rs180934609	G	T			-0.1037	0.1048	0.3224
 1	100498379	rs12136158	G	T			-0.0191	0.0377	0.6123
 1	100498740	rs191467572	G	A			-0.1246	0.2048	0.5429
 1	100498749	rs148811205	G	C			0.0573	0.0693	0.4086
 1	100498969	rs76334301	G	A			0.0174	0.0376	0.643
 1	100499059	rs74888510	C	T			0.0172	0.0377	0.6473
@@ -2680,35 +2680,35 @@
 1	100500482	rs75904885	C	T			-0.0575	0.0697	0.4093
 1	100500675	rs114757369	G	C			0.0553	0.0696	0.4265
 1	100500762	rs12135824	C	T			0.0184	0.0377	0.6249
 1	100500902	rs565662	C	T			-0.0652	0.0391	0.09553
 1	100500915	rs565708	C	A			-0.068	0.0392	0.08278
 1	100502061	rs78501535	T	A			0.0592	0.0693	0.3934
 1	100502690	rs12406605	C	T			0.0247	0.0165	0.1347
-1	100502868	rs115209325	TATAC	T			0.0711	0.039	0.06834
-1	100502995	rs1301028010	C	CTAATTT			-0.0179	0.0371	0.6298
+1	100502868	rs148026087	TATAC	T			0.0711	0.039	0.06834
+1	100502995	rs143635532	C	CTAATTT			-0.0179	0.0371	0.6298
 1	100503163	rs78079041	G	A			-0.0693	0.039	0.07573
 1	100503344	rs79388191	G	A			0.0579	0.0693	0.4032
 1	100503564	rs1109770	C	T			0.0287	0.0221	0.1944
 1	100503875	rs187489161	G	A			-0.0556	0.0694	0.4227
 1	100503892	rs80339334	G	C			-0.0179	0.0377	0.6352
 1	100503993	rs1395332	C	A			0.0278	0.0221	0.209
 1	100504052	rs115488331	C	A			-0.1626	0.1623	0.3164
 1	100504162	rs1395333	C	T			-0.0744	0.0387	0.05433
 1	100504268	rs700529	C	T			-0.0692	0.0387	0.0739
 1	100504272	rs34787051	C	T			0.0142	0.0368	0.6996
 1	100504439	rs78361605	G	A			0.0488	0.0653	0.4545
 1	100504570	rs877245	G	C			0.0154	0.0372	0.6785
 1	100504670	rs74667790	T	A			-0.0558	0.0693	0.4204
-1	100504801	rs1367190242	GAT	G			-0.0171	0.0376	0.6493
+1	100504801	rs66827033	GAT	G			-0.0171	0.0376	0.6493
 1	100505162	rs74871996	G	A			-0.162	0.0855	0.05793
 1	100505332	rs76461538	G	C			-0.055	0.0696	0.4292
 1	100505706	rs559833	T	A			0.0694	0.0342	0.04218
 1	100505721	rs12138063	G	T			-0.0166	0.0376	0.6596
-1	100505866	rs764345607	C	CAG			0.0689	0.0384	0.07302
+1	100505866	rs144403425	C	CAG			0.0689	0.0384	0.07302
 1	100506292	rs11166395	C	A			-0.0178	0.0371	0.6313
 1	100506406	rs186301896	G	A			-0.0826	0.1641	0.6145
 1	100506415	rs555778	G	A			-0.0713	0.0342	0.03682
 1	100507228	rs139504262	G	C			0.0691	0.0391	0.07729
 1	100507286	rs142771822	C	T			-0.0553	0.0687	0.4214
 1	100507380	rs11166396	C	T			0.0186	0.0371	0.6161
 1	100507990	rs496798	G	A			-0.0284	0.0221	0.1986
@@ -2784,15 +2784,15 @@
 1	100528381	rs116143961	C	T			-0.0686	0.0391	0.07922
 1	100528579	rs79493311	C	T			0.0673	0.0392	0.0859
 1	100529210	rs12117112	G	C			-0.0153	0.0376	0.6852
 1	100529330	rs146405546	C	T			0.051	0.053	0.3363
 1	100530122	rs58068806	G	A			0.0681	0.0342	0.0465
 1	100530168	rs483217	G	T			-0.0292	0.0226	0.1955
 1	100530743	rs183733310	G	T			-0.0331	0.0911	0.7159
-1	100531013	rs1225823353	C	CCCTTT			-0.0769	0.0375	0.04034
+1	100531013	rs140999986	C	CCCTTT			-0.0769	0.0375	0.04034
 1	100531432	rs17253615	G	A			-0.0707	0.039	0.07002
 1	100532191	rs191878500	T	A			-0.0587	0.0694	0.3981
 1	100532272	rs834285	G	A			0.0279	0.0222	0.2094
 1	100532320	rs12122332	C	T			0.0603	0.1563	0.6996
 1	100532499	rs140523016	C	A			-0.0656	0.0391	0.09358
 1	100532621	rs142923701	C	T			-0.0816	0.1004	0.4164
 1	100533009	rs141040539	G	T			-0.0579	0.0694	0.404
@@ -2974,26 +2974,26 @@
 1	100590763	rs182860578	G	A			0.0323	0.078	0.6784
 1	100591127	rs57727392	C	T			0.0557	0.0756	0.4616
 1	100591669	rs114057168	C	T			0.036	0.0777	0.6433
 1	100592057	rs74839329	G	A			-0.0681	0.039	0.08069
 1	100592268	rs146081118	G	A			-0.0324	0.0776	0.6764
 1	100592901	rs564938	C	T			-0.0265	0.0223	0.2345
 1	100592925	rs2784178	G	A			-0.017	0.0375	0.6499
-1	100593039	rs752860424	C	CA			-0.0265	0.0222	0.232
+1	100593039	rs35560756	C	CA			-0.0265	0.0222	0.232
 1	100593738	rs11166403	G	C			-0.0213	0.0377	0.5722
 1	100594521	rs2658647	G	A			0.0139	0.0373	0.7093
 1	100594821	rs115191769	C	A			0.0973	0.0574	0.08986
 1	100595154	rs1960059	C	T			-0.0196	0.0377	0.6026
 1	100595831	rs188961878	C	T			0.2431	0.289	0.4002
 1	100595906	rs12125702	C	T			0.1072	0.177	0.5448
 1	100596448	rs2810417	G	A			0.0138	0.0373	0.7118
 1	100596809	rs140439717	C	CA			0.033	0.0285	0.2474
 1	100596890	rs11166404	C	T			0.0209	0.0377	0.5787
 1	100597378	rs148171026	C	T			-0.0001	0.2019	0.9998
-1	100597545	rs796209746	AAAGT	A			-0.0494	0.0751	0.5108
+1	100597545	rs57169801	AAAGT	A			-0.0494	0.0751	0.5108
 1	100598283	rs142029130	G	A			0.0606	0.1584	0.7019
 1	100598299	rs11166405	G	A			0.0198	0.0377	0.5995
 1	100598439	rs55863167	G	C			-0.0602	0.0751	0.4231
 1	100598744	rs141081618	C	T			0.0045	0.1292	0.9725
 1	100598866	rs472498	G	A			0.0313	0.0212	0.1401
 1	100599478	rs72971892	T	A			-0.0535	0.0753	0.4776
 1	100599622	rs12119539	T	A			-0.0214	0.0377	0.5696
@@ -3061,15 +3061,15 @@
 1	100624212	rs593161	G	T			-0.0299	0.0224	0.1833
 1	100624947	rs80221535	G	A			-0.0536	0.121	0.6577
 1	100625127	rs147536410	C	T			-0.0456	0.0779	0.558
 1	100625713	rs75425839	G	A			0.0178	0.0375	0.636
 1	100625934	rs147675956	G	A			0.0481	0.0779	0.5369
 1	100626496	rs185152103	T	A			0.045	0.0783	0.5649
 1	100626504	rs58087587	G	T			0.056	0.0756	0.4588
-1	100626774	rs766848109	C	CAT			0.0244	0.0378	0.5194
+1	100626774	rs66615807	C	CAT			0.0244	0.0378	0.5194
 1	100627408	rs12034019	G	T			0.019	0.037	0.6085
 1	100627685	rs116111086	C	T			-0.0378	0.0776	0.6264
 1	100627774	rs12127181	C	T			0.0218	0.0378	0.5641
 1	100627779	rs79211828	G	A			-0.0241	0.0474	0.6107
 1	100628065	rs12042049	C	T			0.0155	0.0372	0.6765
 1	100628211	rs115625519	T	A			0.0218	0.0377	0.5635
 1	100628311	rs17122001	T	A			0.0266	0.0222	0.2312
@@ -3189,15 +3189,15 @@
 1	100678717	rs11166416	G	A			-0.0297	0.0224	0.1842
 1	100679564	rs6577155	G	A			0.0298	0.0224	0.1824
 1	100681587	rs146249007	G	A			0.0603	0.0782	0.4405
 1	100682244	rs12124225	G	A			-0.0172	0.0378	0.6492
 1	100682912	rs11580205	G	A			0.0299	0.0224	0.1812
 1	100683013	rs11578881	C	T			-0.0277	0.0231	0.2307
 1	100683310	rs10875281	T	A			-0.028	0.0231	0.2257
-1	100683496	rs747933349	TTAGAC	T			0.0281	0.0231	0.2232
+1	100683496	rs58763464	TTAGAC	T			0.0281	0.0231	0.2232
 1	100683627	rs6577156	G	A			-0.03	0.0223	0.1794
 1	100683821	rs6577157	C	T			-0.0299	0.0223	0.1811
 1	100683906	rs6577158	G	T			0.0299	0.0223	0.1806
 1	100684645	rs191429746	C	T			0.1387	0.2712	0.6091
 1	100685131	rs11166417	G	A			-0.0286	0.0223	0.2001
 1	100685266	rs76609629	C	T			-0.0677	0.04	0.09078
 1	100685313	rs11166418	C	A			0.0269	0.0229	0.2406
@@ -3216,15 +3216,15 @@
 1	100690245	rs7526860	G	C			0.0245	0.023	0.2854
 1	100690561	rs6675037	G	A			0.0358	0.0217	0.09979
 1	100690901	rs4536026	G	A			-0.025	0.0229	0.2759
 1	100691245	rs6577159	G	A			0.0276	0.0229	0.2286
 1	100691509	rs4463693	C	T			0.0226	0.023	0.3256
 1	100692416	rs6577160	C	T			-0.0236	0.023	0.3041
 1	100692438	rs6577161	C	T			-0.0235	0.023	0.3058
-1	100692959	rs145026840	C	CATACAGATAGCCCCA			-0.024	0.0229	0.2941
+1	100692959	rs140355478	C	CATACAGATAGCCCCA			-0.024	0.0229	0.2941
 1	100693294	rs6682782	G	A			0.0235	0.0231	0.3087
 1	100694041	rs4908047	G	A			-0.0421	0.0225	0.0609
 1	100694042	rs4907905	C	T			-0.0431	0.0225	0.05489
 1	100694754	rs4908048	C	T			-0.0354	0.0229	0.122
 1	100694792	rs4908049	C	T			0.0318	0.0229	0.165
 1	100695014	rs11166419	G	A			0.0233	0.0371	0.5295
 1	100695250	rs6678629	T	A			-0.0238	0.0231	0.3019
@@ -3278,15 +3278,15 @@
 1	100716167	rs7520551	G	A			-0.022	0.0216	0.3105
 1	100716217	rs78826581	G	A			0.0214	0.0362	0.5545
 1	100716659	rs114718133	T	A			0.1971	0.1101	0.07348
 1	100717414	rs10157963	G	T			-0.0151	0.0225	0.5003
 1	100717447	rs10747506	G	T			0.0159	0.0225	0.4805
 1	100717760	rs3131837	G	C			-0.0161	0.0225	0.4733
 1	100718010	rs12725927	G	A			0.028	0.0216	0.1954
-1	100718316	rs755600801	C	CTTTG			-0.022	0.0217	0.3106
+1	100718316	rs68115821	C	CTTTG			-0.022	0.0217	0.3106
 1	100719083	rs4559529	G	A			0.0173	0.0224	0.4403
 1	100719130	rs12060945	C	T			0.0531	0.0171	0.001905
 1	100719133	rs7417332	C	T			0.0176	0.0224	0.4337
 1	100719371	rs10158183	G	A			-0.0194	0.0224	0.3852
 1	100720376	rs7521284	C	T			-0.0165	0.0224	0.4614
 1	100720764	rs7552568	C	T			0.0229	0.0217	0.2911
 1	100720847	rs10875282	G	A			0.025	0.0217	0.2479
@@ -3340,15 +3340,15 @@
 1	100738128	rs115310914	C	T			0.0851	0.0802	0.2882
 1	100738198	rs10747507	T	A			0.0155	0.0225	0.4896
 1	100738673	rs10783128	C	T			0.0119	0.0225	0.5979
 1	100739472	rs186549204	G	A			-0.1548	0.1159	0.1817
 1	100739646	rs75119298	G	C			0.0011	0.0358	0.9747
 1	100739833	rs76092506	C	A			0.0633	0.0572	0.2688
 1	100740485	rs116538743	C	T			-0.1406	0.0786	0.07359
-1	100740606	rs1349720804	GAACTT	G			-0.0697	0.0407	0.08695
+1	100740606	rs10601886	GAACTT	G			-0.0697	0.0407	0.08695
 1	100741875	rs144689823	C	T			-0.1458	0.1503	0.3318
 1	100741973	rs11166423	G	A			-0.0113	0.0226	0.6175
 1	100742034	rs56207296	G	A			0.0062	0.0358	0.8619
 1	100742399	rs10158777	C	T			0.0124	0.0227	0.5833
 1	100742422	rs17420377	G	C			0.0534	0.0611	0.3823
 1	100742670	rs4495726	G	A			-0.0171	0.0226	0.4483
 1	100743078	rs4433415	G	A			-0.0167	0.0226	0.4591
@@ -3384,15 +3384,15 @@
 1	100754583	rs11166425	G	T			-0.0207	0.0218	0.341
 1	100754660	rs11166426	G	A			-0.0114	0.0225	0.6135
 1	100754862	rs9728652	G	T			0.0231	0.0208	0.2676
 1	100754864	rs9727631	G	T			-0.0143	0.0209	0.4932
 1	100756226	rs113242148	G	T			0.0875	0.0542	0.1065
 1	100756252	rs115135282	G	A			0.0344	0.0363	0.3442
 1	100756271	rs181214647	G	T			-0.0777	0.0745	0.2973
-1	100756884	rs776108956	C	CT			0.0023	0.0373	0.9502
+1	100756884	rs147800556	C	CT			0.0023	0.0373	0.9502
 1	100757176	rs41287264	G	T			0.0624	0.041	0.128
 1	100757366	rs140559030	C	A			0.1886	0.1273	0.1384
 1	100757370	rs41287266	G	A			-0.1903	0.2052	0.3538
 1	100757763	rs6704125	C	T			-0.0094	0.0227	0.6787
 1	100757824	rs114909585	C	T			0.0908	0.0482	0.05943
 1	100757944	rs41287268	C	T			-0.0644	0.1112	0.5625
 1	100758100	rs185094377	G	A			-0.0472	0.1402	0.7366
@@ -3403,15 +3403,15 @@
 1	100760164	rs12089688	C	T			0.0243	0.0223	0.2766
 1	100760231	rs185765528	G	A			0.1177	0.0684	0.0851
 1	100760732	rs11166428	C	T			0.0141	0.0226	0.5328
 1	100761205	rs9787046	C	T			0.0162	0.0227	0.4743
 1	100761380	rs146773872	G	A			-0.0331	0.0362	0.3615
 1	100761423	rs191310577	G	A			-0.0888	0.1161	0.444
 1	100762082	rs189210405	C	T			0.047	0.187	0.8016
-1	100762274	rs932616963	AC	A			-0.0755	0.0414	0.06823
+1	100762274	rs143712488	AC	A			-0.0755	0.0414	0.06823
 1	100762417	rs189270040	C	T			-0.0503	0.1808	0.7807
 1	100762959	rs4908057	G	A			-0.0011	0.0361	0.9766
 1	100762977	rs12070304	C	A			-0.0123	0.0227	0.5878
 1	100763104	rs6657820	G	C			-0.011	0.0228	0.6287
 1	100763239	rs186223249	C	A			-0.2931	0.1238	0.01795
 1	100763868	rs4908058	T	A			0.0162	0.023	0.4823
 1	100764242	rs78213268	G	A			-0.1447	0.08	0.0705
@@ -3537,22 +3537,22 @@
 1	100805427	rs80315486	G	C			-0.0634	0.0625	0.3109
 1	100806404	rs6577168	C	T			0.0159	0.0309	0.6059
 1	100806897	rs10783130	G	C			0.0116	0.0204	0.5698
 1	100806957	rs144987088	G	A			-0.105	0.0743	0.1577
 1	100807067	rs146027418	G	C			0.1787	0.1573	0.2559
 1	100807546	rs12026454	G	T			0.0065	0.0169	0.7025
 1	100807569	rs74229545	G	T			0.0696	0.0624	0.265
-1	100807575	rs1473209476	AC	A			-0.0088	0.0211	0.6762
+1	100807575	rs143972875	AC	A			-0.0088	0.0211	0.6762
 1	100807705	rs12068339	G	T			-0.003	0.0214	0.8881
 1	100807723	rs112472955	C	CG			0.0014	0.0237	0.9533
 1	100807730	rs188395650	C	T			0.0026	0.0237	0.9114
 1	100807829	rs114070885	C	T			-0.0084	0.0213	0.6932
 1	100807830	rs74925509	G	A			-0.0697	0.0624	0.2644
 1	100808286	rs11166439	G	C			-0.0166	0.0204	0.4169
-1	100808350	rs1053334074	C	CT			0.006	0.0213	0.7776
+1	100808350	rs66482710	C	CT			0.006	0.0213	0.7776
 1	100808363	rs11166440	G	A			-0.0161	0.0166	0.3331
 1	100808834	rs74412605	C	T			0.052	0.066	0.4304
 1	100810166	rs4376760	G	T			0.0034	0.0209	0.8713
 1	100810462	rs115659897	G	A			-0.0153	0.1052	0.8846
 1	100811325	rs74103117	G	A			-0.0502	0.0659	0.4463
 1	100811859	rs7516666	G	T			0.0011	0.0181	0.9526
 1	100812104	rs12123193	C	T			0.0026	0.0208	0.9017
@@ -3561,15 +3561,15 @@
 1	100813605	rs61811378	C	T			0.1338	0.0931	0.1507
 1	100814234	rs74103120	T	A			-0.0129	0.0203	0.5244
 1	100814398	rs77355199	C	T			-0.0093	0.021	0.6577
 1	100815080	rs12128994	G	T			-0.0072	0.0211	0.7322
 1	100816141	rs146478127	C	CAAG			0.0385	0.0552	0.4849
 1	100816459	rs3754130	G	A			0.0798	0.0629	0.2045
 1	100816607	rs181013295	G	A			-0.3841	0.151	0.01095
-1	100817165	rs1477360379	C	CCT			0.0064	0.0211	0.7631
+1	100817165	rs72060017	C	CCT			0.0064	0.0211	0.7631
 1	100817384	rs28361189	G	A			0.0077	0.0211	0.7145
 1	100818178	rs529224	G	C			0.0204	0.0165	0.2173
 1	100818286	rs527644	T	A			0.0142	0.0307	0.6434
 1	100818464	rs594529	C	T			0.0184	0.0581	0.7509
 1	100818728	rs17420882	G	T			-0.0315	0.0183	0.08615
 1	100819273	rs2297170	C	T			0.0131	0.0203	0.5175
 1	100819828	rs7548466	C	T			-0.0826	0.0541	0.1269
@@ -3615,15 +3615,15 @@
 1	100834466	rs6675643	G	A			0.0185	0.0216	0.3934
 1	100835078	rs6687448	G	A			-0.0189	0.0216	0.3821
 1	100835546	rs494571	T	A			0.0152	0.0428	0.7219
 1	100835752	rs74510465	C	T			-0.0352	0.0614	0.5663
 1	100836711	rs189669549	C	T			0.0944	0.0949	0.3199
 1	100838317	rs74780928	G	A			-0.0211	0.0217	0.3308
 1	100838512	rs12088125	T	A			0.0204	0.0216	0.3468
-1	100838782	rs894436879	ATTG	A			-0.0203	0.0217	0.3496
+1	100838782	rs150534623	ATTG	A			-0.0203	0.0217	0.3496
 1	100839167	rs116776070	C	T			0.1911	0.0938	0.04156
 1	100839297	rs113513395	T	A			-0.1185	0.0917	0.1959
 1	100839454	rs142047252	C	T			-0.0224	0.0224	0.3178
 1	100839820	rs79230816	G	A			-0.0191	0.0234	0.4127
 1	100839876	rs34097376	C	T			-0.0196	0.0232	0.3991
 1	100840352	rs145141847	G	A			0.1579	0.117	0.1772
 1	100840367	rs3887285	G	A			-0.0194	0.0216	0.3682
@@ -3697,16 +3697,16 @@
 1	100866354	rs148176311	C	T			-0.2178	0.123	0.07664
 1	100867156	rs7520005	G	A			0.0261	0.0208	0.2099
 1	100867392	rs112842520	C	A			-0.0656	0.0625	0.2939
 1	100867438	rs139156904	C	T			-0.062	0.0625	0.3208
 1	100867465	rs144126249	G	A			0.0757	0.0619	0.2212
 1	100867543	rs143160771	G	A			-0.0611	0.0636	0.337
 1	100867549	rs146666348	G	A			-0.0662	0.0635	0.2969
-1	100868093	rs776239154	C	CATCTT			0.0566	0.0624	0.3649
-1	100868698	rs775354218	C	CT			0.0222	0.0217	0.3066
+1	100868093	rs140167539	C	CATCTT			0.0566	0.0624	0.3649
+1	100868698	rs58710320	C	CT			0.0222	0.0217	0.3066
 1	100869204	rs12068983	G	A			0.0229	0.0217	0.2897
 1	100869821	rs7531643	C	T			0.0262	0.0208	0.2069
 1	100870181	rs150574893	C	T			0.0546	0.0623	0.3804
 1	100870417	rs201993947	AC	A			0.0022	0.0339	0.9484
 1	100870555	rs57584762	G	C			-0.0578	0.0626	0.3556
 1	100871006	rs112016464	C	T			0.0267	0.0208	0.1982
 1	100871131	rs80175205	C	T			-0.0617	0.0591	0.297
@@ -3810,15 +3810,15 @@
 1	100918124	rs6703191	C	T			0.0256	0.0207	0.2163
 1	100918701	rs187340760	G	A			-0.0646	0.138	0.6396
 1	100919553	rs7524116	G	A			-0.0258	0.0207	0.2138
 1	100919788	rs10493922	G	A			-0.0253	0.0207	0.2224
 1	100920138	rs17122548	C	T			0.0104	0.08	0.8967
 1	100920240	rs28364870	C	T			-0.0204	0.0208	0.3253
 1	100920273	rs17122552	T	A			-0.0232	0.0208	0.2632
-1	100920632	rs770975651	C	CT			-0.013	0.0803	0.8711
+1	100920632	rs3834081	C	CT			-0.013	0.0803	0.8711
 1	100920901	rs28364871	C	T			-0.0406	0.0875	0.6425
 1	100921190	rs17122554	G	A			0.0248	0.0208	0.2314
 1	100921505	rs28364874	G	C			0.0136	0.0411	0.7405
 1	100921669	rs17456480	T	A			0.0298	0.0422	0.4809
 1	100923182	rs12057397	G	A			-0.0224	0.0214	0.2945
 1	100923262	rs7526455	C	T			0.0226	0.0208	0.276
 1	100923312	rs186841603	G	C			0.0258	0.0942	0.784
@@ -3832,23 +3832,23 @@
 1	100925395	rs146551297	C	T			-0.1026	0.0992	0.3011
 1	100925633	rs11166456	C	T			0.0045	0.0162	0.7818
 1	100925809	rs11803701	G	C			0.0255	0.0207	0.2192
 1	100925930	rs6666899	C	T			-0.0248	0.0207	0.2313
 1	100926050	rs11800410	G	A			0.0113	0.08	0.8876
 1	100926220	rs6667133	C	T			0.0079	0.0805	0.9219
 1	100926901	rs28364877	C	T			-0.0102	0.0204	0.6173
-1	100926991	rs572184338	C	CT			0.0207	0.0209	0.3217
-1	100927102	rs750022362	TG	T			-0.0123	0.0224	0.5829
+1	100926991	rs28364878	C	CT			0.0207	0.0209	0.3217
+1	100927102	rs28364879	TG	T			-0.0123	0.0224	0.5829
 1	100927132	rs28364880	C	T			0.0305	0.0437	0.4852
 1	100928418	rs28364884	G	C			-0.1355	0.1079	0.209
 1	100928595	rs28364886	C	T			0.0058	0.0356	0.8703
 1	100929453	rs471849	G	A			0.0059	0.042	0.8873
 1	100930254	rs10493923	C	T			0.018	0.0166	0.2795
 1	100931073	rs3754131	C	A			-0.0174	0.0166	0.2944
-1	100931758	rs72227440	TGA	T			0.0889	0.1386	0.5212
+1	100931758	rs3835648	TGA	T			0.0889	0.1386	0.5212
 1	100932506	rs2988395	G	C			0.1121	0.1387	0.4191
 1	100932659	rs28364891	C	CA			0.1183	0.1388	0.394
 1	100932962	rs78501063	C	T			-0.0414	0.0563	0.4624
 1	100933388	rs560431	C	T			0.1288	0.1214	0.2886
 1	100934325	rs568820	C	T			0.1194	0.1404	0.395
 1	100934730	rs678247	C	T			-0.1081	0.1391	0.4373
 1	100934810	rs677815	G	A			0.1324	0.1225	0.2797
@@ -3886,15 +3886,15 @@
 1	100955189	rs1432419	G	A			0.0071	0.016	0.6592
 1	100955532	rs508020	C	T			0.0057	0.016	0.7205
 1	100956089	rs144029356	C	A			0.093	0.376	0.8046
 1	100956108	rs649491	G	C			0.1063	0.1396	0.4462
 1	100956184	rs480398	C	T			-0.1069	0.1396	0.4437
 1	100956230	rs72730167	G	A			-0.0334	0.0452	0.4596
 1	100956478	rs12722868	G	A			-0.0169	0.0166	0.3088
-1	100956894	rs756469291	C	CTA			0.1015	0.1394	0.4667
+1	100956894	rs3081868	C	CTA			0.1015	0.1394	0.4667
 1	100957340	rs559548	C	T			-0.1006	0.053	0.05783
 1	100957489	rs187713639	G	A			-0.2788	0.1966	0.1561
 1	100958190	rs149221170	C	T			0.1282	0.1075	0.2329
 1	100958296	rs202033249	AT	A			-0.0847	0.0597	0.1559
 1	100959242	rs1566213	G	A			0.1098	0.1392	0.4302
 1	100959325	rs1566212	C	T			0.1309	0.1226	0.2855
 1	100959634	rs10783132	G	T			0.1118	0.1393	0.4224
@@ -4186,15 +4186,15 @@
 1	101044089	rs2783696	G	A			0.0129	0.0162	0.4253
 1	101044150	rs10875316	G	A			-0.0113	0.0162	0.4846
 1	101044366	rs11166484	G	A			-0.0308	0.0318	0.3336
 1	101044402	rs1577513	C	A			0.0143	0.0161	0.3753
 1	101045040	rs2783693	C	T			0.0148	0.0161	0.3592
 1	101045193	rs34752753	G	T			0.0156	0.0161	0.3352
 1	101045438	rs10875317	G	T			-0.0125	0.0161	0.4381
-1	101045521	rs34063693	C	CATTT			0.0267	0.0168	0.1124
+1	101045521	rs3081879	C	CATTT			0.0267	0.0168	0.1124
 1	101045590	rs79510782	G	A			-0.0473	0.0521	0.3638
 1	101045787	rs139826536	C	T			0.13	0.1144	0.2559
 1	101046092	rs4908074	G	A			-0.0165	0.0208	0.4256
 1	101046147	rs115939881	C	T			-0.2177	0.1221	0.07465
 1	101046229	rs1414417	T	A			0.0172	0.0207	0.4074
 1	101046273	rs12026951	C	T			-0.0146	0.0161	0.3672
 1	101046373	rs1414418	G	T			0.0462	0.0252	0.06634
@@ -4274,15 +4274,15 @@
 1	101069529	rs200585141	AC	A			0.0536	0.0246	0.02973
 1	101070012	rs140960126	C	T			-0.0597	0.2103	0.7764
 1	101071041	rs4492647	C	A			-0.0258	0.0167	0.1227
 1	101071216	rs2484544	G	A			-0.0245	0.0204	0.2297
 1	101071399	rs114402125	G	A			-0.0692	0.0934	0.4585
 1	101071566	rs7521758	C	T			-0.055	0.0245	0.02498
 1	101071668	rs7535936	C	T			0.0493	0.0246	0.04519
-1	101071689	rs34698507	C	CAGTT			0.0207	0.0205	0.3116
+1	101071689	rs10539270	C	CAGTT			0.0207	0.0205	0.3116
 1	101071710	rs149532320	T	A			0.1155	0.0948	0.2231
 1	101071713	rs144187511	G	T			0.0236	0.0598	0.6932
 1	101071807	rs11392790	TG	T			0.0226	0.0204	0.2675
 1	101071855	rs7533695	G	A			0.0554	0.0245	0.02386
 1	101072470	rs3908820	G	A			-0.0301	0.0318	0.3435
 1	101072925	rs17123012	C	T			0.0246	0.0317	0.4389
 1	101073073	rs17123014	T	A			-0.076	0.0487	0.1189
@@ -4334,15 +4334,15 @@
 1	101084510	rs34808415	GT	G			-0.0054	0.0161	0.7365
 1	101084542	rs1815519	G	A			0.0058	0.0277	0.8351
 1	101084829	rs146508894	C	T			0.1573	0.17	0.3547
 1	101085094	rs11583008	G	A			-0.0022	0.016	0.8897
 1	101085835	rs6663612	C	T			-0.0027	0.016	0.8671
 1	101085875	rs12240050	C	A			-0.026	0.0227	0.2522
 1	101086414	rs6681906	C	T			0.0025	0.016	0.8739
-1	101086577	rs948635393	C	CTA			-0.0027	0.0161	0.8655
+1	101086577	rs34819941	C	CTA			-0.0027	0.0161	0.8655
 1	101086816	rs6697310	C	T			-0.0031	0.0161	0.8458
 1	101087131	rs964905	C	T			0.0152	0.016	0.3437
 1	101087479	rs964906	G	A			0.0028	0.0161	0.8637
 1	101087871	rs55846182	G	A			-0.019	0.0954	0.8418
 1	101087901	rs4908085	G	C			-0.0022	0.016	0.8932
 1	101088010	rs149773612	G	A			0.0279	0.0479	0.5601
 1	101088016	rs115110362	C	T			-0.3302	0.2413	0.1711
@@ -4369,15 +4369,15 @@
 1	101092594	rs2297715	G	A			-0.0026	0.016	0.8708
 1	101092628	rs2297714	C	T			0.0244	0.0225	0.2777
 1	101092766	rs2297713	G	T			-0.0021	0.016	0.8958
 1	101092813	rs2297712	C	T			0.0023	0.016	0.8856
 1	101092955	rs12135243	G	A			-0.0027	0.0164	0.8707
 1	101093401	rs34232642	AT	A			-0.0044	0.0161	0.783
 1	101093412	rs192672438	G	A			0.083	0.1803	0.6455
-1	101093845	rs769603074	TTCTGTAGTCAC	T			0.0236	0.027	0.3836
+1	101093845	rs148923874	TTCTGTAGTCAC	T			0.0236	0.027	0.3836
 1	101094139	rs17403618	C	T			-0.0162	0.023	0.48
 1	101094202	rs141398181	C	T			-0.1411	0.1068	0.1863
 1	101094383	rs2282253	G	C			-0.0022	0.016	0.8899
 1	101094489	rs116654388	C	T			-0.0896	0.1284	0.4851
 1	101094609	rs4907918	G	A			0.0028	0.016	0.8607
 1	101094662	rs17412243	G	A			0.026	0.0271	0.3357
 1	101094739	rs139550120	C	T			0.0764	0.2706	0.7777
@@ -4476,15 +4476,15 @@
 1	101117125	rs1855801	G	A			0.0111	0.0342	0.7456
 1	101117684	rs72482850	T	A			0.0195	0.0222	0.3801
 1	101117890	rs12568236	C	A			-0.0191	0.0176	0.2772
 1	101117977	rs186480070	C	A			-0.318	0.1528	0.03739
 1	101118331	rs1855788	G	A			-0.0047	0.0161	0.7692
 1	101118510	rs150537707	G	A			-0.0877	0.1009	0.3848
 1	101118587	rs4908089	C	T			-0.038	0.0311	0.2213
-1	101118630	rs1271492352	C	CTAAA			0.1536	0.0604	0.01092
+1	101118630		C	CTAAA			0.1536	0.0604	0.01092
 1	101119213	rs141050170	C	T			-0.007	0.1089	0.9487
 1	101119506	rs116030424	G	A			0.104	0.1381	0.4516
 1	101119743	rs933095	G	A			0.0208	0.0222	0.3486
 1	101120323	rs76156696	G	A			0.0518	0.2208	0.8145
 1	101121313	rs149045740	G	A			-0.0279	0.0486	0.5655
 1	101121756	rs146645731	GA	G			0.031	0.0555	0.5769
 1	101122198	rs115756886	G	C			0.0166	0.0526	0.7522
@@ -4500,15 +4500,15 @@
 1	101124667	rs116273268	G	A			-0.1329	0.1083	0.2197
 1	101125206	rs72732151	C	T			0.1682	0.0636	0.008163
 1	101125560	rs2050472	C	T			-0.0062	0.0162	0.7018
 1	101126149	rs2491821	C	T			-0.1748	0.0627	0.005313
 1	101126353	rs4587587	G	C			0.0091	0.0198	0.6437
 1	101126959	rs182985027	T	A			-0.3211	0.146	0.02786
 1	101126973	rs141194146	C	T			0.2385	0.3318	0.4723
-1	101127107	rs74923139	ACT	A			0.1515	0.0614	0.01365
+1	101127107	rs5776533	ACT	A			0.1515	0.0614	0.01365
 1	101127310	rs12405129	C	T			0.0248	0.0271	0.3604
 1	101127381	rs4907920	C	T			0.1737	0.0629	0.005791
 1	101128249	rs4907921	C	T			0.0046	0.0162	0.7751
 1	101128579	rs4907922	G	A			-0.0051	0.0161	0.7524
 1	101128874	rs11166495	C	T			-0.0058	0.0162	0.7219
 1	101128934	rs12239501	C	T			0.0075	0.0163	0.6458
 1	101128950	rs12239176	G	A			0.0074	0.0164	0.6497
@@ -4585,15 +4585,15 @@
 1	101150532	rs12568023	C	T			0.0069	0.0198	0.7293
 1	101150791	rs141591843	G	A			0.0044	0.0543	0.9355
 1	101151364	rs11586333	G	C			0.0194	0.0221	0.3801
 1	101151441	rs116443886	G	A			0.143	0.101	0.1568
 1	101151890	rs11582558	G	A			-0.0189	0.0221	0.3923
 1	101152671	rs147235451	C	T			0.0198	0.039	0.6115
 1	101154403	rs190419377	G	A			0.041	0.1701	0.8095
-1	101154546	rs535629038	GA	G			-0.0211	0.0162	0.1922
+1	101154546	rs35071985	GA	G			-0.0211	0.0162	0.1922
 1	101154721	rs118147139	G	A			-0.1022	0.0771	0.1846
 1	101155168	rs140258506	G	C			0.0033	0.056	0.9535
 1	101156847	rs116573060	G	A			0.0826	0.0764	0.2792
 1	101157297	rs115890370	G	A			0.059	0.0576	0.3062
 1	101157405	rs75376323	C	T			0.0087	0.0198	0.66
 1	101158426	rs111548523	C	T			-0.1767	0.0627	0.004821
 1	101158998	rs144902109	G	A			-0.0378	0.1053	0.7199
@@ -4605,15 +4605,15 @@
 1	101160872	rs185683608	C	A			-0.0652	0.1384	0.6378
 1	101161251	rs1932352	G	A			-0.0082	0.0165	0.6182
 1	101161426	rs116335150	G	A			0.0255	0.0356	0.4737
 1	101163483	rs35248309	G	T			0.0229	0.0271	0.3978
 1	101163780	rs74412869	G	A			0.0088	0.0198	0.6545
 1	101164483	rs76692461	G	A			-0.0195	0.0221	0.3789
 1	101165477	rs116163847	C	A			0.0259	0.0345	0.4521
-1	101166253	rs552381243	TG	T			0.1794	0.0625	0.004127
+1	101166253	rs147789007	TG	T			0.1794	0.0625	0.004127
 1	101166306	rs112876911	G	A			-0.0642	0.1146	0.575
 1	101166648	rs12566680	G	A			0.0391	0.0311	0.2097
 1	101168121	rs1591474	C	T			-0.0094	0.017	0.5787
 1	101168196	rs1832123	G	A			-0.0061	0.0162	0.7041
 1	101168250	rs7414363	C	T			0.0089	0.0198	0.6512
 1	101168542	rs12562423	C	T			0.0061	0.0199	0.7603
 1	101168726	rs138345018	C	T			0.0245	0.0599	0.6829
@@ -4973,15 +4973,15 @@
 1	101283094	rs35359111	G	A			-0.0106	0.0239	0.6575
 1	101283765	rs116021477	G	C			-0.0036	0.0217	0.8687
 1	101284027	rs961912	G	A			0.0046	0.016	0.7751
 1	101284182	rs10159114	C	T			0.0041	0.016	0.7966
 1	101284251	rs34617755	C	T			0.0131	0.0239	0.5826
 1	101284293	rs10159117	C	T			0.0042	0.016	0.7928
 1	101284306	rs10158411	C	T			-0.0089	0.0161	0.5806
-1	101284362	rs34215868	G	A			-0.1525	0.1151	0.1851
+1	101284362	rs184908464	G	A			-0.1525	0.1151	0.1851
 1	101285052	rs71660940	G	A			0.0136	0.0239	0.5685
 1	101285547	rs4907926	G	A			-0.0035	0.016	0.8282
 1	101285900	rs10159287	T	A			-0.0041	0.016	0.7988
 1	101286613	rs114450485	G	A			-0.0011	0.0216	0.9607
 1	101286697	rs10159441	C	T			0.0033	0.016	0.8361
 1	101286780	rs6667465	G	A			0.0044	0.016	0.7815
 1	101286821	rs78713904	G	A			-0.0039	0.0919	0.9661
@@ -5112,15 +5112,15 @@
 1	101330984	rs12027668	G	A			-0.0087	0.0163	0.5954
 1	101331536	rs12048904	C	T			0.0085	0.0163	0.6037
 1	101331760	rs17123467	G	A			-0.0088	0.0163	0.5913
 1	101332457	rs137947295	C	T			0.0943	0.0824	0.2524
 1	101332499	rs143093673	C	T			0.0198	0.1178	0.8662
 1	101333733	rs11166529	C	T			-0.009	0.0163	0.5811
 1	101333737	rs10875347	C	T			0.0198	0.0182	0.2756
-1	101333893	rs746307524	TATG	T			0.0027	0.0215	0.9009
+1	101333893	rs36082557	TATG	T			0.0027	0.0215	0.9009
 1	101335803	rs115850179	C	T			0.0303	0.0545	0.578
 1	101335863	rs34586759	G	T			-0.226	0.0972	0.02004
 1	101338324	rs8888	C	T			0.0111	0.0163	0.4986
 1	101338482	rs3188491	G	A			0.0105	0.0164	0.5208
 1	101340134	rs12039319	C	T			-0.0178	0.0162	0.2722
 1	101341083	rs3737581	G	A			0.0191	0.0182	0.2943
 1	101341561	rs188716504	C	A			-0.0559	0.1347	0.6782
@@ -5231,19 +5231,19 @@
 1	101401840	rs140486668	C	T			0.1827	0.1487	0.2192
 1	101402982	rs61780298	G	T			-0.0032	0.021	0.8779
 1	101403115	rs34960901	C	T			-0.0121	0.0241	0.616
 1	101403202	rs182133880	C	T			0.0464	0.2018	0.8183
 1	101403471	rs61780299	C	T			-0.0028	0.0211	0.8927
 1	101403601	rs61780300	C	T			-0.0023	0.021	0.9139
 1	101403815	rs12121879	G	A			-0.0163	0.0236	0.4894
-1	101404724	rs747167730	C	CAT			-0.0024	0.021	0.9084
+1	101404724	rs76849254	C	CAT			-0.0024	0.021	0.9084
 1	101405156	rs144952946	G	T			0.0063	0.0215	0.7692
 1	101405180	rs147962364	G	C			-0.0065	0.0219	0.7673
 1	101405631	rs61780316	C	A			-0.0138	0.0433	0.7505
-1	101406500	rs757414213	C	CG			0.0137	0.0241	0.5704
+1	101406500	rs68126059	C	CG			0.0137	0.0241	0.5704
 1	101407028	rs6698798	T	A			0.029	0.0172	0.09119
 1	101407139	rs61780317	C	T			-0.0035	0.021	0.8687
 1	101407519	rs11581062	G	A			0.0041	0.0174	0.8155
 1	101408933	rs3850453	C	T			0.0041	0.0174	0.8152
 1	101409224	rs114769662	G	A			0.0713	0.0984	0.4685
 1	101411524	rs61780319	C	T			-0.0025	0.0211	0.9051
 1	101412302	rs72734276	G	C			0.0545	0.0601	0.365
@@ -5256,15 +5256,15 @@
 1	101415707	rs6577219	G	A			0.0055	0.0174	0.7516
 1	101416548	rs74919999	C	T			0.1291	0.0449	0.004054
 1	101416871	rs11582211	G	A			-0.0072	0.0176	0.6822
 1	101417143	rs115523210	G	C			0.0388	0.0861	0.6526
 1	101417687	rs138288233	C	A			0.0498	0.0767	0.5161
 1	101417697	rs187908032	C	T			-0.2178	0.2526	0.3886
 1	101418569	rs6675403	G	T			0.0056	0.0175	0.7508
-1	101418623	rs144918421	AT	A			0.0091	0.0246	0.71
+1	101418623	rs34481562	AT	A			0.0091	0.0246	0.71
 1	101418697	rs72734281	G	C			0.0118	0.0247	0.6322
 1	101418719	rs75437067	T	A			0.0094	0.0247	0.7039
 1	101420009	rs141488031	C	T			-0.0552	0.1022	0.5891
 1	101420406	rs6577221	G	A			0.0038	0.0211	0.8555
 1	101420502	rs6577222	G	C			0.0038	0.0175	0.8264
 1	101420755	rs189714196	T	A			-0.152	0.1016	0.1345
 1	101420957	rs3903905	G	T			-0.0044	0.0175	0.8039
@@ -5282,22 +5282,22 @@
 1	101425860	rs17123542	C	T			-0.101	0.0379	0.007723
 1	101426960	rs11588568	C	T			-0.0158	0.0247	0.5211
 1	101428304	rs61780321	G	A			0.0041	0.022	0.8534
 1	101428375	rs183564990	G	T			0.0545	0.1029	0.5963
 1	101428415	rs61780322	C	T			0.0072	0.0443	0.8709
 1	101428464	rs17610195	G	C			0.0061	0.0273	0.8222
 1	101428757	rs113578764	C	T			0.0173	0.0704	0.8054
-1	101429266	rs752881978	C	CAT			0.0193	0.0247	0.4362
+1	101429266	rs35504439	C	CAT			0.0193	0.0247	0.4362
 1	101429724	rs17610202	G	C			-0.0019	0.0222	0.9322
 1	101430504	rs17525507	G	A			0.0012	0.0222	0.9568
 1	101430834	rs180961463	G	T			0.0307	0.1113	0.7824
 1	101430977	rs146460646	G	C			-0.1485	0.0859	0.08398
 1	101431250	rs11166534	G	A			0.0477	0.0724	0.51
 1	101431909	rs7538863	G	T			0.0084	0.018	0.6392
-1	101431960	rs759769752	AG	A			0.0053	0.0222	0.8133
+1	101431960	rs11362786	AG	A			0.0053	0.0222	0.8133
 1	101433407	rs61780323	G	A			0.0007	0.0222	0.9736
 1	101433779	rs6689461	G	A			0.007	0.018	0.6986
 1	101433886	rs12741674	G	A			-0.0181	0.0246	0.4622
 1	101434200	rs139618641	C	T			0.3066	0.1441	0.03332
 1	101434336	rs61780324	C	A			-0.0541	0.0793	0.4955
 1	101434903	rs17408672	T	A			0.0503	0.0421	0.2327
 1	101434970	rs143991795	G	C			0.0516	0.0722	0.4744
@@ -5444,15 +5444,15 @@
 1	101516883	rs71952927	GTA	G			-0.0001	0.0223	0.9959
 1	101517491	rs17449778	G	A			-0.0163	0.0295	0.5793
 1	101517688	rs12567858	G	A			0.0108	0.0179	0.5465
 1	101518270	rs61782085	C	T			0.0011	0.0223	0.9618
 1	101518534	rs12410829	G	C			-0.0413	0.0469	0.3789
 1	101518682	rs139750954	G	A			-0.0249	0.0504	0.6204
 1	101518825	rs61782086	T	A			0.0081	0.0528	0.8787
-1	101518843	rs749984824	C	CAA			-0.0002	0.0223	0.9936
+1	101518843	rs113315027	C	CAA			-0.0002	0.0223	0.9936
 1	101522247	rs72736231	G	A			0.0832	0.1103	0.4508
 1	101522751	rs184979536	G	A			0.1024	0.1438	0.4762
 1	101522752	rs12733701	G	T			0.0254	0.0244	0.2972
 1	101523221	rs12738310	C	T			0.0234	0.0245	0.3395
 1	101523516	rs12122327	C	T			0.0595	0.0695	0.3923
 1	101523639	rs35445887	C	T			-0.0125	0.0179	0.4858
 1	101524336	rs34050803	C	T			-0.0236	0.0245	0.3354
@@ -5633,15 +5633,15 @@
 1	101602129	rs17450579	G	A			0.0225	0.0842	0.7892
 1	101602275	rs72736295	C	T			-0.0161	0.0694	0.8169
 1	101602454	rs589045	G	A			-0.0394	0.0189	0.03658
 1	101602799	rs187277703	G	A			-0.0705	0.098	0.4716
 1	101602905	rs182316439	G	A			0.029	0.123	0.8138
 1	101603189	rs144735511	G	A			0.0535	0.0809	0.508
 1	101603450	rs7513526	C	T			0.0325	0.0251	0.1958
-1	101603523	rs1212121787	AACT	A			-0.0335	0.025	0.1805
+1	101603523	rs147862356	AACT	A			-0.0335	0.025	0.1805
 1	101604003	rs192971669	C	T			0.0666	0.2231	0.7655
 1	101604116	rs6658561	G	T			0.0268	0.025	0.2851
 1	101604215	rs11584741	C	T			0.0031	0.074	0.9662
 1	101604554	rs514793	G	A			0.0191	0.0235	0.4149
 1	101604753	rs12756986	C	T			0.0225	0.0245	0.3585
 1	101604781	rs7524946	G	A			-0.0332	0.0251	0.1868
 1	101604889	rs74591599	C	T			-0.0312	0.0251	0.214
@@ -5667,24 +5667,24 @@
 1	101608840	rs72987264	C	T			-0.0315	0.0252	0.2113
 1	101609176	rs79957386	C	T			-0.0278	0.0252	0.2691
 1	101609191	rs112687689	C	CAA			0.0302	0.0252	0.2302
 1	101609584	rs79033494	G	T			-0.0191	0.0406	0.6381
 1	101609690	rs12408672	C	T			-0.0497	0.0507	0.3263
 1	101609854	rs142532192	C	T			-0.0884	0.0578	0.1267
 1	101610081	rs79303735	C	T			-0.0984	0.0411	0.01661
-1	101610128	rs200388645	C	CTCTT			0.0318	0.0251	0.2049
+1	101610128	rs112243251	C	CTCTT			0.0318	0.0251	0.2049
 1	101610394	rs139535267	G	A			0.0442	0.0954	0.6431
 1	101610618	rs72987265	C	T			0.0294	0.0252	0.2445
 1	101610653	rs72987266	T	A			-0.0279	0.0254	0.2725
 1	101610690	rs72987267	C	T			0.0257	0.0255	0.3146
 1	101610693	rs76089365	C	T			-0.0276	0.0257	0.2825
 1	101610806	rs61782144	G	A			-0.0063	0.0395	0.8734
 1	101611231	rs75027482	C	A			-0.0328	0.0252	0.1929
 1	101611375	rs77072829	C	T			0.0313	0.0251	0.2127
-1	101611513	rs921214961	TA	T			-0.0305	0.0252	0.2261
+1	101611513	rs138133882	TA	T			-0.0305	0.0252	0.2261
 1	101611909	rs112369725	G	T			-0.0344	0.0503	0.4943
 1	101612173	rs72987271	C	A			-0.0294	0.0251	0.2414
 1	101612212	rs72987272	G	A			-0.0301	0.0251	0.2319
 1	101612456	rs190395414	G	A			0.0839	0.0783	0.2838
 1	101612475	rs79043680	T	A			0.032	0.0253	0.2057
 1	101612738	rs72738103	G	A			0.058	0.1396	0.6777
 1	101612787	rs72987273	G	A			-0.0305	0.0251	0.2243
@@ -5797,15 +5797,15 @@
 1	101647080	rs10875355	G	A			-0.0109	0.0176	0.5359
 1	101647607	rs12746530	G	A			-0.0272	0.0511	0.5948
 1	101647626	rs76382185	C	T			-0.0514	0.025	0.03952
 1	101647645	rs56785411	C	A			-0.0373	0.0193	0.05379
 1	101647646	rs74106743	G	A			-0.0348	0.0194	0.07303
 1	101648318	rs76336747	G	A			-0.0347	0.0253	0.1698
 1	101648349	rs75773752	C	T			0.1013	0.0614	0.09923
-1	101648632	rs201427392	AAAGG	A			-0.0161	0.0509	0.7515
+1	101648632	rs140838471	AAAGG	A			-0.0161	0.0509	0.7515
 1	101648821	rs79628995	G	A			0.0292	0.0258	0.2575
 1	101648945	rs76716700	G	T			-0.05	0.0294	0.08854
 1	101649376	rs116763319	C	T			-0.0978	0.1647	0.5525
 1	101650401	rs182464135	G	A			0.3084	0.1946	0.1131
 1	101650409	rs148408620	C	T			0.0073	0.0514	0.8874
 1	101651017	rs10430077	T	A			-0.033	0.0177	0.06251
 1	101651440	rs35250801	C	T			0.0249	0.0509	0.6256
@@ -5873,15 +5873,15 @@
 1	101660370	rs11166551	G	A			-0.0463	0.0258	0.0731
 1	101660413	rs3927520	C	T			0.0653	0.0378	0.08416
 1	101660784	rs144646185	G	A			0.0107	0.0413	0.7951
 1	101660850	rs147898923	G	T			0.0042	0.0701	0.9527
 1	101661393	rs142882259	G	C			0.0928	0.0833	0.2654
 1	101661433	rs12404120	C	T			0.0547	0.0356	0.124
 1	101661466	rs7522355	C	T			0.006	0.0194	0.7551
-1	101661530	rs141691988	ATC	A			0.0455	0.0359	0.2055
+1	101661530	rs59285306	ATC	A			0.0455	0.0359	0.2055
 1	101661568	rs12410412	C	A			-0.0219	0.0175	0.2117
 1	101661812	rs12124965	C	A			-0.0303	0.0217	0.1629
 1	101661835	rs60124357	TA	T			0.0242	0.0302	0.4239
 1	101661978	rs11166552	C	T			-0.0043	0.0183	0.814
 1	101662126	rs7534599	G	A			-0.0085	0.0336	0.7999
 1	101662163	rs7537017	C	T			-0.0303	0.0462	0.5119
 1	101662690	rs190102479	C	T			-0.0547	0.1845	0.7669
@@ -6201,15 +6201,15 @@
 1	101747767	rs6577233	C	T			0.0106	0.0159	0.5072
 1	101747966	rs114751910	G	A			0.0302	0.0566	0.5939
 1	101748071	rs12040717	C	T			-0.0185	0.0327	0.5716
 1	101748158	rs114314913	C	T			0.024	0.0899	0.7894
 1	101748162	rs7550774	G	A			0.0102	0.0159	0.5209
 1	101748517	rs56921769	GT	G			0.0359	0.0268	0.1796
 1	101748658	rs6663691	G	T			-0.01	0.016	0.5323
-1	101749437	rs1230747467	GTCCTAGTT	G			-0.0094	0.0793	0.9053
+1	101749437	rs199577064	GTCCTAGTT	G			-0.0094	0.0793	0.9053
 1	101749680	rs910634	G	T			-0.0103	0.016	0.5213
 1	101749974	rs910633	G	A			0.0115	0.0159	0.4699
 1	101750048	rs910632	G	A			0.0115	0.0159	0.4721
 1	101750214	rs2392240	C	T			-0.012	0.016	0.4531
 1	101750353	rs187790825	C	A			-0.2027	0.0829	0.01447
 1	101750383	rs910631	G	A			0.012	0.0159	0.4533
 1	101750466	rs6659211	G	A			0.0311	0.0268	0.2462
@@ -6390,15 +6390,15 @@
 1	101783848	rs7524633	C	A			-0.0407	0.0167	0.01441
 1	101784000	rs61780749	G	A			0.042	0.0615	0.4944
 1	101784285	rs148619387	G	A			0.1019	0.0884	0.2488
 1	101785179	rs17454557	C	T			-0.0471	0.0394	0.2321
 1	101785340	rs57706739	C	T			0.0887	0.0444	0.04565
 1	101785364	rs147935745	C	T			0.0442	0.0755	0.5584
 1	101785548	rs6676441	G	A			0.0001	0.0406	0.9981
-1	101785672	rs1266090334	AAAT	A			-0.0289	0.027	0.2837
+1	101785672	rs200668916	AAAT	A			-0.0289	0.027	0.2837
 1	101785684	rs12145848	G	A			0.0122	0.0208	0.5568
 1	101786034	rs1555263	G	A			0.0008	0.0166	0.9596
 1	101786117	rs1973939	C	T			0.013	0.0196	0.5054
 1	101786128	rs192130592	G	A			-0.0491	0.1634	0.7639
 1	101786142	rs7519558	C	T			0.0319	0.0192	0.09683
 1	101786293	rs9434191	C	T			-0.0235	0.0235	0.3161
 1	101786421	rs17420712	C	T			0.008	0.0209	0.7027
@@ -6769,15 +6769,15 @@
 1	101862549	rs117077125	T	A			-0.0447	0.1939	0.8179
 1	101862699	rs10874485	G	C			0.1072	0.0484	0.0266
 1	101863214	rs12085470	C	A			-0.0082	0.016	0.6091
 1	101863223	rs12085471	C	A			-0.0084	0.016	0.6008
 1	101863279	rs181289062	G	A			0.0921	0.1388	0.5068
 1	101864021	rs7548919	G	C			0.0643	0.03	0.03208
 1	101864151	rs191147820	C	T			-0.0337	0.1049	0.7476
-1	101864173	rs1468750043	TA	T			0.0082	0.0638	0.898
+1	101864173	rs200167686	TA	T			0.0082	0.0638	0.898
 1	101864215	rs12403551	G	A			-0.0076	0.016	0.6351
 1	101864228	rs55836157	G	A			-0.0758	0.0304	0.01268
 1	101864493	rs12408470	C	T			-0.0088	0.016	0.5819
 1	101864589	rs12404865	C	T			0.0062	0.0161	0.6987
 1	101864597	rs12404868	C	T			0.0062	0.0161	0.7016
 1	101865012	rs12041998	C	T			0.0758	0.0286	0.007944
 1	101865066	rs76418125	G	A			-0.0148	0.0267	0.5789
@@ -6860,15 +6860,15 @@
 1	101880805	rs6694481	C	T			-0.0026	0.0437	0.9516
 1	101880992	rs79943521	G	A			-0.023	0.043	0.5921
 1	101881294	rs190504391	G	C			0.0595	0.1452	0.682
 1	101881822	rs145998579	C	CA			0.0094	0.0445	0.8322
 1	101881889	rs6697985	G	C			-0.0519	0.0372	0.1627
 1	101882295	rs72723636	G	A			-0.0196	0.0351	0.5771
 1	101882596	rs183279528	G	A			0.0025	0.1668	0.9879
-1	101882854	rs1255897427	AAAAC	A			0.0768	0.0844	0.3627
+1	101882854		AAAAC	A			0.0768	0.0844	0.3627
 1	101882875	rs6701418	C	A			-0.0013	0.0163	0.9379
 1	101883023	rs12138422	G	A			-0.0092	0.0189	0.625
 1	101883032	rs6665621	G	A			0.0108	0.0165	0.5143
 1	101883505	rs12043112	G	A			0.0074	0.0279	0.791
 1	101883768	rs112683582	C	T			-0.1318	0.0604	0.02912
 1	101883782	rs74625277	T	A			0.0211	0.0263	0.422
 1	101884572	rs58181333	G	A			-0.0084	0.0279	0.7639
@@ -6956,26 +6956,26 @@
 1	101903680	rs181473146	G	A			0.3153	0.1898	0.0966
 1	101903923	rs12127142	C	T			-0.016	0.0271	0.5545
 1	101904161	rs74617235	G	T			0.0433	0.0734	0.5547
 1	101904166	rs186208589	T	A			0.1587	0.1331	0.2334
 1	101904325	rs4908145	G	A			-0.0144	0.0165	0.3808
 1	101904451	rs72723656	C	T			0.0413	0.0402	0.3038
 1	101904547	rs139410900	C	T			-0.026	0.2382	0.9131
-1	101904642	rs770818478	TGC	T			-0.0133	0.0271	0.6224
+1	101904642	rs59800119	TGC	T			-0.0133	0.0271	0.6224
 1	101904649	rs4908146	C	T			0.014	0.0287	0.6266
 1	101904701	rs117910241	G	A			0.0182	0.0537	0.7347
 1	101904719	rs111741610	T	A			-0.1403	0.0603	0.02002
 1	101904916	rs183659956	C	T			0.1487	0.1327	0.2625
 1	101905057	rs12074596	C	T			0.3163	0.1658	0.05642
 1	101905115	rs112900871	C	T			0.1366	0.0615	0.02626
 1	101905249	rs10747409	G	A			0.0139	0.0286	0.627
 1	101905251	rs12047481	G	A			-0.0016	0.0277	0.9535
 1	101905399	rs186181126	C	T			0.2416	0.2528	0.3392
 1	101905600	rs151088695	G	A			0.1603	0.1329	0.2279
-1	101905751	rs755268192	AAGG	A			0.0002	0.028	0.9947
+1	101905751	rs57454035	AAGG	A			0.0002	0.028	0.9947
 1	101905770	rs115963083	G	A			0.0503	0.0506	0.3208
 1	101906074	rs141875560	C	T			0.0234	0.0542	0.6653
 1	101906281	rs4908147	C	T			-0.013	0.0272	0.6335
 1	101906359	rs72723658	G	A			0.0067	0.0278	0.8088
 1	101906412	rs11811621	G	A			-0.0009	0.0163	0.956
 1	101906886	rs187230236	C	A			0.1212	0.1301	0.3515
 1	101906905	rs7556416	G	A			-0.0101	0.0165	0.5417
@@ -7062,15 +7062,15 @@
 1	101926982	rs12405025	G	A			-0.02	0.0326	0.5396
 1	101927038	rs12405027	C	A			-0.0209	0.0326	0.521
 1	101927102	rs2798586	C	T			0.0195	0.0286	0.496
 1	101927194	rs11164204	T	A			0.0106	0.0221	0.6329
 1	101927321	rs1199715	G	A			-0.0218	0.0326	0.5034
 1	101927417	rs182366318	C	T			0.2013	0.1308	0.1239
 1	101927483	rs9324334	G	T			0.0003	0.0278	0.9908
-1	101927517	rs906167030	TA	T			0.0155	0.0444	0.7272
+1	101927517	rs143070521	TA	T			0.0155	0.0444	0.7272
 1	101927667	rs1199713	C	A			0.0074	0.0217	0.734
 1	101928396	rs1199711	C	T			-0.0014	0.0182	0.9408
 1	101928502	rs142511554	G	A			0.187	0.1309	0.1532
 1	101928933	rs112740963	C	T			-0.17	0.0761	0.02559
 1	101929301	rs181940504	G	A			0.0273	0.1783	0.8782
 1	101929350	rs189595268	G	T			-0.1743	0.1307	0.1823
 1	101929409	rs60639654	G	A			0.0152	0.027	0.5719
@@ -7100,15 +7100,15 @@
 1	101934624	rs61780580	C	A			-0.0111	0.027	0.6802
 1	101934675	rs1819749	G	A			-0.0067	0.0163	0.6826
 1	101934869	rs1160290	G	A			0.0141	0.0287	0.6241
 1	101935152	rs56312009	C	T			-0.0137	0.0269	0.6098
 1	101935194	rs1777869	C	A			0.0069	0.0163	0.6707
 1	101935196	rs182850012	G	A			-0.0309	0.1056	0.7697
 1	101935635	rs1776927	G	C			-0.0066	0.0163	0.684
-1	101936042	rs199813887	C	CAAAA			0.0131	0.031	0.672
+1	101936042		C	CAAAA			0.0131	0.031	0.672
 1	101936239	rs186498828	G	T			-0.1646	0.1299	0.205
 1	101936348	rs147747188	C	T			-0.0502	0.1729	0.7715
 1	101936540	rs60698249	G	A			0.0018	0.0278	0.9481
 1	101936888	rs116334130	G	T			0.0624	0.0721	0.387
 1	101936904	rs17124601	G	A			0.003	0.0278	0.9138
 1	101937089	rs1388453	C	T			0.02	0.0325	0.5374
 1	101937381	rs1388454	G	A			0.0113	0.0173	0.5152
@@ -7463,15 +7463,15 @@
 1	101986022	rs72725641	C	A			0.0178	0.0728	0.8063
 1	101986109	rs1199580	C	A			0.0067	0.0159	0.6743
 1	101986165	rs192427853	C	A			0.1913	0.1301	0.1415
 1	101986201	rs182282709	G	T			0.1752	0.1324	0.1858
 1	101986202	rs187207534	T	A			-0.1752	0.1324	0.1858
 1	101986206	rs12123756	C	T			-0.0034	0.0187	0.8549
 1	101986223	rs78562723	C	T			0.0812	0.0524	0.121
-1	101986237	rs768964509	C	CTGTCCTCAGAGA			0.0039	0.0284	0.8894
+1	101986237	rs139267503	C	CTGTCCTCAGAGA			0.0039	0.0284	0.8894
 1	101986353	rs56363143	AT	A			0.0313	0.0266	0.2393
 1	101986432	rs12119903	G	A			0.0099	0.017	0.561
 1	101986475	rs191629303	G	T			-0.1847	0.1301	0.1557
 1	101986575	rs184619812	C	T			0.1723	0.1332	0.196
 1	101986610	rs72725642	G	A			-0.0026	0.0278	0.9244
 1	101986672	rs12123925	C	T			-0.0028	0.0187	0.8791
 1	101986816	rs193083480	G	A			-0.1858	0.1301	0.1532
@@ -7491,15 +7491,15 @@
 1	101987589	rs191837136	G	A			-0.173	0.1328	0.1928
 1	101987619	rs1199578	G	A			0.0079	0.0162	0.6232
 1	101987739	rs182806679	G	C			-0.0191	0.0948	0.8406
 1	101987864	rs192999267	G	T			0.0336	0.1805	0.8523
 1	101987875	rs11164221	T	A			-0.003	0.0187	0.8736
 1	101987900	rs185254235	C	T			-0.1965	0.1295	0.1292
 1	101988167	rs59419209	AAAG	A			-0.0023	0.0278	0.9331
-1	101988353	rs11346127	C	CT			0.0239	0.0317	0.4514
+1	101988353		C	CT			0.0239	0.0317	0.4514
 1	101988393	rs78382395	G	A			-0.0429	0.0596	0.4714
 1	101988395	rs12030527	C	T			0.0025	0.028	0.9288
 1	101988558	rs192305045	T	A			0.187	0.1303	0.1511
 1	101989037	rs12122181	G	C			0.0027	0.0187	0.885
 1	101989151	rs180781630	G	A			-0.1797	0.1347	0.1822
 1	101989215	rs184887276	G	A			0.164	0.2516	0.5145
 1	101989246	rs76250476	G	A			-0.0163	0.0285	0.5674
@@ -7678,15 +7678,15 @@
 1	102013609	rs1014919	G	C			-0.0129	0.0244	0.5977
 1	102013715	rs1777887	G	C			-0.0166	0.0198	0.402
 1	102013815	rs1777886	C	T			0.0173	0.0195	0.3764
 1	102014020	rs12736372	G	A			0.007	0.0191	0.7133
 1	102014131	rs150150327	C	A			0.0938	0.0913	0.3045
 1	102014316	rs6704106	C	T			-0.0001	0.0186	0.9974
 1	102014325	rs186389154	C	T			-0.1584	0.1308	0.226
-1	102014378	rs780031412	C	CTACTT			-0.0026	0.0187	0.8882
+1	102014378	rs142561599	C	CTACTT			-0.0026	0.0187	0.8882
 1	102014461	rs12565611	C	T			-0.0035	0.0187	0.852
 1	102014568	rs12565619	C	T			-0.0024	0.0187	0.896
 1	102015200	rs4326640	C	T			0.0022	0.0187	0.9068
 1	102015502	rs1155720	T	A			0.003	0.0185	0.8718
 1	102015585	rs1155719	G	T			0.0041	0.0185	0.8235
 1	102015618	rs1155718	C	T			-0.0042	0.0185	0.82
 1	102015773	rs979828	G	A			0.0031	0.0187	0.8678
@@ -7918,15 +7918,15 @@
 1	102049445	rs76699049	C	T			-0.2109	0.1375	0.1252
 1	102050183	rs111527059	C	T			0.1957	0.146	0.18
 1	102050373	rs12030834	T	A			-0.0156	0.0182	0.3921
 1	102050849	rs1601230	C	T			0.0023	0.0205	0.9117
 1	102050851	rs12066303	C	T			-0.1686	0.1459	0.2478
 1	102050924	rs12038083	G	C			-0.0079	0.0202	0.6947
 1	102051020	rs1601229	C	T			-0.0114	0.0193	0.5539
-1	102051057	rs767750840	AT	A			-0.0036	0.0206	0.8632
+1	102051057	rs35815715	AT	A			-0.0036	0.0206	0.8632
 1	102051379	rs11164232	G	T			-0.1983	0.1452	0.172
 1	102051960	rs75191242	C	A			-0.1629	0.1324	0.2185
 1	102052957	rs7518371	C	A			-0.0155	0.0182	0.3925
 1	102053262	rs10874495	C	A			0.0019	0.0205	0.9269
 1	102053315	rs12402573	T	A			-0.0045	0.0209	0.8307
 1	102053346	rs1484300	C	T			-0.1282	0.1235	0.2992
 1	102053450	rs6666387	G	A			-0.0121	0.0192	0.5264
@@ -7972,15 +7972,15 @@
 1	102062743	rs199511204	AT	A			-0.0473	0.0468	0.3123
 1	102062766	rs115261181	C	A			0.0289	0.0465	0.5342
 1	102062792	rs115983585	G	A			0.0273	0.0463	0.5552
 1	102062910	rs138757362	C	T			-0.1589	0.1333	0.2332
 1	102062939	rs182022809	T	A			0.0242	0.0485	0.6178
 1	102062961	rs12127943	G	A			0.037	0.0461	0.4212
 1	102063005	rs147311492	G	A			0.0277	0.046	0.5472
-1	102063037	rs756599093	GT	G			-0.0238	0.046	0.6048
+1	102063037	rs200535234	GT	G			-0.0238	0.046	0.6048
 1	102063289	rs180864381	C	A			0.1399	0.1889	0.4588
 1	102063311	rs144840765	C	T			-0.0216	0.0463	0.64
 1	102063321	rs148500965	C	T			-0.025	0.0464	0.5898
 1	102063350	rs34083855	C	T			-0.0244	0.0381	0.5226
 1	102063407	rs114671021	G	A			0.026	0.0447	0.5605
 1	102063459	rs111431501	T	A			-0.0407	0.045	0.3658
 1	102063568	rs143375459	C	T			0.1495	0.1188	0.2082
@@ -8127,15 +8127,15 @@
 1	102082203	rs60516913	G	A			-0.0148	0.0354	0.6762
 1	102082236	rs10782840	G	A			-0.0134	0.0181	0.4575
 1	102083036	rs186094177	G	A			-0.0367	0.0657	0.5766
 1	102083219	rs12087909	T	A			0.0138	0.0355	0.6971
 1	102083279	rs12135183	C	T			0.0092	0.0211	0.6609
 1	102083360	rs12077819	G	A			-0.0194	0.0279	0.4878
 1	102083452	rs12088000	C	A			0.0219	0.0281	0.4361
-1	102083470	rs1276325387	ATACT	A			-0.1351	0.1366	0.3227
+1	102083470	rs140440461	ATACT	A			-0.1351	0.1366	0.3227
 1	102083543	rs12088053	G	A			0.0108	0.0356	0.7612
 1	102083546	rs12088054	C	A			0.0119	0.0356	0.7374
 1	102083857	rs1484307	T	A			0.0152	0.0354	0.6673
 1	102083992	rs1484306	G	A			0.0148	0.0354	0.6761
 1	102084023	rs144498455	G	A			-0.0217	0.0446	0.6263
 1	102084271	rs1484303	G	A			-0.0145	0.0354	0.6816
 1	102084321	rs35681286	C	T			0.0151	0.0354	0.669
@@ -8227,15 +8227,15 @@
 1	102096070	rs55661599	C	A			0.0148	0.0386	0.7009
 1	102096132	rs12725339	C	T			0.0258	0.0693	0.7098
 1	102096331	rs74507207	G	C			0.1653	0.1323	0.2115
 1	102097028	rs6677725	G	T			-0.0102	0.0195	0.6014
 1	102097036	rs56140505	C	T			0.0208	0.0444	0.6394
 1	102097044	rs111419874	C	T			0.0687	0.0543	0.2055
 1	102097129	rs150856126	G	A			-0.0469	0.1313	0.7207
-1	102097492	rs960941040	TC	T			-0.0164	0.04	0.6809
+1	102097492	rs201848595	TC	T			-0.0164	0.04	0.6809
 1	102097644	rs78693559	C	T			0.1541	0.1314	0.2411
 1	102097651	rs116455498	C	A			-0.0111	0.0407	0.7841
 1	102097905	rs140652582	G	A			-0.002	0.1206	0.9869
 1	102098186	rs4907948	C	T			-0.0286	0.0443	0.5186
 1	102098340	rs12091778	G	C			0.0162	0.0181	0.3702
 1	102098495	rs1872258	T	A			-0.0097	0.0211	0.6451
 1	102098629	rs75406638	C	T			-0.1504	0.1317	0.2534
@@ -8324,46 +8324,46 @@
 1	102119265	rs182622619	C	T			-0.0006	0.1022	0.995
 1	102119338	rs12079191	C	T			-0.0036	0.0374	0.9236
 1	102119641	rs77444674	C	T			0.0006	0.1046	0.9958
 1	102119678	rs57544888	C	T			-0.0034	0.0374	0.9267
 1	102119729	rs56807681	C	T			-0.0032	0.0374	0.9317
 1	102120081	rs76807015	T	A			0.1376	0.0822	0.09396
 1	102120197	rs11800181	G	T			-0.0024	0.0377	0.9499
-1	102120861	rs749298362	C	CAT			0.007	0.0377	0.8518
+1	102120861	rs150184889	C	CAT			0.007	0.0377	0.8518
 1	102121055	rs6660076	C	T			-0.0038	0.0378	0.9205
 1	102121188	rs79631627	G	T			0.0179	0.1036	0.8625
 1	102121356	rs140705432	ACTT	A			0.0058	0.0376	0.8777
 1	102122249	rs80114219	G	A			-0.0266	0.041	0.5157
 1	102122386	rs146959224	C	T			-0.0366	0.1144	0.749
 1	102122574	rs1843112	G	A			0.0139	0.0346	0.6867
 1	102122751	rs67488364	G	A			-0.002	0.0699	0.9775
 1	102123056	rs75839795	G	A			-0.0919	0.1268	0.4686
 1	102123322	rs6679807	G	A			0.0104	0.0382	0.7862
 1	102123337	rs56221742	C	A			0.0012	0.0424	0.9779
-1	102123341	rs1052684194	AT	A			-0.0119	0.039	0.7595
+1	102123341	rs34334304	AT	A			-0.0119	0.039	0.7595
 1	102123413	rs55790574	C	A			0.0152	0.1497	0.9193
 1	102123592	rs34321558	TTC	T			-0.0251	0.0418	0.548
 1	102123799	rs114607615	C	T			-0.0147	0.0546	0.7883
 1	102123839	rs75972044	C	T			0.0155	0.0363	0.6707
-1	102125059	rs112743200	C	CTTCA			-0.0099	0.0372	0.7906
+1	102125059	rs56408336	C	CTTCA			-0.0099	0.0372	0.7906
 1	102125080	rs56011121	TG	T			-0.0338	0.0436	0.4387
 1	102125450	rs56173817	G	T			-0.0147	0.0365	0.6864
 1	102126314	rs72727842	C	A			-0.0108	0.0696	0.8761
 1	102126370	rs1601235	G	A			-0.0057	0.0408	0.8882
 1	102126587	rs150275428	C	T			-0.2327	0.278	0.4025
 1	102126763	rs60629450	C	T			0.0099	0.0377	0.7928
 1	102126827	rs141983138	G	A			-0.0541	0.0866	0.5324
 1	102127240	rs72984783	C	A			-0.0427	0.1122	0.7035
 1	102127439	rs80117870	G	A			-0.0555	0.1136	0.625
 1	102127452	rs9803762	C	T			-0.014	0.0364	0.7009
 1	102127706	rs191559517	G	T			0.1211	0.1618	0.4543
 1	102128325	rs75595526	G	A			-0.0421	0.0462	0.3618
 1	102129075	rs142199975	T	A			-0.0021	0.095	0.9823
 1	102129182	rs58888240	G	A			0.0051	0.0418	0.9037
-1	102129350	rs140071498	GT	G			-0.0123	0.0359	0.7331
+1	102129350	rs60141855	GT	G			-0.0123	0.0359	0.7331
 1	102129493	rs1385124	G	A			0.0078	0.0384	0.8387
 1	102129555	rs1385125	G	C			-0.0062	0.041	0.8799
 1	102129604	rs1385126	C	T			-0.0074	0.0384	0.8472
 1	102129842	rs139011556	C	A			-0.0444	0.115	0.6993
 1	102130144	rs4908172	C	T			0.0103	0.038	0.7865
 1	102130763	rs7550042	C	T			-0.0032	0.0392	0.9354
 1	102130764	rs7512920	G	A			-0.0014	0.0389	0.9719
@@ -8535,15 +8535,15 @@
 1	102189849	rs66781040	TAG	T			0.0033	0.0164	0.8388
 1	102189921	rs148662519	G	C			0.1608	0.1963	0.4127
 1	102190257	rs12740404	T	A			0.0024	0.0164	0.8841
 1	102190446	rs56025619	G	A			0.0209	0.0197	0.288
 1	102190469	rs7547233	G	A			0.0328	0.03	0.2743
 1	102190696	rs74106289	G	A			0.0075	0.0353	0.8312
 1	102190874	rs74396678	T	A			-0.0219	0.0441	0.6197
-1	102191177	rs1015701213	GT	G			0.0257	0.0206	0.2122
+1	102191177	rs11301043	GT	G			0.0257	0.0206	0.2122
 1	102191398	rs61805182	C	T			0.0078	0.0164	0.6359
 1	102191503	rs12126386	G	A			0.0287	0.0298	0.3359
 1	102192265	rs12740577	C	T			-0.0029	0.0356	0.9339
 1	102192559	rs77743406	T	A			-0.0547	0.0572	0.3394
 1	102192809	rs11164280	G	A			-0.0076	0.0354	0.8304
 1	102193273	rs6664594	G	A			-0.0011	0.0347	0.9757
 1	102193300	rs6702059	C	A			-0.0258	0.0202	0.2016
@@ -8593,15 +8593,15 @@
 1	102199912	rs11164285	C	T			0.0116	0.0213	0.5863
 1	102199968	rs78909362	G	A			0.0802	0.0597	0.1787
 1	102200037	rs114543330	G	T			0.0131	0.0489	0.7883
 1	102200090	rs12565816	G	T			-0.0092	0.0167	0.5837
 1	102200154	rs12073778	G	A			-0.0087	0.0353	0.8045
 1	102200551	rs4908176	G	A			0.0114	0.0214	0.5932
 1	102200830	rs4908177	C	A			0.0115	0.0214	0.5926
-1	102200918	rs374893253	GCTGA	G			-0.0123	0.0253	0.6256
+1	102200918	rs10530829	GCTGA	G			-0.0123	0.0253	0.6256
 1	102201064	rs72727871	C	T			0.0085	0.0915	0.9258
 1	102201173	rs146401775	AG	A			0.0139	0.0252	0.5813
 1	102201181	rs142832931	C	T			-0.0006	0.0919	0.9952
 1	102201271	rs79484993	C	T			0.014	0.0253	0.5796
 1	102201705	rs4907953	G	T			-0.0133	0.0252	0.5969
 1	102201856	rs1933244	C	T			-0.0137	0.021	0.5151
 1	102202074	rs11164286	T	A			-0.0147	0.0252	0.5602
@@ -8619,15 +8619,15 @@
 1	102203814	rs12133497	G	A			0.0137	0.0253	0.5887
 1	102203882	rs995269	C	T			0.0102	0.0168	0.5424
 1	102203982	rs12126242	G	A			-0.0231	0.03	0.4398
 1	102204001	rs12133556	G	A			0.0099	0.0253	0.6975
 1	102204021	rs12133561	G	A			0.0111	0.0253	0.6611
 1	102204553	rs191263043	G	T			0.0609	0.2037	0.7649
 1	102204588	rs116462004	C	T			0.0162	0.0439	0.7127
-1	102204772	rs769722962	GT	G			0.0023	0.0364	0.9494
+1	102204772	rs34900166	GT	G			0.0023	0.0364	0.9494
 1	102204857	rs6687256	G	T			-0.0149	0.0252	0.5547
 1	102204906	rs74329572	C	T			-0.4211	0.1403	0.002686
 1	102204919	rs77309032	G	A			-0.0137	0.0253	0.5867
 1	102205485	rs74329224	G	C			0.0144	0.0443	0.7452
 1	102205531	rs80024688	G	T			0.0156	0.0955	0.8704
 1	102205555	rs115421156	T	A			-0.0995	0.0577	0.08445
 1	102205609	rs17427188	C	A			-0.0011	0.0361	0.9756
@@ -8656,28 +8656,28 @@
 1	102209813	rs6686167	G	A			-0.0225	0.0298	0.4501
 1	102209892	rs114926926	C	T			0.0242	0.0452	0.5916
 1	102209933	rs72988816	C	T			-0.0356	0.0203	0.0797
 1	102210078	rs75829441	G	A			0.0133	0.0253	0.5983
 1	102210196	rs115627469	C	A			0.0139	0.0443	0.7537
 1	102210368	rs114724914	C	T			-0.0411	0.0622	0.509
 1	102210427	rs115294608	C	A			-0.0085	0.0441	0.8468
-1	102210487	rs139353882	G	T			-0.066	0.0745	0.3757
+1	102210487	rs188775276	G	T			-0.066	0.0745	0.3757
 1	102210570	rs181196386	G	A			0.0186	0.0467	0.6896
 1	102210578	rs186243963	G	A			-0.026	0.047	0.5794
 1	102210620	rs140847493	G	A			-0.0163	0.0446	0.7152
 1	102210622	rs12037683	G	T			0.0142	0.0213	0.5056
 1	102210768	rs6666029	C	T			0.0062	0.0165	0.7083
 1	102210952	rs79077072	G	A			-0.0098	0.0438	0.8236
 1	102210995	rs77489760	G	T			-0.0143	0.0443	0.7467
 1	102211149	rs75938584	C	T			-0.0125	0.0443	0.7779
 1	102211253	rs34838133	C	T			0.014	0.0213	0.5108
 1	102211705	rs1445222	G	A			-0.0244	0.0179	0.1738
 1	102212006	rs79642708	G	A			-0.0136	0.0438	0.7553
 1	102212256	rs201108742	AC	A			-0.012	0.0442	0.7864
-1	102212418	rs773320650	AAC	A			-0.0121	0.0359	0.7356
+1	102212418	rs147459531	AAC	A			-0.0121	0.0359	0.7356
 1	102212436	rs115564459	C	T			-0.0181	0.0449	0.6876
 1	102212494	rs116829796	G	A			-0.0144	0.0443	0.745
 1	102212582	rs114892828	C	T			-0.0153	0.0442	0.7291
 1	102212791	rs147715657	C	CA			-0.0224	0.0298	0.4533
 1	102213147	rs79090882	C	T			-0.0136	0.0438	0.7557
 1	102213187	rs114035526	G	A			-0.0162	0.0444	0.7162
 1	102213194	rs111501607	T	A			-0.0269	0.0301	0.373
@@ -8944,15 +8944,15 @@
 1	102270859	rs1327593	C	T			0.0251	0.0165	0.1276
 1	102271432	rs1838587	C	T			-0.0238	0.0163	0.1454
 1	102271774	rs4907955	G	A			0.0212	0.0166	0.2005
 1	102271775	rs72729629	C	T			-0.0394	0.0667	0.5552
 1	102272312	rs10874518	C	A			0.0154	0.0171	0.3655
 1	102272701	rs77202016	C	A			0.0356	0.0511	0.4861
 1	102273589	rs75027444	G	A			0.0232	0.0525	0.6588
-1	102273692	rs374661620	C	CAT			-0.0229	0.0165	0.1631
+1	102273692	rs34616565	C	CAT			-0.0229	0.0165	0.1631
 1	102273755	rs149530965	G	A			-0.004	0.1727	0.9814
 1	102273815	rs143967580	AG	A			0.0741	0.0953	0.4365
 1	102273920	rs57341152	AAAGATG	A			0.0244	0.0165	0.1384
 1	102273948	rs10782853	G	T			0.0242	0.0164	0.1408
 1	102274126	rs1854170	G	A			0.0151	0.017	0.3748
 1	102274276	rs1854169	C	T			0.0131	0.0208	0.5294
 1	102274494	rs1327592	T	A			-0.0125	0.0209	0.5479
@@ -9008,15 +9008,15 @@
 1	102291637	rs6659351	G	A			0.0168	0.027	0.5335
 1	102291885	rs6684685	C	A			0.0125	0.0176	0.4794
 1	102292110	rs17470099	C	T			-0.0237	0.0223	0.2869
 1	102292303	rs192895294	C	T			0.2186	0.1396	0.1175
 1	102292310	rs72985992	C	A			-0.0328	0.1088	0.7632
 1	102292385	rs1025975	G	T			-0.0105	0.0176	0.551
 1	102292567	rs4908187	C	A			0.0043	0.0174	0.8058
-1	102293279	rs952217264	GC	G			-0.1083	0.1042	0.2988
+1	102293279	rs201990609	GC	G			-0.1083	0.1042	0.2988
 1	102293284	rs184419703	G	A			0.1026	0.112	0.3596
 1	102293318	rs4908188	G	C			-0.0203	0.0174	0.2421
 1	102293356	rs4908189	C	T			0.0194	0.0174	0.2658
 1	102294173	rs76374953	C	T			-0.1806	0.0962	0.06043
 1	102294391	rs80297308	C	T			0.1909	0.0648	0.003214
 1	102294507	rs6661054	C	T			-0.0113	0.0178	0.5259
 1	102294664	rs6669772	G	A			0.0067	0.0343	0.8451
@@ -9119,15 +9119,15 @@
 1	102318431	rs75566783	C	T			0.0175	0.0248	0.4808
 1	102318881	rs56883975	C	A			-0.0238	0.0924	0.7964
 1	102318895	rs80166472	T	A			0.0793	0.0667	0.2344
 1	102318919	rs9943277	C	A			0.0081	0.017	0.6318
 1	102319027	rs9943151	G	A			-0.0091	0.017	0.5921
 1	102319384	rs12025533	C	T			0.01	0.0921	0.9131
 1	102319387	rs1120398	G	A			-0.0022	0.0166	0.8951
-1	102319808	rs200657342	AC	A			0.0116	0.0703	0.8691
+1	102319808	rs61560407	AC	A			0.0116	0.0703	0.8691
 1	102320291	rs6693196	C	T			-0.0004	0.0166	0.9792
 1	102320487	rs76206689	G	A			0.0573	0.0369	0.1203
 1	102321641	rs17125595	G	C			0.048	0.1158	0.6782
 1	102321856	rs11164314	C	T			0.016	0.0912	0.8607
 1	102321879	rs72729672	C	T			-0.0484	0.11	0.6598
 1	102322008	rs61149341	C	T			-0.0651	0.0648	0.3151
 1	102322439	rs12059847	C	T			0.0165	0.0246	0.5013
@@ -9278,15 +9278,15 @@
 1	102361363	rs148846828	TG	T			-0.0077	0.057	0.8922
 1	102361632	rs2148910	C	A			0.0006	0.018	0.9747
 1	102362302	rs58973440	C	A			-0.0016	0.0568	0.9773
 1	102362505	rs76470651	G	C			0.0479	0.0528	0.3641
 1	102363318	rs17432246	G	A			-0.0022	0.0184	0.9056
 1	102363506	rs145774397	G	A			-0.0197	0.2881	0.9456
 1	102363590	rs138442622	C	T			-0.025	0.0812	0.7586
-1	102363754	rs772282945	C	CTG			0.041	0.0526	0.4365
+1	102363754	rs140727494	C	CTG			0.041	0.0526	0.4365
 1	102364026	rs12120495	C	T			-0.0153	0.0513	0.7659
 1	102364269	rs58587209	G	A			0.0077	0.019	0.6864
 1	102364340	rs12136252	G	A			-0.0002	0.018	0.9926
 1	102364484	rs148527769	C	T			-0.0707	0.0793	0.3732
 1	102364559	rs11809591	C	T			0.004	0.0172	0.817
 1	102364657	rs12748614	C	A			-0.0011	0.0166	0.9488
 1	102364703	rs12730585	C	T			0.0063	0.0181	0.7259
@@ -9318,15 +9318,15 @@
 1	102371076	rs17125705	G	A			0.0157	0.0418	0.7082
 1	102371628	rs77114333	G	A			-0.0389	0.024	0.1045
 1	102371735	rs1360998	G	A			-0.0048	0.0162	0.7676
 1	102372339	rs1998978	G	T			-0.0056	0.0162	0.7296
 1	102372552	rs61808282	C	T			0.0979	0.151	0.5166
 1	102372942	rs72729697	G	A			0.1007	0.1246	0.4192
 1	102373256	rs12564023	C	T			0.0185	0.0416	0.6567
-1	102373434	rs953956079	AT	A			0.0244	0.0434	0.5733
+1	102373434		AT	A			0.0244	0.0434	0.5733
 1	102373567	rs17125714	C	T			0.039	0.0239	0.1018
 1	102373603	rs10782858	G	A			0.0066	0.0162	0.6847
 1	102373957	rs12730852	C	T			0.0013	0.0224	0.9536
 1	102374155	rs78046885	G	A			-0.1157	0.0654	0.0768
 1	102374280	rs728323	C	T			0.0072	0.0167	0.6665
 1	102374343	rs35055361	T	A			0.0012	0.0227	0.9582
 1	102374372	rs1415106	G	A			0.0178	0.0416	0.6693
@@ -9449,15 +9449,15 @@
 1	102399210	rs61285779	C	T			0.0354	0.0396	0.3709
 1	102399464	rs112319850	G	C			-0.2464	0.1392	0.07669
 1	102400076	rs145580622	G	A			0.2571	0.1869	0.1689
 1	102400105	rs7522914	G	A			-0.0125	0.0163	0.443
 1	102400316	rs145319530	C	A			-0.0212	0.1128	0.8512
 1	102400642	rs7548767	G	C			0.2383	0.2275	0.2947
 1	102400668	rs143034268	C	A			-0.0588	0.1085	0.5882
-1	102400840	rs993574467	AG	A			-0.2479	0.2254	0.2715
+1	102400840	rs79598983	AG	A			-0.2479	0.2254	0.2715
 1	102401354	rs76667190	G	C			0.0604	0.0693	0.3837
 1	102401403	rs78817965	C	T			0.0356	0.0396	0.369
 1	102401426	rs12757309	T	A			0.0192	0.0766	0.8025
 1	102401800	rs56747824	C	T			-0.1279	0.2229	0.5661
 1	102402400	rs7531754	G	A			-0.012	0.0163	0.4622
 1	102402745	rs11587732	C	T			0.0357	0.0396	0.3667
 1	102402914	rs80337822	G	T			0.1037	0.0686	0.1303
@@ -9635,15 +9635,15 @@
 1	102435169	rs17125886	G	A			0.0622	0.0486	0.201
 1	102435269	rs146337395	AT	A			0.0483	0.051	0.3438
 1	102435287	rs116801960	G	C			-0.046	0.0511	0.3681
 1	102435833	rs149042335	G	A			0.0454	0.0511	0.3739
 1	102435849	rs138746755	G	A			0.0446	0.0511	0.383
 1	102436038	rs12048155	G	A			-0.0036	0.0172	0.8342
 1	102436157	rs12027913	C	T			0.0031	0.0172	0.8554
-1	102436502	rs775012962	TGCACGTA	T			0.0042	0.0173	0.8084
+1	102436502	rs67605946	TGCACGTA	T			0.0042	0.0173	0.8084
 1	102436599	rs12045775	C	T			-0.0045	0.0172	0.7943
 1	102436727	rs11164352	G	A			0.003	0.0172	0.8594
 1	102437060	rs945727	C	T			-0.0044	0.0172	0.7998
 1	102437203	rs951897	G	A			-0.0042	0.0204	0.8378
 1	102437216	rs945726	G	C			-0.0059	0.0172	0.7306
 1	102437271	rs945725	G	A			0.0066	0.0172	0.7026
 1	102437378	rs12021860	G	A			-0.0048	0.0172	0.7812
```

### Comparing `smunger-0.0.9/tests/exampledata/catalog.munged.txt.gz` & `smunger-0.1.0/tests/exampledata/catalog.munged.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.9/tests/exampledata/catalog.munged.txt.gz.tbi` & `smunger-0.1.0/tests/exampledata/catalog.munged.txt.gz.tbi`

 * *Files identical despite different names*

### Comparing `smunger-0.0.9/tests/exampledata/catalog.txt.gz` & `smunger-0.1.0/tests/exampledata/catalog.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.9/tests/exampledata/test.munged.txt.gz` & `smunger-0.1.0/tests/exampledata/test.munged.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.9/tests/exampledata/test.munged.txt.gz.tbi` & `smunger-0.1.0/tests/exampledata/test.munged.txt.gz.tbi`

 * *Files identical despite different names*

### Comparing `smunger-0.0.9/tests/exampledata/test.txt.gz` & `smunger-0.1.0/tests/exampledata/test.txt.gz`

 * *Files identical despite different names*

### Comparing `smunger-0.0.9/PKG-INFO` & `smunger-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smunger
-Version: 0.0.9
+Version: 0.1.0
 Summary: munger for GWAS summary statistics.
 Home-page: https://github.com/jianhua/smunger
 License: MIT
 Author: Jianhua Wang
 Author-email: jianhua.mert@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,27 +12,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: black (>=22.3.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
 Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "test"
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: liftover (>=1.1.16,<2.0.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.3,<5.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.5.11,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.1.1,<2.0.0)
 Requires-Dist: mkdocstrings[python] (>=0.19.1,<0.20.0) ; extra == "doc"
 Requires-Dist: mypy (>=0.900,<0.901) ; extra == "test"
@@ -40,14 +38,15 @@
 Requires-Dist: pip (>=20.3.1,<21.0.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=2.12.0,<3.0.0) ; extra == "dev"
 Requires-Dist: pytabix (>=0.1,<0.2)
 Requires-Dist: pytest (>=6.2.4,<7.0.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=2.12.0,<3.0.0) ; extra == "test"
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
 Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev"
 Requires-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev"
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
```

