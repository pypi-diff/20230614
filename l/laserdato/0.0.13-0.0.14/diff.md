# Comparing `tmp/laserdato-0.0.13.tar.gz` & `tmp/laserdato-0.0.14.tar.gz`

## Comparing `laserdato-0.0.13.tar` & `laserdato-0.0.14.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 laserdato-0.0.13/main.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/__init__.py
--rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/embed.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/get_model.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/laser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/lib/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/lib/constants.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 laserdato-0.0.13/laserdato/lib/text_processing.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.0.13/settings.json/settings.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.0.13/LICENSE
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 laserdato-0.0.13/README.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 laserdato-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 laserdato-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 laserdato-0.0.14/main.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/__init__.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/align.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/get_model.py
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/laser.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/embed.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/encoder.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/laserLstmEncoder.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/laserTransformerEncoder.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/embed/multiGpuEncoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/lib/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/lib/constants.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 laserdato-0.0.14/laserdato/lib/text_processing.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.0.14/settings.json/settings.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.0.14/LICENSE
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 laserdato-0.0.14/README.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 laserdato-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 laserdato-0.0.14/PKG-INFO
```

### Comparing `laserdato-0.0.13/laserdato/get_model.py` & `laserdato-0.0.14/laserdato/get_model.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.13/laserdato/lib/constants.py` & `laserdato-0.0.14/laserdato/lib/constants.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.13/laserdato/lib/text_processing.py` & `laserdato-0.0.14/laserdato/lib/text_processing.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,8 +29,9 @@
     sentences = [
         mosesPunctuationNormalizer(ftfy.fix_text(s).lower()) for s in sentences
     ]
     # line = translit(line, language_code=, reversed=True)
     sp = spm.SentencePieceProcessor(model_file=spm_model)
     # in 3.11 might need to do transformrf_sentences = [sp.EncodeAsPieces(sentence) for sentence in sentences]
     transformed_sentences = sp.EncodeAsPieces(sentences)
+
     return [" ".join([word for word in sentence]) for sentence in transformed_sentences]
```

### Comparing `laserdato-0.0.13/LICENSE` & `laserdato-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.13/README.md` & `laserdato-0.0.14/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 freeze_support()
                 ...
 
         The "freeze_support()" line can be omitted if the program
         is not going to be frozen to produce an executable.
 ```
 
-You might need to use this (strutucture)[https://pytorch.org/docs/stable/notes/windows.html#multiprocessing-error-without-if-clause-protection] to used embed_sentences with multiple GPUs 
+You might need to use this [strutucture](https://pytorch.org/docs/stable/notes/windows.html#multiprocessing-error-without-if-clause-protection) to used embed_sentences with multiple GPUs 
 
 ```
 def main()
     # do something here
 
 if __name__ == '__main__':
     main()
```

### Comparing `laserdato-0.0.13/pyproject.toml` & `laserdato-0.0.14/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "laserdato"
-version = "0.0.13"
+version = "0.0.14"
 authors = [
   { name="Lingua Custodia", email="" },
 ]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.7"
 dependencies = [
   "torch~=2.0.1",
   "sentencepiece",
   "numpy",
   "requests",
   "ftfy",
   "mosestokenizer",
   "fairseq",
+  "faiss-cpu",
 ]
 [project.urls]
```

### Comparing `laserdato-0.0.13/PKG-INFO` & `laserdato-0.0.14/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: laserdato
-Version: 0.0.13
+Version: 0.0.14
 Summary: A small example package
 Author: Lingua Custodia
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Requires-Dist: fairseq
+Requires-Dist: faiss-cpu
 Requires-Dist: ftfy
 Requires-Dist: mosestokenizer
 Requires-Dist: numpy
 Requires-Dist: requests
 Requires-Dist: sentencepiece
 Requires-Dist: torch~=2.0.1
 Description-Content-Type: text/markdown
@@ -40,15 +41,15 @@
                 freeze_support()
                 ...
 
         The "freeze_support()" line can be omitted if the program
         is not going to be frozen to produce an executable.
 ```
 
-You might need to use this (strutucture)[https://pytorch.org/docs/stable/notes/windows.html#multiprocessing-error-without-if-clause-protection] to used embed_sentences with multiple GPUs 
+You might need to use this [strutucture](https://pytorch.org/docs/stable/notes/windows.html#multiprocessing-error-without-if-clause-protection) to used embed_sentences with multiple GPUs 
 
 ```
 def main()
     # do something here
 
 if __name__ == '__main__':
     main()
```

