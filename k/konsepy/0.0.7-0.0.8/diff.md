# Comparing `tmp/konsepy-0.0.7.tar.gz` & `tmp/konsepy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konsepy-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "konsepy-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `konsepy-0.0.7.tar` & `konsepy-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      996 2023-06-13 19:40:44.640376 konsepy-0.0.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0       41 2023-06-13 19:40:44.640376 konsepy-0.0.7/.gitignore
--rw-r--r--   0        0        0      803 2023-06-13 19:40:44.640376 konsepy-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0      335 2023-06-13 19:40:44.640376 konsepy-0.0.7/README.md
--rw-r--r--   0        0        0      905 2023-06-13 19:40:44.640376 konsepy-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/__init__.py
--rw-r--r--   0        0        0     4116 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/bio_tag.py
--rw-r--r--   0        0        0     3056 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/cli.py
--rw-r--r--   0        0        0      104 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/constants.py
--rw-r--r--   0        0        0     4480 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/get_text_snippets.py
--rw-r--r--   0        0        0     1564 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/importer.py
--rw-r--r--   0        0        0     5284 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/regex.py
--rw-r--r--   0        0        0     2469 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/run_all.py
--rw-r--r--   0        0        0      654 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/rxutils.py
--rw-r--r--   0        0        0     5285 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/textio.py
--rw-r--r--   0        0        0      202 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/types.py
--rw-r--r--   0        0        0     1297 2023-06-13 19:40:44.640376 konsepy-0.0.7/test/build.ps1
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      996 2023-06-13 22:15:28.630545 konsepy-0.0.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0       41 2023-06-13 22:15:28.630545 konsepy-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1002 2023-06-13 22:15:28.630545 konsepy-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0      335 2023-06-13 22:15:28.630545 konsepy-0.0.8/README.md
+-rw-r--r--   0        0        0      905 2023-06-13 22:15:28.630545 konsepy-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/__init__.py
+-rw-r--r--   0        0        0     4149 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/bio_tag.py
+-rw-r--r--   0        0        0     3056 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/cli.py
+-rw-r--r--   0        0        0      104 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/constants.py
+-rw-r--r--   0        0        0     4480 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/get_text_snippets.py
+-rw-r--r--   0        0        0     1564 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/importer.py
+-rw-r--r--   0        0        0     5396 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/regex.py
+-rw-r--r--   0        0        0     2469 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/run_all.py
+-rw-r--r--   0        0        0      654 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/rxutils.py
+-rw-r--r--   0        0        0     5285 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/textio.py
+-rw-r--r--   0        0        0      202 2023-06-13 22:15:28.630545 konsepy-0.0.8/src/konsepy/types.py
+-rw-r--r--   0        0        0     1297 2023-06-13 22:15:28.630545 konsepy-0.0.8/test/build.ps1
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.8/PKG-INFO
```

### Comparing `konsepy-0.0.7/.github/workflows/publish-to-pypi.yml` & `konsepy-0.0.8/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.7/CHANGELOG.md` & `konsepy-0.0.8/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 * `Added`: for new features.
 * `Changed`: for changes in existing functionality.
 * `Deprecated`: for soon-to-be removed features.
 * `Removed`: for now removed features.
 * `Fixed`: for any bug fixes.
 * `Security`: in case of vulnerabilities.
 
+## [0.0.7] & [0.0.8] - 2023-06-13
+
+### Fixed
+
+* Fixed where `noteorder_label` didn't yet get correctly passed around
+* `enum.EnumType` is only available in 3.11+, so reverted to old `enum.EnumMeta`
+
 ## [0.0.6] - 2023-05-04
 
 ### Added
 
 * Added `noteorder_label` to allow notes to appear in a delined form (with multiple rows for a note)
 * Powershell script to test konsepy_nlp_template tutorial
```

### Comparing `konsepy-0.0.7/pyproject.toml` & `konsepy-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.7/src/konsepy/bio_tag.py` & `konsepy-0.0.8/src/konsepy/bio_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             fieldnames=['index', 'studyid', 'note_id', 'sentence_id', 'domain', 'category', 'capture', 'start', 'end']
         )
         writer.writeheader()
         i = 0
         for doc, (count, studyid, note_id, note_date) in nlp.pipe(format_for_spacy(
                 iterate_csv_file(
                     input_files, id_label=id_label, noteid_label=noteid_label, notedate_label=notedate_label,
-                    notetext_label=notetext_label,
+                    notetext_label=notetext_label, noteorder_label=noteorder_label,
                 )
         ), as_tuples=True):
             constant_meta = {
                 'studyid': studyid,
                 'note_id': note_id,
             }
             for sent_id, sentence in enumerate(doc.sents):
```

### Comparing `konsepy-0.0.7/src/konsepy/cli.py` & `konsepy-0.0.8/src/konsepy/cli.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.7/src/konsepy/get_text_snippets.py` & `konsepy-0.0.8/src/konsepy/get_text_snippets.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.7/src/konsepy/importer.py` & `konsepy-0.0.8/src/konsepy/importer.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.7/src/konsepy/regex.py` & `konsepy-0.0.8/src/konsepy/regex.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from loguru import logger
 
 
 def run_regex_on_files(input_files, regex_func, *, start_after=0, stop_after=None,
                        require_regex=None, window_size=50,
                        id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
                        notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-                       select_probability=1.0):
+                       noteorder_label=None, select_probability=1.0):
     count = 0  # default value; received from forloop below
     cat_counter_notes = Counter()
     cat_counter_mrns = defaultdict(set)
     noteid_to_cat = defaultdict(Counter)
     mrn_to_cat = defaultdict(Counter)
     unique_mrns = set()
     not_found_text = Counter()
     if require_regex:
         require_regex = re.compile(require_regex, re.I)
     for count, mrn, note_id, note_date, text in iterate_csv_file(
             input_files, start_after=start_after, stop_after=stop_after,
             id_label=id_label, noteid_label=noteid_label,
             notedate_label=notedate_label, notetext_label=notetext_label,
-            select_probability=select_probability
+            noteorder_label=noteorder_label, select_probability=select_probability,
     ):
         if count % 10000 == 0:
             logger.info(
                 f'Completed {count} records: {len(unique_mrns)} MRNs contain any category ({datetime.datetime.now()})')
         extract_categories(
             mrn, note_id, text, regex_func,
             cat_counter_mrns=cat_counter_mrns, cat_counter_notes=cat_counter_notes,
@@ -65,27 +65,27 @@
             not_found_text[' '.join(text.split())] += 1
 
 
 def run_regex_and_output(package_name, input_files, outdir, *concepts,
                          start_after=0, stop_after=None, require_regex=None, window_size=50,
                          id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
                          notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
-                         select_probability=1.0):
+                         noteorder_label=None, select_probability=1.0):
     dt = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
     for iconcept in get_all_concepts(package_name, *concepts):
         curr_outdir = outdir / f'{iconcept.name}_{dt}'
         curr_outdir.mkdir(parents=True)
         logger.add(curr_outdir / f'{iconcept.name}_{dt}.log')
         note_counter, cat_counter_mrns, not_found_text, mrn_to_cat, note_to_cat = run_regex_on_files(
             input_files, iconcept.run_func,
             start_after=start_after, stop_after=stop_after, require_regex=require_regex,
             window_size=window_size,
             id_label=id_label, noteid_label=noteid_label,
             notedate_label=notedate_label, notetext_label=notetext_label,
-            select_probability=select_probability
+            noteorder_label=noteorder_label, select_probability=select_probability,
         )
         output_results(curr_outdir, not_found_text=not_found_text, note_counter=note_counter,
                        cat_counter_mrns=cat_counter_mrns, category_enums=[iconcept.category_enum],
                        note_to_cat=note_to_cat, mrn_to_cat=mrn_to_cat)
 
 
 def search_first_regex(regexes):
```

### Comparing `konsepy-0.0.7/src/konsepy/run_all.py` & `konsepy-0.0.8/src/konsepy/run_all.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.7/src/konsepy/rxutils.py` & `konsepy-0.0.8/src/konsepy/rxutils.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.7/src/konsepy/textio.py` & `konsepy-0.0.8/src/konsepy/textio.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.7/test/build.ps1` & `konsepy-0.0.8/test/build.ps1`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.7/PKG-INFO` & `konsepy-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konsepy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Framework for build NLP information extraction systems using regular expressions.
 Keywords: nlp
 Author-email: dcronkite <dcronkite+pypi@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

