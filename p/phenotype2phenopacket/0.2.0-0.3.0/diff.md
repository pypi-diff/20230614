# Comparing `tmp/phenotype2phenopacket-0.2.0.tar.gz` & `tmp/phenotype2phenopacket-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenotype2phenopacket-0.2.0.tar", max compression
+gzip compressed data, was "phenotype2phenopacket-0.3.0.tar", max compression
```

## Comparing `phenotype2phenopacket-0.2.0.tar` & `phenotype2phenopacket-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1320 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/README.md
--rw-r--r--   0        0        0      913 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/add/__init__.py
--rw-r--r--   0        0        0     2361 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/add/add_genes.py
--rw-r--r--   0        0        0      478 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli.py
--rw-r--r--   0        0        0     1092 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_add.py
--rw-r--r--   0        0        0     1085 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_convert.py
--rw-r--r--   0        0        0     1087 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_create.py
--rw-r--r--   0        0        0        0 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/convert/__init__.py
--rw-r--r--   0        0        0     1123 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/convert/convert.py
--rw-r--r--   0        0        0        0 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/create/__init__.py
--rw-r--r--   0        0        0     1897 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/create/create.py
--rw-r--r--   0        0        0 16425815 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt
--rw-r--r--   0        0        0        0 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/__init__.py
--rw-r--r--   0        0        0     2405 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/gene_map_utils.py
--rw-r--r--   0        0        0    22255 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/phenopacket_utils.py
--rw-r--r--   0        0        0     1925 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/utils.py
--rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 phenotype2phenopacket-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1320 2023-06-14 17:37:44.450551 phenotype2phenopacket-0.3.0/README.md
+-rw-r--r--   0        0        0      913 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/add/__init__.py
+-rw-r--r--   0        0        0     2361 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/add/add_genes.py
+-rw-r--r--   0        0        0      478 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/cli.py
+-rw-r--r--   0        0        0     1092 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/cli_add.py
+-rw-r--r--   0        0        0     1085 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/cli_convert.py
+-rw-r--r--   0        0        0     1087 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/cli_create.py
+-rw-r--r--   0        0        0        0 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/convert/__init__.py
+-rw-r--r--   0        0        0     1123 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/convert/convert.py
+-rw-r--r--   0        0        0        0 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/create/__init__.py
+-rw-r--r--   0        0        0     1897 2023-06-14 17:37:44.454551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/create/create.py
+-rw-r--r--   0        0        0 16425815 2023-06-14 17:37:44.542551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt
+-rw-r--r--   0        0        0        0 2023-06-14 17:37:44.542551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/utils/__init__.py
+-rw-r--r--   0        0        0     2405 2023-06-14 17:37:44.546551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/utils/gene_map_utils.py
+-rw-r--r--   0        0        0    23353 2023-06-14 17:37:44.546551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/utils/phenopacket_utils.py
+-rw-r--r--   0        0        0     1925 2023-06-14 17:37:44.546551 phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/utils/utils.py
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 phenotype2phenopacket-0.3.0/PKG-INFO
```

### Comparing `phenotype2phenopacket-0.2.0/README.md` & `phenotype2phenopacket-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/pyproject.toml` & `phenotype2phenopacket-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phenotype2phenopacket"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>"]
 readme = "README.md"
 packages = [{ include = "phenotype2phenopacket", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/add/add_genes.py` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/add/add_genes.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_add.py` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/cli_add.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_convert.py` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/cli_convert.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_create.py` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/cli_create.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/convert/convert.py` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/convert/convert.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/create/create.py` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/create/create.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/gene_map_utils.py` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/utils/gene_map_utils.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/phenopacket_utils.py` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/utils/phenopacket_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import re
 import secrets
+import signal
 from copy import copy
 from dataclasses import dataclass
 from fractions import Fraction
 from pathlib import Path
 from typing import Union
 
 import polars as pl
@@ -40,47 +41,52 @@
 frequency_hpo = {
     "HP:0040281": FrequencyTerm(0, 0),
     "HP:0040282": FrequencyTerm(1, 4),
     "HP:0040283": FrequencyTerm(5, 29),
     "HP:0040284": FrequencyTerm(30, 79),
     "HP:0040285": FrequencyTerm(80, 99),
     "HP:0040286": FrequencyTerm(100, 100),
+    "HP:0040280": FrequencyTerm(100, 100),
 }
 
 
 @dataclass
 class OnsetTerm:
     lower_age: Union[int, str]
     upper_age: Union[int, str]
 
 
 onset_hpo = {
     "HP:0011462": OnsetTerm(16, 40),
-    "HP:0011460": OnsetTerm(0, 0.019230769230769232),
+    "HP:0011460": OnsetTerm(0, 0),
     "HP:0011463": OnsetTerm(1, 5),
     "HP:0003584": OnsetTerm(60, 90),
     "HP:0025709": OnsetTerm(19, 25),
-    "HP:0034198": OnsetTerm(0, 0.019230769230769232),
+    "HP:0034198": OnsetTerm(0, 0),
     "HP:0003596": OnsetTerm(40, 60),
     "HP:0003621": OnsetTerm(5, 15),
     "HP:0003593": OnsetTerm(0, 1),
     "HP:4000040": OnsetTerm(0, 0),
-    "HP:0011461": OnsetTerm(0, 0.019230769230769232),
+    "HP:0011461": OnsetTerm(0, 0),
     "HP:0003577": OnsetTerm(0, 0),
-    "HP:0034197": OnsetTerm(0, 0.019230769230769232),
+    "HP:0034197": OnsetTerm(0, 0),
     "HP:0025708": OnsetTerm(16, 19),
     "HP:0410280": OnsetTerm(1, 15),
-    "HP:0030674": OnsetTerm(0, 0.019230769230769232),
-    "HP:0003623": OnsetTerm(0, 0.019230769230769232),
-    "HP:0034199": OnsetTerm(0, 0.019230769230769232),
+    "HP:0030674": OnsetTerm(0, 0),
+    "HP:0003623": OnsetTerm(0, 0),
+    "HP:0034199": OnsetTerm(0, 0),
     "HP:0003581": OnsetTerm(16, 80),
     "HP:0025710": OnsetTerm(25, 40),
 }
 
 
+def handler(signum, frame):
+    raise TimeoutError("Took too long to filter terms.")
+
+
 @dataclass
 class PhenopacketFile:
     phenopacket: Phenopacket
     phenopacket_path: Path
 
 
 def phenopacket_reader(file: Path):
@@ -100,20 +106,26 @@
 
 
 def create_json_message(phenopacket: Phenopacket) -> str:
     """Create json message for writing to file."""
     return MessageToJson(phenopacket)
 
 
-def write_phenopacket(phenopacket: Phenopacket, output_file: Path) -> None:
+def write_phenopacket(phenopacket: Phenopacket, output_file: Path) -> Path:
     """Write a phenopacket."""
     phenopacket_json = create_json_message(phenopacket)
-    with open(output_file, "w") as outfile:
-        outfile.write(phenopacket_json)
-    outfile.close()
+    suffix = 1
+    while Path(
+        output_file.parents[0].joinpath(f"{output_file.stem}_patient_{suffix}.json")
+    ).is_file():
+        suffix += 1
+    output_file = output_file.parents[0].joinpath(f"{output_file.stem}_patient_{suffix}.json")
+    with open(output_file, "w") as file:
+        file.write(phenopacket_json)
+    file.close()
 
 
 class SyntheticPatientGenerator:
     def __init__(self, disease_df: pl.DataFrame, ontology, ontology_factory):
         self.disease_df = disease_df
         self.ontology = ontology
         self.ontology_factory = ontology_factory
@@ -122,15 +134,18 @@
         self.filtered_df = []
         self.secret_rand = secrets.SystemRandom()
 
     def get_number_of_terms(self):
         """Get number of terms to ascribe from full set."""
         if len(self.disease_df) == 1:
             return 1
-        return int(len(self.disease_df) * (self.secret_rand.uniform(0.2, 0.75)))
+        number_of_terms = 0
+        while number_of_terms == 0:
+            number_of_terms = int(len(self.disease_df) * (self.secret_rand.uniform(0.2, 0.75)))
+        return number_of_terms
 
     @staticmethod
     def shuffle_dataframe(disease_df: pl.DataFrame):
         """Shuffle dataframe."""
         return disease_df.sample(fraction=1, shuffle=True)
 
     def add_frequency(self):
@@ -154,20 +169,27 @@
                 if self.upper_age < float(onset_hpo[phenotype_entry["onset"]].upper_age):
                     self.upper_age = float(onset_hpo[phenotype_entry["onset"]].upper_age)
         return OnsetTerm(lower_age=self.lower_age, upper_age=self.upper_age)
 
     def check_hpo_frequency(self, phenotype_entry: dict):
         """Filter with HPO defined frequencies."""
         frequency_limits = frequency_hpo[phenotype_entry["frequency"]]
-        random_frequency = self.secret_rand.uniform(0, 100)
         if (
-            float(frequency_limits.lower) < random_frequency < float(frequency_limits.upper)
+            frequency_limits.lower == 100
+            and frequency_limits.upper == 100
             and phenotype_entry not in self.filtered_df
         ):
             self.filtered_df.append(phenotype_entry)
+        else:
+            random_frequency = self.secret_rand.uniform(0, 100)
+            if (
+                float(frequency_limits.lower) < random_frequency < float(frequency_limits.upper)
+                and phenotype_entry not in self.filtered_df
+            ):
+                self.filtered_df.append(phenotype_entry)
 
     def check_frequency_threshold(
         self, frequency: float, phenotype_entry: dict, random_frequency: float
     ):
         """Check if patient frequency meets the filter for the disease frequency."""
         if random_frequency <= float(frequency) and phenotype_entry not in self.filtered_df:
             self.filtered_df.append(phenotype_entry)
@@ -201,20 +223,31 @@
         elif "/" in str(phenotype_entry["frequency"]):
             self.check_fraction_frequency(phenotype_entry)
         elif is_float(phenotype_entry["frequency"]) is True:
             self.check_float_frequency(phenotype_entry)
 
     def filter_phenotype_entries(self, frequency_df: pl.DataFrame, max_number: int):
         """Filter annotations based on frequency."""
-        while len(self.filtered_df) < max_number:
-            for phenotype_entry in frequency_df.rows(named=True):
-                if len(self.filtered_df) >= max_number:
-                    break
-                self.check_frequency(phenotype_entry)
-        return pl.from_dicts(self.filtered_df)
+        time_limit = 15
+        signal.signal(signal.SIGALRM, handler)
+        signal.alarm(time_limit)
+        try:
+            while len(self.filtered_df) < max_number:
+                for phenotype_entry in frequency_df.rows(named=True):
+                    if len(self.filtered_df) >= max_number:
+                        break
+                    self.check_frequency(phenotype_entry)
+            return pl.from_dicts(self.filtered_df)
+        except TimeoutError:
+            if len(self.filtered_df) == 0:
+                return frequency_df.sample(n=max_number)
+            else:
+                return pl.from_dicts(self.filtered_df)
+        finally:
+            signal.alarm(0)
 
     def get_patient_terms(self):
         """Get patient terms, filtered on frequency thresholds."""
         return self.filter_phenotype_entries(
             self.shuffle_dataframe(self.add_frequency()), self.get_number_of_terms()
         )
 
@@ -254,15 +287,19 @@
         if term.startswith("Abnormality of"):
             return phenotype_entry
         for _i in range(steps):
             parents = self.ontology.hierarchical_parents(term_id)
             parent = self.secret_rand.choice(parents)
             rels = self.ontology.entity_alias_map(parent)
             term = "".join(rels[(list(rels.keys())[0])])
-            if term.startswith("Abnormality of") or term_id == "HP:0000118":
+            if (
+                term.startswith("Abnormality of")
+                or term_id == "HP:0000118"
+                or term_id == "HP:0032443"
+            ):
                 break
             else:
                 term_id = parent
         phenotype_entry["hpo_id"] = term_id
         return phenotype_entry
 
     @staticmethod
```

### Comparing `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/utils.py` & `phenotype2phenopacket-0.3.0/src/phenotype2phenopacket/utils/utils.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.2.0/PKG-INFO` & `phenotype2phenopacket-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenotype2phenopacket
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

