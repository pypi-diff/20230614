# Comparing `tmp/fastaframes-0.0.2.tar.gz` & `tmp/fastaframes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastaframes-0.0.2.tar", last modified: Tue May  2 05:34:08 2023, max compression
+gzip compressed data, was "fastaframes-0.0.3.tar", last modified: Wed Jun 14 21:30:02 2023, max compression
```

## Comparing `fastaframes-0.0.2.tar` & `fastaframes-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:34:08.048781 fastaframes-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-02 05:34:08.048781 fastaframes-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-02 05:33:56.000000 fastaframes-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-02 05:33:56.000000 fastaframes-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:34:08.048781 fastaframes-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-02 05:33:56.000000 fastaframes-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:34:08.044781 fastaframes-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:34:08.044781 fastaframes-0.0.2/src/fastaframes/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-02 05:33:56.000000 fastaframes-0.0.2/src/fastaframes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-02 05:33:56.000000 fastaframes-0.0.2/src/fastaframes/fastaframes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-02 05:33:56.000000 fastaframes-0.0.2/src/fastaframes/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:34:08.044781 fastaframes-0.0.2/src/fastaframes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-02 05:34:08.000000 fastaframes-0.0.2/src/fastaframes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-02 05:34:08.000000 fastaframes-0.0.2/src/fastaframes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:34:08.000000 fastaframes-0.0.2/src/fastaframes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 05:34:08.000000 fastaframes-0.0.2/src/fastaframes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 05:34:08.000000 fastaframes-0.0.2/src/fastaframes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:34:08.048781 fastaframes-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-02 05:33:56.000000 fastaframes-0.0.2/tests/test_description_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-02 05:33:56.000000 fastaframes-0.0.2/tests/test_fastaframes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:30:02.106545 fastaframes-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-14 21:29:50.000000 fastaframes-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-14 21:30:02.106545 fastaframes-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-14 21:29:50.000000 fastaframes-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-14 21:29:50.000000 fastaframes-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:30:02.106545 fastaframes-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-14 21:29:50.000000 fastaframes-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:30:02.102545 fastaframes-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:30:02.102545 fastaframes-0.0.3/src/fastaframes/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 21:29:50.000000 fastaframes-0.0.3/src/fastaframes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-06-14 21:29:50.000000 fastaframes-0.0.3/src/fastaframes/fastaframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-14 21:29:50.000000 fastaframes-0.0.3/src/fastaframes/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:30:02.106545 fastaframes-0.0.3/src/fastaframes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-14 21:30:02.000000 fastaframes-0.0.3/src/fastaframes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-14 21:30:02.000000 fastaframes-0.0.3/src/fastaframes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:30:02.000000 fastaframes-0.0.3/src/fastaframes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 21:30:02.000000 fastaframes-0.0.3/src/fastaframes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 21:30:02.000000 fastaframes-0.0.3/src/fastaframes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:30:02.106545 fastaframes-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-14 21:29:50.000000 fastaframes-0.0.3/tests/test_description_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-06-14 21:29:50.000000 fastaframes-0.0.3/tests/test_fastaframes.py
```

### Comparing `fastaframes-0.0.2/README.md` & `fastaframes-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![example workflow](https://github.com/pgarrett-scripps/FastaFrames/actions/workflows/python-package.yml/badge.svg)
 ![example workflow](https://github.com/pgarrett-scripps/FastaFrames/actions/workflows/pylint.yml/badge.svg)
 
 # FastaFrames
-This Python module provides a set of functions to work with FASTA files. 
+This Python package provides a set of functions to work with FASTA files. 
 It allows you to read FASTA files, convert them to pandas dataframes, manipulate data, 
-and write data back to FASTA files. It also supports converting FASTA files to a list of FastaEntry dataclass objects.
+and write data back to FASTA files. 
 
 ## Features
 - Read FASTA files into pandas DataFrames
 - Write FASTA files from pandas DataFrames
 
 ## Usage
 
@@ -49,15 +49,15 @@
 
 # or
     
 # Write directly to file
 to_fasta(fasta_data=fasta_df, file='output.fasta')
 ```
 
-## Example DataFrame:
+## Example Fasta DataFrame:
 
 |   | db | unique_identifier | entry_name   | protein_name                                         | organism_name | organism_identifier | gene_name | protein_existence | sequence_version | protein_sequence                                       |
 |---|----|------------------|--------------|------------------------------------------------------|---------------|---------------------|-----------|-------------------|------------------|--------------------------------------------------------|
 | 0 | sp | A0A087X1C5       | CP2D7_HUMAN  | Putative cytochrome P450 2D7                         | Homo sapiens  | 9606.0              | CYP2D7    | 5.0               | 1.0              | MGLEALVPLAMIVAIFLLLVDLMHRHQRWAARYPPGPLPLPGLGNLLHVDFQNTPYCFDQ |
 | 1 | sp | A0A0B4J2F2       | SIK1B_HUMAN  | Putative serine/threonine-protein kinase SIK1B        | Homo sapiens  | 9606.0              | SIK1B     | 5.0               | 1.0              | MVIMSEFSADPAGQGQGQQKPLRVGFYDIERTLGKGNFAVVKLARHRVTKTQVAIKIIDKLVQ |
 | 2 | sp | A0A0C5B5G6       | MOTSC_HUMAN  | Mitochondrial-derived peptide MOTS-c                 | Homo sapiens  | 9606.0              | MT-RNR1   | 1.0               | 1.0              | MRWQEMGYIFYPRKLR                                      |
 | 3 | sp | A0A0K2S4Q6       | CD3CH_HUMAN  | Protein CD300H                                       | Homo sapiens  | 9606.0              | CD300H    | 1.0               | 1.0              | MTQRAGAAMLPSALLLLCVPGCLTVSGPSTVMGAVGESLSVQCRYEEKYKTFNKYWCRQP |
```

### Comparing `fastaframes-0.0.2/pyproject.toml` & `fastaframes-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastaframes-0.0.2/src/fastaframes/fastaframes.py` & `fastaframes-0.0.3/src/fastaframes/fastaframes.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dataclasses import dataclass, asdict
 from io import TextIOWrapper, StringIO
 from typing import Union, TextIO, List, Dict, Tuple
 
 import pandas as pd
 
-from fastaframes.util import get_lines, convert_to_best_datatype
+from fastaframes.util import _get_lines, convert_to_best_datatype
 
 
 @dataclass
 class FastaEntry:
     """
     A data class representing a single entry in a FASTA file.
     """
@@ -60,15 +60,15 @@
     Args:
         file_input (Union[str, TextIOWrapper, StringIO, TextIO]): A string or file object containing the FASTA data.
 
     Returns:
         List[FastaEntry]: A list of FastaEntry objects.
     """
 
-    lines = get_lines(file_input)
+    lines = _get_lines(file_input)
 
     entries = []
     for line in lines:
         if line == "":
             continue
 
         if line[0] == ">":  # new protein
@@ -120,16 +120,18 @@
 
     Args:
         fasta_df (pd.DataFrame): The fasta dataframe.
 
     Returns:
         List[FastaEntry]: A list of FastaEntry objects.
     """
+    cols = ['db', 'unique_identifier', 'entry_name', 'protein_name', 'organism_name', 'organism_identifier',
+            'gene_name', 'protein_existence', 'sequence_version', 'protein_sequence']
 
-    entries = [FastaEntry(**row.to_dict()) for _, row in fasta_df.iterrows()]
+    entries = [FastaEntry(**row.to_dict()) for _, row in fasta_df[cols].iterrows()]
     return entries
 
 
 def entries_to_fasta(entries: List[FastaEntry], file: str = None) -> Union[StringIO, None]:
     """
     Converts a list of FastaEntry objects to a StringIO object or file containing the fasta content.
```

### Comparing `fastaframes-0.0.2/src/fastaframes/util.py` & `fastaframes-0.0.3/src/fastaframes/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 """
 This module provides some simple utility functions for filterframes
 """
 
 import os
 from io import TextIOWrapper, StringIO
-from typing import Union, List, TextIO, Any
+from typing import Union, List, TextIO, Any, Generator
 
+FILE_TYPES = Union[str, TextIOWrapper, StringIO, TextIO]
 
-def get_lines(file_input: Union[str, TextIOWrapper, StringIO, TextIO]) -> List[str]:
+
+def _get_lines(file_input: FILE_TYPES) -> Generator[str, None, None]:
     """
+    Retrieve lines from a file or string input.
+
     This function reads lines from a given input, which can be a file path, a string containing lines,
     a TextIOWrapper, or a StringIO object.
 
     Args:
         file_input (Union[str, TextIOWrapper, StringIO]): The input source.
 
     Returns:
-        list: A list of lines from the input source.
+        generator: A generator that yields lines from the input source.
 
     Raises:
         ValueError: If the input type is not supported.
     """
-    if isinstance(file_input, str):
+    if isinstance(file_input, str):  # File path or string
         if os.path.exists(file_input):
             with open(file=file_input, mode='r', encoding='UTF-8') as file:
-                lines = file.read().split('\n')
+                for line in file:
+                    yield line.rstrip('\n')
         else:
-            lines = file_input.split('\n')
-    elif isinstance(file_input, (TextIOWrapper, TextIO)):
-        lines = file_input.read().split('\n')
-
-    elif isinstance(file_input, StringIO):
-        lines = file_input.getvalue().split('\n')
+            for line in file_input.split('\n'):
+                yield line.rstrip('\n')
+    elif isinstance(file_input, (TextIOWrapper, TextIO)):  # TextIOWrapper or StringIO
+        file_input.seek(0)
+        for line in file_input:
+            yield line.rstrip('\n')
+    elif isinstance(file_input, StringIO):  # StringIO
+        file_input.seek(0)
+        for line in file_input.readlines():
+            yield line.rstrip('\n')
     else:
-        raise ValueError(f'Unsupported input type: {type(file_input)}!')
-
-    return lines
+        try:
+            for line in file_input:
+                yield line.decode('UTF-8').rstrip('\n')
+        except Exception as e:
+            raise ValueError(f'Unsupported input type: {type(file_input)}!')
 
 
 def convert_to_best_datatype(values: List[Any]):
     """
     This function tries to convert a list of values to either float, int, or str datatypes, in that order.
 
     Args:
```

### Comparing `fastaframes-0.0.2/tests/test_description_parsing.py` & `fastaframes-0.0.3/tests/test_description_parsing.py`

 * *Files identical despite different names*

### Comparing `fastaframes-0.0.2/tests/test_fastaframes.py` & `fastaframes-0.0.3/tests/test_fastaframes.py`

 * *Files identical despite different names*

