# Comparing `tmp/huspacy_nightly-0.9.0.dev237-py3-none-any.whl.zip` & `tmp/huspacy_nightly-0.9.0.dev239-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 92429 bytes, number of entries: 17
+Zip file size: 92430 bytes, number of entries: 17
 -rw-r--r--  2.0 unx     3973 b- defN 80-Jan-01 00:00 huspacy/__init__.py
 -rw-r--r--  2.0 unx      102 b- defN 80-Jan-01 00:00 huspacy/components/__init__.py
 -rw-r--r--  2.0 unx    17063 b- defN 80-Jan-01 00:00 huspacy/components/edit_tree_lemmatizer.py
 -rw-r--r--  2.0 unx     3237 b- defN 80-Jan-01 00:00 huspacy/components/lemma_postprocessing.py
 -rw-r--r--  2.0 unx     5077 b- defN 80-Jan-01 00:00 huspacy/components/lookup_lemmatizer.py
 -rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 huspacy/extra/__init__.py
 -rw-r--r--  2.0 unx     1635 b- defN 80-Jan-01 00:00 huspacy/extra/roman_num_converter.py
 -rw-r--r--  2.0 unx     2059 b- defN 80-Jan-01 00:00 huspacy/extra/sentencizer.py
 -rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 huspacy/integrations/__init__.py
 -rw-r--r--  2.0 unx     2413 b- defN 80-Jan-01 00:00 huspacy/integrations/nerpp.py
 -rw-r--r--  2.0 unx     4063 b- defN 80-Jan-01 00:00 huspacy/integrations/sentiment.py
 -rw-r--r--  2.0 unx   541963 b- defN 80-Jan-01 00:00 huspacy/resources/poltext_sentiment.json
 -rw-r--r--  2.0 unx   791334 b- defN 80-Jan-01 00:00 huspacy/resources/precognox_sentiment.json
 -rw-r--r--  2.0 unx     2103 b- defN 80-Jan-01 00:00 huspacy/utils.py
--rw-r--r--  2.0 unx    12064 b- defN 80-Jan-01 00:00 huspacy_nightly-0.9.0.dev237.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 huspacy_nightly-0.9.0.dev237.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1503 b- defN 16-Jan-01 00:00 huspacy_nightly-0.9.0.dev237.dist-info/RECORD
-17 files, 1388781 bytes uncompressed, 89937 bytes compressed:  93.5%
+-rw-r--r--  2.0 unx    12064 b- defN 80-Jan-01 00:00 huspacy_nightly-0.9.0.dev239.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 huspacy_nightly-0.9.0.dev239.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1503 b- defN 16-Jan-01 00:00 huspacy_nightly-0.9.0.dev239.dist-info/RECORD
+17 files, 1388781 bytes uncompressed, 89938 bytes compressed:  93.5%
```

## zipnote {}

```diff
@@ -36,17 +36,17 @@
 
 Filename: huspacy/resources/precognox_sentiment.json
 Comment: 
 
 Filename: huspacy/utils.py
 Comment: 
 
-Filename: huspacy_nightly-0.9.0.dev237.dist-info/METADATA
+Filename: huspacy_nightly-0.9.0.dev239.dist-info/METADATA
 Comment: 
 
-Filename: huspacy_nightly-0.9.0.dev237.dist-info/WHEEL
+Filename: huspacy_nightly-0.9.0.dev239.dist-info/WHEEL
 Comment: 
 
-Filename: huspacy_nightly-0.9.0.dev237.dist-info/RECORD
+Filename: huspacy_nightly-0.9.0.dev239.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `huspacy_nightly-0.9.0.dev237.dist-info/METADATA` & `huspacy_nightly-0.9.0.dev239.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huspacy-nightly
-Version: 0.9.0.dev237
+Version: 0.9.0.dev239
 Summary: HuSpaCy: industrial strength Hungarian natural language processing
 Home-page: https://github.com/huspacy/huspacy
 License: Apache-2.0
 Keywords: nlp,huspacy,Hungarian,text processing,text processing,language processing,text mining,tokenization,sentence boundary detection,sbd,sentence splitting,pos tagging,tagging,lemmatization,ner,named entity recognition,parsing,word embeddings,word vectors,spacy,spacy model
 Author: SzegedAI, MILAB
 Author-email: gyorgy@orosz.link
 Maintainer: György Orosz
```

## Comparing `huspacy_nightly-0.9.0.dev237.dist-info/RECORD` & `huspacy_nightly-0.9.0.dev239.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 huspacy/extra/sentencizer.py,sha256=8rDNILh3gwngMoq-srtrQLeLv8kke4BkS4L0MBSaw54,2059
 huspacy/integrations/__init__.py,sha256=7cBtB8nMP3CEm4izgf9JJVEhUq2G1fYtAXL5SuClZ40,44
 huspacy/integrations/nerpp.py,sha256=Wt9cKYMY1lpZ8WwAlWOuGMA--_JDuGxEFYQn9FBlwC4,2413
 huspacy/integrations/sentiment.py,sha256=g-squqWpGYJLqst3gH9_PhdkoQfvgw5GsiO_XFF0sLE,4063
 huspacy/resources/poltext_sentiment.json,sha256=pHx0iDx6Nl9zUuQKkdOB2hH3aXddMn-4wIZOUE9oS-Y,541963
 huspacy/resources/precognox_sentiment.json,sha256=STcuZYUMDFb5rgrcH9r39SsNl36mkG6gzqfsqIPE2TQ,791334
 huspacy/utils.py,sha256=b1-pq2FHw-nJSlFrwg-vTwGnMiWMypRXmyLEzrS90CI,2103
-huspacy_nightly-0.9.0.dev237.dist-info/METADATA,sha256=gSADEaqvuYCIOjlecd5kOtO2za08v5lktFRSyDOYupQ,12064
-huspacy_nightly-0.9.0.dev237.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-huspacy_nightly-0.9.0.dev237.dist-info/RECORD,,
+huspacy_nightly-0.9.0.dev239.dist-info/METADATA,sha256=WZ08V9VvNzqk-z6Svz7KC4X6JLVeUEPS6-zv655JT8Y,12064
+huspacy_nightly-0.9.0.dev239.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+huspacy_nightly-0.9.0.dev239.dist-info/RECORD,,
```

