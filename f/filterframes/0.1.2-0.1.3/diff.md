# Comparing `tmp/filterframes-0.1.2.tar.gz` & `tmp/filterframes-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filterframes-0.1.2.tar", last modified: Mon May  1 06:46:16 2023, max compression
+gzip compressed data, was "filterframes-0.1.3.tar", last modified: Wed Jun 14 21:29:13 2023, max compression
```

## Comparing `filterframes-0.1.2.tar` & `filterframes-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.899396 filterframes-0.1.2/
--rw-rw-rw-   0        0        0     1093 2023-05-01 06:00:47.000000 filterframes-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5832 2023-05-01 06:46:16.891358 filterframes-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3950 2023-05-01 06:23:52.000000 filterframes-0.1.2/README.md
--rw-rw-rw-   0        0        0      929 2023-05-01 06:19:29.000000 filterframes-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 06:46:16.899396 filterframes-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      220 2023-05-01 03:56:38.000000 filterframes-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.874764 filterframes-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.882762 filterframes-0.1.2/src/filterframes/
--rw-rw-rw-   0        0        0      249 2023-05-01 04:47:21.000000 filterframes-0.1.2/src/filterframes/__init__.py
--rw-rw-rw-   0        0        0    10679 2023-05-01 06:00:47.000000 filterframes-0.1.2/src/filterframes/filterframes.py
-drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.891358 filterframes-0.1.2/src/filterframes.egg-info/
--rw-rw-rw-   0        0        0     5832 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 06:46:16.000000 filterframes-0.1.2/src/filterframes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 06:46:16.891358 filterframes-0.1.2/tests/
--rw-rw-rw-   0        0        0     1907 2023-05-01 04:56:24.000000 filterframes-0.1.2/tests/test_filterframes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:29:13.726827 filterframes-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-14 21:29:01.000000 filterframes-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-14 21:29:13.726827 filterframes-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-14 21:29:01.000000 filterframes-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-14 21:29:01.000000 filterframes-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:29:13.726827 filterframes-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-14 21:29:01.000000 filterframes-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:29:13.722827 filterframes-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:29:13.726827 filterframes-0.1.3/src/filterframes/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-14 21:29:01.000000 filterframes-0.1.3/src/filterframes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-06-14 21:29:01.000000 filterframes-0.1.3/src/filterframes/filterframes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:29:13.726827 filterframes-0.1.3/src/filterframes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-14 21:29:13.000000 filterframes-0.1.3/src/filterframes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-14 21:29:13.000000 filterframes-0.1.3/src/filterframes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:29:13.000000 filterframes-0.1.3/src/filterframes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 21:29:13.000000 filterframes-0.1.3/src/filterframes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 21:29:13.000000 filterframes-0.1.3/src/filterframes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:29:13.726827 filterframes-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-14 21:29:01.000000 filterframes-0.1.3/tests/test_filterframes.py
```

### Comparing `filterframes-0.1.2/LICENSE` & `filterframes-0.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Patrick Garrett
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Patrick Garrett
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `filterframes-0.1.2/PKG-INFO` & `filterframes-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-Metadata-Version: 2.1
-Name: filterframes
-Version: 0.1.2
-Summary: A very simple DTASelect-Filter.txt parser.
-Author-email: Patrick Garrett <pgarrett@scripps.edu>
-License: MIT License
-        
-        Copyright (c) 2023 Patrick Garrett
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: repository, https://github.com/pgarrett-scripps/FilterFrames.git
-Keywords: IP2,PASER,Parser,Streamlit,DTASelect-filter,Peptide,Protein,Proteomics
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/python-package.yml/badge.svg)
-![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/pylint.yml/badge.svg)
-
-# filterframes
-
-filterframes is a Python package that provides an easy way to parse and manipulate DTASelect filter 
-files using pandas. The package allows you to read DTASelect-filter.txt files, create peptide and protein dataframes, 
-modify the dataframes, and write the modified dataframes back to a new DTASelect-filter.txt file. 
-
-### Note on dataframe columns:
-
-The column names in the peptide and protein dataframes will correspond to the header lines in the DTASelect-filter.txt
-files. In order to edit and output a valid DTASelect-filter file you must ensure that the
-peptide and protein dataframe column names and order are conserved, and that no additional columns are 
-included. Any changes in the columns order or names will be reflected  in the output DTASelect-filter.txt file.
-
-## Installation
-
-You can install filterframes using pip:
-
-```sh
-pip install filterframes
-```
-
-You can also install filterframes locally:
-
-```sh
-git clone https://github.com/pgarrett-scripps/FilterFrames.git
-cd filterframes
-pip install .
-```
-
-## Usage
-
-Here are some basic examples of how to use the package:
-
-### Example Python Script:
-```python
-from filterframes import from_dta_select_filter, to_dta_select_filter
-
-# Read DTASelect-filter.txt file and create peptide and protein dataframes
-file_input = r'tests/data/DTASelect-filter_V2_1_12_paser.txt'
-header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(file_input)
-
-# Display the first 5 rows of the peptide and protein dataframes
-print("Peptide DataFrame:")
-print(peptide_df.head())
-print("\nProtein DataFrame:")
-print(protein_df.head())
-
-# Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
-# ...
-
-# Write modified peptide and protein dataframes back to a DTASelect-filter.txt file
-file_output = r'tests/data/DTASelect-filter_V2_1_12_paser.out.txt'
-with open(file_output, 'w') as f:
-    output_string_io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
-    f.write(output_string_io.getvalue())
-
-print(f"\nModified DTASelect-filter.txt file saved to {file_output}")
-```
-
-### Example Streamlit App:
-
-```python
-# app.py
-from io import StringIO
-
-import streamlit as st
-from filterframes import from_dta_select_filter, to_dta_select_filter
-
-uploaded_filter_file = st.file_uploader("Choose a DTASelect-filter.txt file", type="txt")
-
-if uploaded_filter_file:
-    header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(StringIO(uploaded_filter_file.getvalue().decode('utf-8')))
-    
-    st.header('Peptide df')
-    st.dataframe(peptide_df)
-    st.header('Protein df')
-    st.dataframe(protein_df)
-
-    # Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
-    # ...
-
-    io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
-
-    st.download_button(label="Download Filter",
-                       data=io.getvalue(),
-                       file_name="DTASelect-filter.txt",
-                       mime="text/plain")
-```
-
-## Functions
-The main functions provided by the package are:
-
-
-```
-from_dta_select_filter(file_input: Union[str, TextIOWrapper, StringIO]) -> Tuple[List[str], pd.DataFrame, pd.DataFrame, List[str]]
-```
-
-Reads a DTASelect-filter.txt file and returns header lines, peptide dataframe, protein dataframe, and end lines.
-
-
-```
-to_dta_select_filter(header_lines: List[str], peptide_df: pd.DataFrame, protein_df: pd.DataFrame, end_lines: List[str]) -> StringIO
-```
-
-Writes the given header lines, peptide dataframe, protein dataframe, and end lines to a StringIO object in the DTASelect-filter.txt format.
-
+Metadata-Version: 2.1
+Name: filterframes
+Version: 0.1.3
+Summary: A very simple DTASelect-Filter.txt parser.
+Author-email: Patrick Garrett <pgarrett@scripps.edu>
+License: MIT License
+        
+        Copyright (c) 2023 Patrick Garrett
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/pgarrett-scripps/FilterFrames.git
+Keywords: IP2,PASER,Parser,Streamlit,DTASelect-filter,Peptide,Protein,Proteomics
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/python-package.yml/badge.svg)
+![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/pylint.yml/badge.svg)
+
+# filterframes
+
+filterframes is a Python package that provides an easy way to parse and manipulate DTASelect filter 
+files using pandas. The package allows you to read DTASelect-filter.txt files, create peptide and protein dataframes, 
+modify the dataframes, and write the modified dataframes back to a new DTASelect-filter.txt file. 
+
+### Note on dataframe columns:
+
+The column names in the peptide and protein dataframes will correspond to the header lines in the DTASelect-filter.txt
+files. In order to edit and output a valid DTASelect-filter file you must ensure that the
+peptide and protein dataframe column names and order are conserved, and that no additional columns are 
+included. Any changes in the columns order or names will be reflected  in the output DTASelect-filter.txt file.
+
+## Installation
+
+You can install filterframes using pip:
+
+```sh
+pip install filterframes
+```
+
+You can also install filterframes locally:
+
+```sh
+git clone https://github.com/pgarrett-scripps/FilterFrames.git
+cd filterframes
+pip install .
+```
+
+## Usage
+
+Here are some basic examples of how to use the package:
+
+### Example Python Script:
+```python
+from filterframes import from_dta_select_filter, to_dta_select_filter
+
+# Read DTASelect-filter.txt file and create peptide and protein dataframes
+file_input = r'tests/data/DTASelect-filter_V2_1_12_paser.txt'
+header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(file_input)
+
+# Display the first 5 rows of the peptide and protein dataframes
+print("Peptide DataFrame:")
+print(peptide_df.head())
+print("\nProtein DataFrame:")
+print(protein_df.head())
+
+# Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
+# ...
+
+# Write modified peptide and protein dataframes back to a DTASelect-filter.txt file
+file_output = r'tests/data/DTASelect-filter_V2_1_12_paser.out.txt'
+with open(file_output, 'w') as f:
+    output_string_io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
+    f.write(output_string_io.getvalue())
+
+print(f"\nModified DTASelect-filter.txt file saved to {file_output}")
+```
+
+### Example Streamlit App:
+
+```python
+# app.py
+from io import StringIO
+
+import streamlit as st
+from filterframes import from_dta_select_filter, to_dta_select_filter
+
+uploaded_filter_file = st.file_uploader("Choose a DTASelect-filter.txt file", type="txt")
+
+if uploaded_filter_file:
+    header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(StringIO(uploaded_filter_file.getvalue().decode('utf-8')))
+    
+    st.header('Peptide df')
+    st.dataframe(peptide_df)
+    st.header('Protein df')
+    st.dataframe(protein_df)
+
+    # Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
+    # ...
+
+    io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
+
+    st.download_button(label="Download Filter",
+                       data=io.getvalue(),
+                       file_name="DTASelect-filter.txt",
+                       mime="text/plain")
+```
+
+## Functions
+The main functions provided by the package are:
+
+
+```
+from_dta_select_filter(file_input: Union[str, TextIOWrapper, StringIO]) -> Tuple[List[str], pd.DataFrame, pd.DataFrame, List[str]]
+```
+
+Reads a DTASelect-filter.txt file and returns header lines, peptide dataframe, protein dataframe, and end lines.
+
+
+```
+to_dta_select_filter(header_lines: List[str], peptide_df: pd.DataFrame, protein_df: pd.DataFrame, end_lines: List[str]) -> StringIO
+```
+
+Writes the given header lines, peptide dataframe, protein dataframe, and end lines to a StringIO object in the DTASelect-filter.txt format.
+
```

### Comparing `filterframes-0.1.2/README.md` & `filterframes-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/python-package.yml/badge.svg)
-![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/pylint.yml/badge.svg)
-
-# filterframes
-
-filterframes is a Python package that provides an easy way to parse and manipulate DTASelect filter 
-files using pandas. The package allows you to read DTASelect-filter.txt files, create peptide and protein dataframes, 
-modify the dataframes, and write the modified dataframes back to a new DTASelect-filter.txt file. 
-
-### Note on dataframe columns:
-
-The column names in the peptide and protein dataframes will correspond to the header lines in the DTASelect-filter.txt
-files. In order to edit and output a valid DTASelect-filter file you must ensure that the
-peptide and protein dataframe column names and order are conserved, and that no additional columns are 
-included. Any changes in the columns order or names will be reflected  in the output DTASelect-filter.txt file.
-
-## Installation
-
-You can install filterframes using pip:
-
-```sh
-pip install filterframes
-```
-
-You can also install filterframes locally:
-
-```sh
-git clone https://github.com/pgarrett-scripps/FilterFrames.git
-cd filterframes
-pip install .
-```
-
-## Usage
-
-Here are some basic examples of how to use the package:
-
-### Example Python Script:
-```python
-from filterframes import from_dta_select_filter, to_dta_select_filter
-
-# Read DTASelect-filter.txt file and create peptide and protein dataframes
-file_input = r'tests/data/DTASelect-filter_V2_1_12_paser.txt'
-header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(file_input)
-
-# Display the first 5 rows of the peptide and protein dataframes
-print("Peptide DataFrame:")
-print(peptide_df.head())
-print("\nProtein DataFrame:")
-print(protein_df.head())
-
-# Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
-# ...
-
-# Write modified peptide and protein dataframes back to a DTASelect-filter.txt file
-file_output = r'tests/data/DTASelect-filter_V2_1_12_paser.out.txt'
-with open(file_output, 'w') as f:
-    output_string_io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
-    f.write(output_string_io.getvalue())
-
-print(f"\nModified DTASelect-filter.txt file saved to {file_output}")
-```
-
-### Example Streamlit App:
-
-```python
-# app.py
-from io import StringIO
-
-import streamlit as st
-from filterframes import from_dta_select_filter, to_dta_select_filter
-
-uploaded_filter_file = st.file_uploader("Choose a DTASelect-filter.txt file", type="txt")
-
-if uploaded_filter_file:
-    header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(StringIO(uploaded_filter_file.getvalue().decode('utf-8')))
-    
-    st.header('Peptide df')
-    st.dataframe(peptide_df)
-    st.header('Protein df')
-    st.dataframe(protein_df)
-
-    # Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
-    # ...
-
-    io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
-
-    st.download_button(label="Download Filter",
-                       data=io.getvalue(),
-                       file_name="DTASelect-filter.txt",
-                       mime="text/plain")
-```
-
-## Functions
-The main functions provided by the package are:
-
-
-```
-from_dta_select_filter(file_input: Union[str, TextIOWrapper, StringIO]) -> Tuple[List[str], pd.DataFrame, pd.DataFrame, List[str]]
-```
-
-Reads a DTASelect-filter.txt file and returns header lines, peptide dataframe, protein dataframe, and end lines.
-
-
-```
-to_dta_select_filter(header_lines: List[str], peptide_df: pd.DataFrame, protein_df: pd.DataFrame, end_lines: List[str]) -> StringIO
-```
-
-Writes the given header lines, peptide dataframe, protein dataframe, and end lines to a StringIO object in the DTASelect-filter.txt format.
-
+![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/python-package.yml/badge.svg)
+![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/pylint.yml/badge.svg)
+
+# filterframes
+
+filterframes is a Python package that provides an easy way to parse and manipulate DTASelect filter 
+files using pandas. The package allows you to read DTASelect-filter.txt files, create peptide and protein dataframes, 
+modify the dataframes, and write the modified dataframes back to a new DTASelect-filter.txt file. 
+
+### Note on dataframe columns:
+
+The column names in the peptide and protein dataframes will correspond to the header lines in the DTASelect-filter.txt
+files. In order to edit and output a valid DTASelect-filter file you must ensure that the
+peptide and protein dataframe column names and order are conserved, and that no additional columns are 
+included. Any changes in the columns order or names will be reflected  in the output DTASelect-filter.txt file.
+
+## Installation
+
+You can install filterframes using pip:
+
+```sh
+pip install filterframes
+```
+
+You can also install filterframes locally:
+
+```sh
+git clone https://github.com/pgarrett-scripps/FilterFrames.git
+cd filterframes
+pip install .
+```
+
+## Usage
+
+Here are some basic examples of how to use the package:
+
+### Example Python Script:
+```python
+from filterframes import from_dta_select_filter, to_dta_select_filter
+
+# Read DTASelect-filter.txt file and create peptide and protein dataframes
+file_input = r'tests/data/DTASelect-filter_V2_1_12_paser.txt'
+header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(file_input)
+
+# Display the first 5 rows of the peptide and protein dataframes
+print("Peptide DataFrame:")
+print(peptide_df.head())
+print("\nProtein DataFrame:")
+print(protein_df.head())
+
+# Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
+# ...
+
+# Write modified peptide and protein dataframes back to a DTASelect-filter.txt file
+file_output = r'tests/data/DTASelect-filter_V2_1_12_paser.out.txt'
+with open(file_output, 'w') as f:
+    output_string_io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
+    f.write(output_string_io.getvalue())
+
+print(f"\nModified DTASelect-filter.txt file saved to {file_output}")
+```
+
+### Example Streamlit App:
+
+```python
+# app.py
+from io import StringIO
+
+import streamlit as st
+from filterframes import from_dta_select_filter, to_dta_select_filter
+
+uploaded_filter_file = st.file_uploader("Choose a DTASelect-filter.txt file", type="txt")
+
+if uploaded_filter_file:
+    header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(StringIO(uploaded_filter_file.getvalue().decode('utf-8')))
+    
+    st.header('Peptide df')
+    st.dataframe(peptide_df)
+    st.header('Protein df')
+    st.dataframe(protein_df)
+
+    # Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
+    # ...
+
+    io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
+
+    st.download_button(label="Download Filter",
+                       data=io.getvalue(),
+                       file_name="DTASelect-filter.txt",
+                       mime="text/plain")
+```
+
+## Functions
+The main functions provided by the package are:
+
+
+```
+from_dta_select_filter(file_input: Union[str, TextIOWrapper, StringIO]) -> Tuple[List[str], pd.DataFrame, pd.DataFrame, List[str]]
+```
+
+Reads a DTASelect-filter.txt file and returns header lines, peptide dataframe, protein dataframe, and end lines.
+
+
+```
+to_dta_select_filter(header_lines: List[str], peptide_df: pd.DataFrame, protein_df: pd.DataFrame, end_lines: List[str]) -> StringIO
+```
+
+Writes the given header lines, peptide dataframe, protein dataframe, and end lines to a StringIO object in the DTASelect-filter.txt format.
+
```

### Comparing `filterframes-0.1.2/src/filterframes/filterframes.py` & `filterframes-0.1.3/src/filterframes/filterframes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,288 +1,299 @@
-"""Module providing function for converting between DTASelectFilter.tx files and pandas DataFrame objects"""
-import os
-from enum import Enum
-from io import TextIOWrapper, StringIO
-from typing import List, Union, Any, TextIO
-
-import pandas as pd
-
-
-def _get_lines(file_input: Union[str, TextIOWrapper, StringIO, TextIO]):
-    """
-    Retrieve lines from a file or string input.
-
-    This function reads lines from a given input, which can be a file path, a string containing lines,
-    a TextIOWrapper, or a StringIO object.
-
-    Args:
-        file_input (Union[str, TextIOWrapper, StringIO]): The input source.
-
-    Returns:
-        list: A list of lines from the input source.
-
-    Raises:
-        ValueError: If the input type is not supported.
-    """
-    if isinstance(file_input, str):
-        if os.path.exists(file_input):
-            with open(file=file_input, mode='r', encoding='UTF-8') as file:
-                lines = file.read().split('\n')
-        else:
-            lines = file_input.split('\n')
-    elif isinstance(file_input, (TextIOWrapper, TextIO)):
-        lines = file_input.read().split('\n')
-
-    elif isinstance(file_input, StringIO):
-        lines = file_input.getvalue().split('\n')
-    else:
-        raise ValueError(f'Unsupported input type: {type(file_input)}!')
-
-    return lines[:-1]
-
-
-def _convert_to_best_datatype(values: List[Any]):
-    """
-    Convert a list of values to the most suitable datatype.
-
-    This function tries to convert a list of values to either float, int, or str datatypes, in that order.
-
-    Args:
-        values (List[Any]): A list of values to be converted.
-
-    Returns:
-        list: A list of converted values.
-
-    Raises:
-        ValueError: If unable to convert values to any datatype.
-    """
-
-    for datatype in [float, int, str]:
-        try:
-            converted_values = [datatype(value) for value in values]
-            return converted_values
-        except (ValueError, TypeError):
-            continue
-    raise ValueError("Unable to convert values to any datatype")
-
-
-def _create_file_name(peptide_row: pd.Series) -> str:
-    """
-    Create a file name from a given peptide row.
-
-    This function constructs a file name string from the FileName, LowScan, HighScan, and Charge
-    fields of a given peptide row.
-
-    Args:
-        peptide_row (pd.Series): A row from a peptide dataframe.
-
-    Returns:
-        str: The constructed file name string.
-    """
-
-    return f"{peptide_row['FileName']}.{peptide_row['LowScan']}.{peptide_row['HighScan']}.{peptide_row['Charge']}"
-
-
-def _reorder_columns(dataframe: pd.DataFrame, column: str, new_position: int) -> pd.DataFrame:
-    """
-    Reorder columns in a dataframe by moving a specified column to a new position.
-
-    Args:
-        df (pd.DataFrame): The input dataframe.
-        column (str): The column to be moved.
-        new_position (int): The new position for the specified column.
-
-    Returns:
-        pd.DataFrame: A dataframe with reordered columns.
-    """
-
-    columns = dataframe.columns.tolist()
-    columns.insert(new_position, columns.pop(columns.index(column)))
-    return dataframe[columns]
-
-
-def _write_lines(file_output, lines):
-    """
-    Write a list of lines to a given file output.
-
-    Args:
-        file_output (TextIOWrapper or StringIO): The output file object.
-        lines (list): A list of lines to be written.
-    """
-
-    for line in lines:
-        file_output.write(line + '\n')
-
-
-def from_dta_select_filter(file_input: Union[str, TextIOWrapper, StringIO, TextIO]) -> (
-        List[str], pd.DataFrame, pd.DataFrame, List[str]):
-    """
-    Process the given file and extract relevant information to create peptide and protein dataframes.
-
-    This function reads the input file and processes it line by line to create peptide and protein
-    dataframes, as well as lists of header lines and end lines (information lines).
-
-    Args:
-        file_input (Union[str, TextIOWrapper, StringIO]): The input file as a string, TextIOWrapper, or StringIO.
-
-    Returns:
-        tuple: A tuple containing the following elements:
-            - header_lines (List[str]): A list of header lines.
-            - peptide_df (pd.DataFrame): A dataframe containing peptide data.
-            - protein_df (pd.DataFrame): A dataframe containing protein data.
-            - end_lines (List[str]): A list of end lines (information lines).
-    """
-
-    lines = _get_lines(file_input)
-
-    class FileState(Enum):
-        """
-        Enum for specifying the different parts of the DTASelect-filter.txt file
-        """
-        HEADER = 1
-        DATA = 2
-        INFO = 3
-
-    file_state = FileState.HEADER
-
-    header_lines, end_lines = [], []
-    peptide_data, protein_data = None, None
-    current_protein_grp, peptide_line_cnt = 0, 0
-
-    for line in lines:
-        line_elements = line.rstrip().split("\t")
-
-        if line.startswith('Locus'):  # Protein Line Header
-            protein_data = {key: [] for key in line_elements}
-            protein_data['ProteinGroup'] = []
-
-        if line.startswith('Unique'):  # Peptide Line Header
-            peptide_data = {key: [] for key in line_elements}
-            peptide_data['ProteinGroup'] = []
-
-        # Update file state
-        if len(line_elements) > 0 and line_elements[0] == 'Unique':
-            header_lines.append(line)
-            file_state = FileState.DATA
-            continue
-
-        if len(line_elements) > 1 and line_elements[1] == "Proteins":
-            file_state = FileState.INFO
-
-        if file_state == FileState.HEADER:
-            header_lines.append(line)
-
-        if file_state == FileState.DATA:
-            if line_elements[0] == '' or '*' in line_elements[0] or line_elements[0].isnumeric():
-                for key, value in zip(peptide_data, line_elements):
-                    peptide_data[key].append(value)
-                peptide_data['ProteinGroup'].append(current_protein_grp)
-
-                peptide_line_cnt += 1
-            else:
-                if peptide_line_cnt != 0:
-                    current_protein_grp += 1
-                    peptide_line_cnt = 0
-
-                for key, value in zip(protein_data, line_elements):
-                    protein_data[key].append(value)
-                protein_data['ProteinGroup'].append(current_protein_grp)
-
-        if file_state == FileState.INFO:
-            end_lines.append(line)
-
-    for k in peptide_data:
-        peptide_data[k] = _convert_to_best_datatype(peptide_data[k])
-
-    for k in protein_data:
-        protein_data[k] = _convert_to_best_datatype(protein_data[k])
-
-    peptide_df = pd.DataFrame(peptide_data)
-    protein_df = pd.DataFrame(protein_data)
-
-    file_name_components = [fn.split('.') for fn in peptide_df['FileName']]
-    peptide_df.drop(['FileName'], axis=1, inplace=True)
-
-    peptide_df['FileName'] = _convert_to_best_datatype([comp[0] for comp in file_name_components])
-    peptide_df['FileName'] = peptide_df['FileName'].astype('category')
-
-    peptide_df['LowScan'] = _convert_to_best_datatype([comp[1] for comp in file_name_components])
-    peptide_df['HighScan'] = _convert_to_best_datatype([comp[2] for comp in file_name_components])
-    peptide_df['Charge'] = _convert_to_best_datatype([comp[3] for comp in file_name_components])
-
-    peptide_df = peptide_df.convert_dtypes()
-    protein_df = protein_df.convert_dtypes()
-
-    return header_lines, peptide_df, protein_df, end_lines
-
-
-def to_dta_select_filter(header_lines: List[str], peptide_df: pd.DataFrame, protein_df: pd.DataFrame,
-                         end_lines: List[str]) -> StringIO:
-    """
-    Convert the given header lines, peptide and protein dataframes, and end lines into a StringIO object.
-
-    This function takes the header lines, peptide and protein dataframes, and end lines as inputs, and writes
-    them into a StringIO object in the DTASelect-filter.txt format.
-
-    Args:
-        header_lines (List[str]): A list of header lines.
-        peptide_df (pd.DataFrame): A dataframe containing peptide data.
-        protein_df (pd.DataFrame): A dataframe containing protein data.
-        end_lines (List[str]): A list of end lines (information lines).
-
-    Returns:
-        StringIO: A StringIO object containing the reformatted data in DTASelect-filter.txt format.
-    """
-
-    peptide_df = peptide_df.copy(deep=True)
-    protein_df = protein_df.copy(deep=True)
-
-    file_output = StringIO()
-
-    # Write header lines
-    _write_lines(file_output, header_lines)
-
-    # Write protein and peptide data
-    concatenated_file_names = peptide_df.apply(_create_file_name, axis=1)
-    peptide_df.drop(['FileName', 'LowScan', 'HighScan', 'Charge'], axis=1, inplace=True)
-    peptide_df['FileName'] = concatenated_file_names
-    # Re-order columns to make FileName the second column
-    peptide_df = _reorder_columns(peptide_df, 'FileName', 1)
-
-    protein_data_str = protein_df.drop(['ProteinGroup'], axis=1).to_csv(header=False, index=False, sep='\t')
-    peptide_data_str = peptide_df.drop(['ProteinGroup'], axis=1).to_csv(header=False, index=False, sep='\t')
-
-    protein_data_str = protein_data_str.replace('\r', '')
-    peptide_data_str = peptide_data_str.replace('\r', '')
-
-    current_protein_grp = 0
-    protein_lines = protein_data_str.split('\n')
-    peptide_lines = peptide_data_str.split('\n')
-
-    if protein_lines[-1] == '':
-        protein_lines = protein_lines[:-1]
-
-    if peptide_lines[-1] == '':
-        peptide_lines = peptide_lines[:-1]
-
-    protein_line_idx = 0
-    peptide_line_idx = 0
-
-    while protein_line_idx < len(protein_lines) and peptide_line_idx < len(peptide_lines):
-        if int(protein_df.iloc[protein_line_idx]['ProteinGroup']) == current_protein_grp:
-            file_output.write(protein_lines[protein_line_idx] + '\n')
-            protein_line_idx += 1
-        else:
-            file_output.write(peptide_lines[peptide_line_idx] + '\n')
-            peptide_line_idx += 1
-            if peptide_line_idx < len(peptide_lines) and int(
-                    peptide_df.iloc[peptide_line_idx - 1]['ProteinGroup']) != int(
-                peptide_df.iloc[peptide_line_idx]['ProteinGroup']):
-                current_protein_grp += 1
-
-    # Write remaining protein and peptide lines
-    _write_lines(file_output, protein_lines[protein_line_idx:])
-    _write_lines(file_output, peptide_lines[peptide_line_idx:])
-
-    _write_lines(file_output, end_lines)
-
-    return file_output
+"""Module providing function for converting between DTASelectFilter.tx files and pandas DataFrame objects"""
+import os
+from enum import Enum
+from io import TextIOWrapper, StringIO
+from typing import List, Union, Any, TextIO, Generator
+
+import pandas as pd
+
+FILE_TYPES = Union[str, TextIOWrapper, StringIO, TextIO]
+
+
+def _get_lines(file_input: FILE_TYPES) -> Generator[str, None, None]:
+    """
+    Retrieve lines from a file or string input.
+
+    This function reads lines from a given input, which can be a file path, a string containing lines,
+    a TextIOWrapper, or a StringIO object.
+
+    Args:
+        file_input (Union[str, TextIOWrapper, StringIO]): The input source.
+
+    Returns:
+        generator: A generator that yields lines from the input source.
+
+    Raises:
+        ValueError: If the input type is not supported.
+    """
+    if isinstance(file_input, str): # File path or string
+        if os.path.exists(file_input):
+            with open(file=file_input, mode='r', encoding='UTF-8') as file:
+                for line in file:
+                    yield line.rstrip('\n')
+        else:
+            for line in file_input.split('\n'):
+                yield line.rstrip('\n')
+    elif isinstance(file_input, (TextIOWrapper, TextIO)): # TextIOWrapper or StringIO
+        file_input.seek(0)
+        for line in file_input:
+            yield line.rstrip('\n')
+    elif isinstance(file_input, StringIO): # StringIO
+        file_input.seek(0)
+        for line in file_input.readlines():
+            yield line.rstrip('\n')
+    else:
+        try:
+            for line in file_input:
+                yield line.decode('UTF-8').rstrip('\n')
+        except Exception as e:
+            raise ValueError(f'Unsupported input type: {type(file_input)}!')
+
+
+def _convert_to_best_datatype(values: List[Any]):
+    """
+    Convert a list of values to the most suitable datatype.
+
+    This function tries to convert a list of values to either float, int, or str datatypes, in that order.
+
+    Args:
+        values (List[Any]): A list of values to be converted.
+
+    Returns:
+        list: A list of converted values.
+
+    Raises:
+        ValueError: If unable to convert values to any datatype.
+    """
+
+    for datatype in [float, int, str]:
+        try:
+            converted_values = [datatype(value) for value in values]
+            return converted_values
+        except (ValueError, TypeError):
+            continue
+    raise ValueError("Unable to convert values to any datatype")
+
+
+def _create_file_name(peptide_row: pd.Series) -> str:
+    """
+    Create a file name from a given peptide row.
+
+    This function constructs a file name string from the FileName, LowScan, HighScan, and Charge
+    fields of a given peptide row.
+
+    Args:
+        peptide_row (pd.Series): A row from a peptide dataframe.
+
+    Returns:
+        str: The constructed file name string.
+    """
+
+    return f"{peptide_row['FileName']}.{peptide_row['LowScan']}.{peptide_row['HighScan']}.{peptide_row['Charge']}"
+
+
+def _reorder_columns(dataframe: pd.DataFrame, column: str, new_position: int) -> pd.DataFrame:
+    """
+    Reorder columns in a dataframe by moving a specified column to a new position.
+
+    Args:
+        dataframe (pd.DataFrame): The input dataframe.
+        column (str): The column to be moved.
+        new_position (int): The new position for the specified column.
+
+    Returns:
+        pd.DataFrame: A dataframe with reordered columns.
+    """
+
+    columns = dataframe.columns.tolist()
+    columns.insert(new_position, columns.pop(columns.index(column)))
+    return dataframe[columns]
+
+
+def _write_lines(file_output, lines):
+    """
+    Write a list of lines to a given file output.
+
+    Args:
+        file_output (TextIOWrapper or StringIO): The output file object.
+        lines (list): A list of lines to be written.
+    """
+
+    for line in lines:
+        file_output.write(line + '\n')
+
+
+def from_dta_select_filter(file_input: Union[str, TextIOWrapper, StringIO, TextIO]) -> (
+        List[str], pd.DataFrame, pd.DataFrame, List[str]):
+    """
+    Process the given file and extract relevant information to create peptide and protein dataframes.
+
+    This function reads the input file and processes it line by line to create peptide and protein
+    dataframes, as well as lists of header lines and end lines (information lines).
+
+    Args:
+        file_input (Union[str, TextIOWrapper, StringIO]): The input file as a string, TextIOWrapper, or StringIO.
+
+    Returns:
+        tuple: A tuple containing the following elements:
+            - header_lines (List[str]): A list of header lines.
+            - peptide_df (pd.DataFrame): A dataframe containing peptide data.
+            - protein_df (pd.DataFrame): A dataframe containing protein data.
+            - end_lines (List[str]): A list of end lines (information lines).
+    """
+
+    lines = _get_lines(file_input)
+
+    class FileState(Enum):
+        """
+        Enum for specifying the different parts of the DTASelect-filter.txt file
+        """
+        HEADER = 1
+        DATA = 2
+        INFO = 3
+
+    file_state = FileState.HEADER
+
+    header_lines, end_lines = [], []
+    peptide_data, protein_data = None, None
+    current_protein_grp, peptide_line_cnt = 0, 0
+
+    for i, line in enumerate(lines):
+        line_elements = line.rstrip().split("\t")
+
+        if line.startswith('Locus'):  # Protein Line Header
+            protein_data = {key: [] for key in line_elements}
+            protein_data['ProteinGroup'] = []
+
+        if line.startswith('Unique'):  # Peptide Line Header
+            peptide_data = {key: [] for key in line_elements}
+            peptide_data['ProteinGroup'] = []
+
+            header_lines.append(line)
+            file_state = FileState.DATA
+            continue
+
+        if len(line_elements) > 1 and line_elements[1] == "Proteins":
+            file_state = FileState.INFO
+
+        if file_state == FileState.HEADER:
+            header_lines.append(line)
+
+        if file_state == FileState.DATA:
+            if line_elements[0] == '' or '*' in line_elements[0] or line_elements[0].isnumeric():
+
+                for key, value in zip(peptide_data, line_elements):
+                    peptide_data[key].append(value)
+                peptide_data['ProteinGroup'].append(current_protein_grp)
+
+                peptide_line_cnt += 1
+            else:
+                if peptide_line_cnt != 0:
+                    current_protein_grp += 1
+                    peptide_line_cnt = 0
+
+                for key, value in zip(protein_data, line_elements):
+                    protein_data[key].append(value)
+                protein_data['ProteinGroup'].append(current_protein_grp)
+
+        if file_state == FileState.INFO:
+            end_lines.append(line)
+
+    for k in peptide_data:
+        peptide_data[k] = _convert_to_best_datatype(peptide_data[k])
+
+    for k in protein_data:
+        protein_data[k] = _convert_to_best_datatype(protein_data[k])
+
+    peptide_df = pd.DataFrame(peptide_data)
+    protein_df = pd.DataFrame(protein_data)
+
+    file_name_components = [fn.split('.') for fn in peptide_df['FileName']]
+    peptide_df.drop(['FileName'], axis=1, inplace=True)
+
+    peptide_df['FileName'] = _convert_to_best_datatype([comp[0] for comp in file_name_components])
+    peptide_df['FileName'] = peptide_df['FileName'].astype('category')
+
+    peptide_df['LowScan'] = _convert_to_best_datatype([comp[1] for comp in file_name_components])
+    peptide_df['HighScan'] = _convert_to_best_datatype([comp[2] for comp in file_name_components])
+    peptide_df['Charge'] = _convert_to_best_datatype([comp[3] for comp in file_name_components])
+
+    peptide_df = peptide_df.convert_dtypes()
+    protein_df = protein_df.convert_dtypes()
+
+    if end_lines[-1] == '':
+        end_lines = end_lines[:-1]
+
+    return header_lines, peptide_df, protein_df, end_lines
+
+
+def to_dta_select_filter(header_lines: List[str], peptide_df: pd.DataFrame, protein_df: pd.DataFrame,
+                         end_lines: List[str]) -> StringIO:
+    """
+    Convert the given header lines, peptide and protein dataframes, and end lines into a StringIO object.
+
+    This function takes the header lines, peptide and protein dataframes, and end lines as inputs, and writes
+    them into a StringIO object in the DTASelect-filter.txt format.
+
+    Args:
+        header_lines (List[str]): A list of header lines.
+        peptide_df (pd.DataFrame): A dataframe containing peptide data.
+        protein_df (pd.DataFrame): A dataframe containing protein data.
+        end_lines (List[str]): A list of end lines (information lines).
+
+    Returns:
+        StringIO: A StringIO object containing the reformatted data in DTASelect-filter.txt format.
+    """
+
+    peptide_df = peptide_df.copy(deep=True)
+    protein_df = protein_df.copy(deep=True)
+
+    file_output = StringIO()
+
+    # Write header lines
+    _write_lines(file_output, header_lines)
+
+    # Write protein and peptide data
+    concatenated_file_names = peptide_df.apply(_create_file_name, axis=1)
+    peptide_df.drop(['FileName', 'LowScan', 'HighScan', 'Charge'], axis=1, inplace=True)
+    peptide_df['FileName'] = concatenated_file_names
+    # Re-order columns to make FileName the second column
+    peptide_df = _reorder_columns(peptide_df, 'FileName', 1)
+
+    protein_data_str = protein_df.drop(['ProteinGroup'], axis=1).to_csv(header=False, index=False, sep='\t')
+    peptide_data_str = peptide_df.drop(['ProteinGroup'], axis=1).to_csv(header=False, index=False, sep='\t')
+
+    protein_data_str = protein_data_str.replace('\r', '')
+    peptide_data_str = peptide_data_str.replace('\r', '')
+
+    current_protein_grp = 0
+    protein_lines = protein_data_str.split('\n')
+    peptide_lines = peptide_data_str.split('\n')
+
+    if protein_lines[-1] == '':
+        protein_lines = protein_lines[:-1]
+
+    if peptide_lines[-1] == '':
+        peptide_lines = peptide_lines[:-1]
+
+    protein_line_idx = 0
+    peptide_line_idx = 0
+
+    while protein_line_idx < len(protein_lines) and peptide_line_idx < len(peptide_lines):
+        if int(protein_df.iloc[protein_line_idx]['ProteinGroup']) == current_protein_grp:
+            file_output.write(protein_lines[protein_line_idx] + '\n')
+            protein_line_idx += 1
+        else:
+            file_output.write(peptide_lines[peptide_line_idx] + '\n')
+            peptide_line_idx += 1
+            if peptide_line_idx < len(peptide_lines) and int(
+                    peptide_df.iloc[peptide_line_idx - 1]['ProteinGroup']) != int(
+                peptide_df.iloc[peptide_line_idx]['ProteinGroup']):
+                current_protein_grp += 1
+
+    # Write remaining protein and peptide lines
+    _write_lines(file_output, protein_lines[protein_line_idx:])
+    _write_lines(file_output, peptide_lines[peptide_line_idx:])
+
+    _write_lines(file_output, end_lines)
+
+    return file_output
```

### Comparing `filterframes-0.1.2/src/filterframes.egg-info/PKG-INFO` & `filterframes-0.1.3/src/filterframes.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-Metadata-Version: 2.1
-Name: filterframes
-Version: 0.1.2
-Summary: A very simple DTASelect-Filter.txt parser.
-Author-email: Patrick Garrett <pgarrett@scripps.edu>
-License: MIT License
-        
-        Copyright (c) 2023 Patrick Garrett
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: repository, https://github.com/pgarrett-scripps/FilterFrames.git
-Keywords: IP2,PASER,Parser,Streamlit,DTASelect-filter,Peptide,Protein,Proteomics
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/python-package.yml/badge.svg)
-![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/pylint.yml/badge.svg)
-
-# filterframes
-
-filterframes is a Python package that provides an easy way to parse and manipulate DTASelect filter 
-files using pandas. The package allows you to read DTASelect-filter.txt files, create peptide and protein dataframes, 
-modify the dataframes, and write the modified dataframes back to a new DTASelect-filter.txt file. 
-
-### Note on dataframe columns:
-
-The column names in the peptide and protein dataframes will correspond to the header lines in the DTASelect-filter.txt
-files. In order to edit and output a valid DTASelect-filter file you must ensure that the
-peptide and protein dataframe column names and order are conserved, and that no additional columns are 
-included. Any changes in the columns order or names will be reflected  in the output DTASelect-filter.txt file.
-
-## Installation
-
-You can install filterframes using pip:
-
-```sh
-pip install filterframes
-```
-
-You can also install filterframes locally:
-
-```sh
-git clone https://github.com/pgarrett-scripps/FilterFrames.git
-cd filterframes
-pip install .
-```
-
-## Usage
-
-Here are some basic examples of how to use the package:
-
-### Example Python Script:
-```python
-from filterframes import from_dta_select_filter, to_dta_select_filter
-
-# Read DTASelect-filter.txt file and create peptide and protein dataframes
-file_input = r'tests/data/DTASelect-filter_V2_1_12_paser.txt'
-header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(file_input)
-
-# Display the first 5 rows of the peptide and protein dataframes
-print("Peptide DataFrame:")
-print(peptide_df.head())
-print("\nProtein DataFrame:")
-print(protein_df.head())
-
-# Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
-# ...
-
-# Write modified peptide and protein dataframes back to a DTASelect-filter.txt file
-file_output = r'tests/data/DTASelect-filter_V2_1_12_paser.out.txt'
-with open(file_output, 'w') as f:
-    output_string_io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
-    f.write(output_string_io.getvalue())
-
-print(f"\nModified DTASelect-filter.txt file saved to {file_output}")
-```
-
-### Example Streamlit App:
-
-```python
-# app.py
-from io import StringIO
-
-import streamlit as st
-from filterframes import from_dta_select_filter, to_dta_select_filter
-
-uploaded_filter_file = st.file_uploader("Choose a DTASelect-filter.txt file", type="txt")
-
-if uploaded_filter_file:
-    header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(StringIO(uploaded_filter_file.getvalue().decode('utf-8')))
-    
-    st.header('Peptide df')
-    st.dataframe(peptide_df)
-    st.header('Protein df')
-    st.dataframe(protein_df)
-
-    # Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
-    # ...
-
-    io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
-
-    st.download_button(label="Download Filter",
-                       data=io.getvalue(),
-                       file_name="DTASelect-filter.txt",
-                       mime="text/plain")
-```
-
-## Functions
-The main functions provided by the package are:
-
-
-```
-from_dta_select_filter(file_input: Union[str, TextIOWrapper, StringIO]) -> Tuple[List[str], pd.DataFrame, pd.DataFrame, List[str]]
-```
-
-Reads a DTASelect-filter.txt file and returns header lines, peptide dataframe, protein dataframe, and end lines.
-
-
-```
-to_dta_select_filter(header_lines: List[str], peptide_df: pd.DataFrame, protein_df: pd.DataFrame, end_lines: List[str]) -> StringIO
-```
-
-Writes the given header lines, peptide dataframe, protein dataframe, and end lines to a StringIO object in the DTASelect-filter.txt format.
-
+Metadata-Version: 2.1
+Name: filterframes
+Version: 0.1.3
+Summary: A very simple DTASelect-Filter.txt parser.
+Author-email: Patrick Garrett <pgarrett@scripps.edu>
+License: MIT License
+        
+        Copyright (c) 2023 Patrick Garrett
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/pgarrett-scripps/FilterFrames.git
+Keywords: IP2,PASER,Parser,Streamlit,DTASelect-filter,Peptide,Protein,Proteomics
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/python-package.yml/badge.svg)
+![example workflow](https://github.com/pgarrett-scripps/FilterFrames/actions/workflows/pylint.yml/badge.svg)
+
+# filterframes
+
+filterframes is a Python package that provides an easy way to parse and manipulate DTASelect filter 
+files using pandas. The package allows you to read DTASelect-filter.txt files, create peptide and protein dataframes, 
+modify the dataframes, and write the modified dataframes back to a new DTASelect-filter.txt file. 
+
+### Note on dataframe columns:
+
+The column names in the peptide and protein dataframes will correspond to the header lines in the DTASelect-filter.txt
+files. In order to edit and output a valid DTASelect-filter file you must ensure that the
+peptide and protein dataframe column names and order are conserved, and that no additional columns are 
+included. Any changes in the columns order or names will be reflected  in the output DTASelect-filter.txt file.
+
+## Installation
+
+You can install filterframes using pip:
+
+```sh
+pip install filterframes
+```
+
+You can also install filterframes locally:
+
+```sh
+git clone https://github.com/pgarrett-scripps/FilterFrames.git
+cd filterframes
+pip install .
+```
+
+## Usage
+
+Here are some basic examples of how to use the package:
+
+### Example Python Script:
+```python
+from filterframes import from_dta_select_filter, to_dta_select_filter
+
+# Read DTASelect-filter.txt file and create peptide and protein dataframes
+file_input = r'tests/data/DTASelect-filter_V2_1_12_paser.txt'
+header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(file_input)
+
+# Display the first 5 rows of the peptide and protein dataframes
+print("Peptide DataFrame:")
+print(peptide_df.head())
+print("\nProtein DataFrame:")
+print(protein_df.head())
+
+# Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
+# ...
+
+# Write modified peptide and protein dataframes back to a DTASelect-filter.txt file
+file_output = r'tests/data/DTASelect-filter_V2_1_12_paser.out.txt'
+with open(file_output, 'w') as f:
+    output_string_io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
+    f.write(output_string_io.getvalue())
+
+print(f"\nModified DTASelect-filter.txt file saved to {file_output}")
+```
+
+### Example Streamlit App:
+
+```python
+# app.py
+from io import StringIO
+
+import streamlit as st
+from filterframes import from_dta_select_filter, to_dta_select_filter
+
+uploaded_filter_file = st.file_uploader("Choose a DTASelect-filter.txt file", type="txt")
+
+if uploaded_filter_file:
+    header_lines, peptide_df, protein_df, end_lines = from_dta_select_filter(StringIO(uploaded_filter_file.getvalue().decode('utf-8')))
+    
+    st.header('Peptide df')
+    st.dataframe(peptide_df)
+    st.header('Protein df')
+    st.dataframe(protein_df)
+
+    # Modify peptide or protein dataframes as needed (e.g., filtering, normalization, etc.)
+    # ...
+
+    io = to_dta_select_filter(header_lines, peptide_df, protein_df, end_lines)
+
+    st.download_button(label="Download Filter",
+                       data=io.getvalue(),
+                       file_name="DTASelect-filter.txt",
+                       mime="text/plain")
+```
+
+## Functions
+The main functions provided by the package are:
+
+
+```
+from_dta_select_filter(file_input: Union[str, TextIOWrapper, StringIO]) -> Tuple[List[str], pd.DataFrame, pd.DataFrame, List[str]]
+```
+
+Reads a DTASelect-filter.txt file and returns header lines, peptide dataframe, protein dataframe, and end lines.
+
+
+```
+to_dta_select_filter(header_lines: List[str], peptide_df: pd.DataFrame, protein_df: pd.DataFrame, end_lines: List[str]) -> StringIO
+```
+
+Writes the given header lines, peptide dataframe, protein dataframe, and end lines to a StringIO object in the DTASelect-filter.txt format.
+
```

### Comparing `filterframes-0.1.2/tests/test_filterframes.py` & `filterframes-0.1.3/tests/test_filterframes.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from io import StringIO
-
-import pandas as pd
-
-from filterframes import from_dta_select_filter, to_dta_select_filter
-
-
-def test_from_dta_select_filter_to_df_V2_1_12_paser():
-    with open('tests/data/DTASelect-filter_V2_1_12_paser.txt', 'r') as file:
-        head_lines, peptide_df, protein_df, tail_lines = from_dta_select_filter(file)
-    assert len(protein_df) == 3
-
-    io = to_dta_select_filter(head_lines, peptide_df, protein_df, tail_lines)
-
-    assert isinstance(io, StringIO)
-    head_lines2, peptide_df2, protein_df2, tail_lines2 = from_dta_select_filter(io)
-    pd.testing.assert_frame_equal(peptide_df, peptide_df2)
-    assert head_lines == head_lines2
-    assert tail_lines == tail_lines2
-
-    str_value = io.getvalue()
-    assert isinstance(str_value, str)
-    head_lines3, peptide_df3, protein_df3, tail_lines3 = from_dta_select_filter(str_value)
-    pd.testing.assert_frame_equal(peptide_df, peptide_df3)
-    assert head_lines == head_lines3
-    assert tail_lines == tail_lines3
-
-
-def test_from_dta_select_filter_to_df_V2_1_13():
-    with open('tests/data/DTASelect-filter_V2_1_13.txt', 'r') as file:
-        head_lines, peptide_df, protein_df, tail_lines = from_dta_select_filter(file)
-    assert len(protein_df) == 8
-
-    io = to_dta_select_filter(head_lines, peptide_df, protein_df, tail_lines)
-
-    assert isinstance(io, StringIO)
-    head_lines2, peptide_df2, protein_df2, tail_lines2 = from_dta_select_filter(io)
-    pd.testing.assert_frame_equal(peptide_df, peptide_df2)
-    assert head_lines == head_lines2
-    assert tail_lines == tail_lines2
-
-    str_value = io.getvalue()
-    assert isinstance(str_value, str)
-    head_lines3, peptide_df3, protein_df3, tail_lines3 = from_dta_select_filter(str_value)
-    pd.testing.assert_frame_equal(peptide_df, peptide_df3)
-    assert head_lines == head_lines3
-    assert tail_lines == tail_lines3
+from io import StringIO
+
+import pandas as pd
+
+from filterframes import from_dta_select_filter, to_dta_select_filter
+
+
+def test_from_dta_select_filter_to_df_V2_1_12_paser():
+    with open('tests/data/DTASelect-filter_V2_1_12_paser.txt', 'r') as file:
+        head_lines, peptide_df, protein_df, tail_lines = from_dta_select_filter(file)
+    assert len(protein_df) == 3
+
+    io = to_dta_select_filter(head_lines, peptide_df, protein_df, tail_lines)
+
+    assert isinstance(io, StringIO)
+    head_lines2, peptide_df2, protein_df2, tail_lines2 = from_dta_select_filter(io)
+    pd.testing.assert_frame_equal(peptide_df, peptide_df2)
+    assert head_lines == head_lines2
+    assert tail_lines == tail_lines2
+
+    str_value = io.getvalue()
+    assert isinstance(str_value, str)
+    head_lines3, peptide_df3, protein_df3, tail_lines3 = from_dta_select_filter(str_value)
+    pd.testing.assert_frame_equal(peptide_df, peptide_df3)
+    assert head_lines == head_lines3
+    assert tail_lines == tail_lines3
+
+
+def test_from_dta_select_filter_to_df_V2_1_13():
+    with open('tests/data/DTASelect-filter_V2_1_13.txt', 'r') as file:
+        head_lines, peptide_df, protein_df, tail_lines = from_dta_select_filter(file)
+    assert len(protein_df) == 8
+
+    io = to_dta_select_filter(head_lines, peptide_df, protein_df, tail_lines)
+
+    assert isinstance(io, StringIO)
+    head_lines2, peptide_df2, protein_df2, tail_lines2 = from_dta_select_filter(io)
+    pd.testing.assert_frame_equal(peptide_df, peptide_df2)
+    assert head_lines == head_lines2
+    assert tail_lines == tail_lines2
+
+    str_value = io.getvalue()
+    assert isinstance(str_value, str)
+    head_lines3, peptide_df3, protein_df3, tail_lines3 = from_dta_select_filter(str_value)
+    pd.testing.assert_frame_equal(peptide_df, peptide_df3)
+    assert head_lines == head_lines3
+    assert tail_lines == tail_lines3
```

