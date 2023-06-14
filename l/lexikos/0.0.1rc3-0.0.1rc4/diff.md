# Comparing `tmp/lexikos-0.0.1rc3.tar.gz` & `tmp/lexikos-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikos-0.0.1rc3.tar", last modified: Tue Jun  6 02:46:30 2023, max compression
+gzip compressed data, was "lexikos-0.0.1rc4.tar", last modified: Wed Jun 14 04:34:33 2023, max compression
```

## Comparing `lexikos-0.0.1rc3.tar` & `lexikos-0.0.1rc4.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.744902 lexikos-0.0.1rc3/
--rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc3/LICENSE
--rw-r--r--   0 mac        (502) staff       (20)       16 2023-04-21 13:04:42.000000 lexikos-0.0.1rc3/MANIFEST.in
--rw-r--r--   0 mac        (502) staff       (20)    29266 2023-06-06 02:46:30.745171 lexikos-0.0.1rc3/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)    15542 2023-06-05 11:09:13.000000 lexikos-0.0.1rc3/README.md
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.672441 lexikos-0.0.1rc3/lexikos/
--rw-r--r--   0 mac        (502) staff       (20)      105 2023-06-05 09:31:30.000000 lexikos-0.0.1rc3/lexikos/__init__.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.667372 lexikos-0.0.1rc3/lexikos/dict/
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.681853 lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/
--rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
--rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.694037 lexikos-0.0.1rc3/lexikos/dict/synthetic/
--rw-r--r--   0 mac        (502) staff       (20)      406 2023-05-19 10:04:44.000000 lexikos-0.0.1rc3/lexikos/dict/synthetic/austalk_en_au.tsv
--rw-r--r--   0 mac        (502) staff       (20)     2618 2023-05-19 10:05:54.000000 lexikos-0.0.1rc3/lexikos/dict/synthetic/sc_cw_en_au.tsv
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.743727 lexikos-0.0.1rc3/lexikos/dict/wikipron/
--rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_au_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_in_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_us_broad.tsv
--rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
--rw-r--r--   0 mac        (502) staff       (20)     5360 2023-06-06 02:44:11.000000 lexikos-0.0.1rc3/lexikos/g2p.py
--rw-r--r--   0 mac        (502) staff       (20)     2911 2023-05-09 09:56:54.000000 lexikos-0.0.1rc3/lexikos/lexicon.py
--rw-r--r--   0 mac        (502) staff       (20)     3360 2023-06-05 09:31:30.000000 lexikos-0.0.1rc3/lexikos/normalizer.py
--rw-r--r--   0 mac        (502) staff       (20)     1354 2023-06-06 02:44:11.000000 lexikos-0.0.1rc3/lexikos/t5.py
--rw-r--r--   0 mac        (502) staff       (20)      722 2023-06-06 02:44:11.000000 lexikos-0.0.1rc3/lexikos/utils.py
-drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-06 02:46:30.673702 lexikos-0.0.1rc3/lexikos.egg-info/
--rw-r--r--   0 mac        (502) staff       (20)    29266 2023-06-06 02:46:30.000000 lexikos-0.0.1rc3/lexikos.egg-info/PKG-INFO
--rw-r--r--   0 mac        (502) staff       (20)     1071 2023-06-06 02:46:30.000000 lexikos-0.0.1rc3/lexikos.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (502) staff       (20)        1 2023-06-06 02:46:30.000000 lexikos-0.0.1rc3/lexikos.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (502) staff       (20)        8 2023-06-06 02:46:30.000000 lexikos-0.0.1rc3/lexikos.egg-info/top_level.txt
--rw-r--r--   0 mac        (502) staff       (20)      821 2023-06-05 09:31:30.000000 lexikos-0.0.1rc3/pyproject.toml
--rw-r--r--   0 mac        (502) staff       (20)      113 2023-06-06 02:46:30.745820 lexikos-0.0.1rc3/setup.cfg
--rw-r--r--   0 mac        (502) staff       (20)      964 2023-04-21 13:31:07.000000 lexikos-0.0.1rc3/setup.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.625024 lexikos-0.0.1rc4/
+-rw-r--r--   0 mac        (502) staff       (20)    11357 2023-04-21 08:15:12.000000 lexikos-0.0.1rc4/LICENSE
+-rw-r--r--   0 mac        (502) staff       (20)       41 2023-06-14 04:34:25.000000 lexikos-0.0.1rc4/MANIFEST.in
+-rw-r--r--   0 mac        (502) staff       (20)    29266 2023-06-14 04:34:33.625297 lexikos-0.0.1rc4/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)    15542 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/README.md
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.591140 lexikos-0.0.1rc4/lexikos/
+-rw-r--r--   0 mac        (502) staff       (20)      105 2023-06-14 04:29:58.000000 lexikos-0.0.1rc4/lexikos/__init__.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.587243 lexikos-0.0.1rc4/lexikos/dict/
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.599592 lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/
+-rw-r--r--   0 mac        (502) staff       (20)  3752695 2023-04-21 10:31:03.000000 lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  5371871 2023-05-05 05:21:25.000000 lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.607560 lexikos-0.0.1rc4/lexikos/dict/synthetic/
+-rw-r--r--   0 mac        (502) staff       (20)      406 2023-05-19 10:04:44.000000 lexikos-0.0.1rc4/lexikos/dict/synthetic/austalk_en_au.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     2618 2023-05-19 10:05:54.000000 lexikos-0.0.1rc4/lexikos/dict/synthetic/sc_cw_en_au.tsv
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.624666 lexikos-0.0.1rc4/lexikos/dict/wikipron/
+-rw-r--r--   0 mac        (502) staff       (20)  1211254 2023-04-21 09:01:35.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1247086 2023-04-21 09:01:53.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_au_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    24475 2023-04-21 09:01:55.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_au_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1222027 2023-05-03 03:54:38.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_ca_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    25360 2023-05-03 03:54:42.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1198453 2023-05-03 03:54:46.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_in_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    22107 2023-05-03 03:54:51.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_in_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1204678 2023-05-03 03:54:56.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_nz_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    23973 2023-05-03 03:55:01.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1927167 2023-04-21 09:43:15.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_uk_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    36958 2023-04-21 09:43:03.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)  1841113 2023-04-21 09:43:18.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_us_broad.tsv
+-rw-r--r--   0 mac        (502) staff       (20)    47411 2023-04-21 09:43:20.000000 lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_us_narrow.tsv
+-rw-r--r--   0 mac        (502) staff       (20)     5360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/lexikos/g2p.py
+-rw-r--r--   0 mac        (502) staff       (20)     2747 2023-06-14 04:27:47.000000 lexikos-0.0.1rc4/lexikos/lexicon.py
+-rw-r--r--   0 mac        (502) staff       (20)     3360 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/lexikos/normalizer.py
+-rw-r--r--   0 mac        (502) staff       (20)     1354 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/lexikos/t5.py
+-rw-r--r--   0 mac        (502) staff       (20)      722 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/lexikos/utils.py
+drwxr-xr-x   0 mac        (502) staff       (20)        0 2023-06-14 04:34:33.593092 lexikos-0.0.1rc4/lexikos.egg-info/
+-rw-r--r--   0 mac        (502) staff       (20)    29266 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (502) staff       (20)     1118 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (502) staff       (20)        1 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (502) staff       (20)       33 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/requires.txt
+-rw-r--r--   0 mac        (502) staff       (20)        8 2023-06-14 04:34:33.000000 lexikos-0.0.1rc4/lexikos.egg-info/top_level.txt
+-rw-r--r--   0 mac        (502) staff       (20)      821 2023-06-14 04:30:01.000000 lexikos-0.0.1rc4/pyproject.toml
+-rw-r--r--   0 mac        (502) staff       (20)       32 2023-06-14 04:29:02.000000 lexikos-0.0.1rc4/requirements.txt
+-rw-r--r--   0 mac        (502) staff       (20)      113 2023-06-14 04:34:33.625814 lexikos-0.0.1rc4/setup.cfg
+-rw-r--r--   0 mac        (502) staff       (20)     1187 2023-06-14 04:32:35.000000 lexikos-0.0.1rc4/setup.py
```

### Comparing `lexikos-0.0.1rc3/LICENSE` & `lexikos-0.0.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/PKG-INFO` & `lexikos-0.0.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `lexikos-0.0.1rc3/README.md` & `lexikos-0.0.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv` & `lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv` & `lexikos-0.0.1rc4/lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/synthetic/sc_cw_en_au.tsv` & `lexikos-0.0.1rc4/lexikos/dict/synthetic/sc_cw_en_au.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_au_broad.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_au_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_au_narrow.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_au_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_ca_broad.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_ca_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_ca_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_in_broad.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_in_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_in_narrow.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_in_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_nz_broad.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_nz_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_nz_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_uk_broad.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_uk_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_uk_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_us_broad.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_us_broad.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/dict/wikipron/eng_latn_us_narrow.tsv` & `lexikos-0.0.1rc4/lexikos/dict/wikipron/eng_latn_us_narrow.tsv`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/g2p.py` & `lexikos-0.0.1rc4/lexikos/g2p.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/lexicon.py` & `lexikos-0.0.1rc4/lexikos/lexicon.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,20 +40,16 @@
         lex = {}
         with open(file, "r") as f:
             for line in f.readlines():
                 word, phonemes = line.strip().split("\t")
                 phonemes = phonemes.replace(" . ", " ")
                 if normalize_phonemes:
                     phonemes = self._normalize_phonemes(phonemes)
-                phonemes = [phonemes]
                 word = word.lower()
-                if word in lex:
-                    lex[word] = lex[word].union(phonemes)
-                else:
-                    lex[word] = set(phonemes)
+                lex[word] = lex.get(word, set()) | set([phonemes])
         return lex
 
     def _merge_dicts(self, dicts: List[Dict[Any, Set]]):
         output_dict = dicts[0]
         for d in dicts[1:]:
             for k, v in d.items():
                 if k in output_dict:
@@ -65,15 +61,15 @@
     def _normalize_phonemes(self, phonemes: str) -> str:
         """
         Modified from: [Michael McAuliffe](https://memcauliffe.com/speaker-dictionaries-and-multilingual-ipa.html#multilingual-ipa-mode)
         """
         diacritics = ["ː", "ˑ", "̆", "̯", "͡", "‿", "͜", "̩", "ˈ", "ˌ"]
         for d in diacritics:
             phonemes = phonemes.replace(d, "")
-        phonemes = " ".join([p for p in phonemes if p != " "]).strip()
+        phonemes = phonemes.strip()
         return phonemes
 
 
 if __name__ == "__main__":
     lexicon = Lexicon()
     print(lexicon["added"])
     print(lexicon["runner"])
```

### Comparing `lexikos-0.0.1rc3/lexikos/normalizer.py` & `lexikos-0.0.1rc4/lexikos/normalizer.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/t5.py` & `lexikos-0.0.1rc4/lexikos/t5.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos/utils.py` & `lexikos-0.0.1rc4/lexikos/utils.py`

 * *Files identical despite different names*

### Comparing `lexikos-0.0.1rc3/lexikos.egg-info/PKG-INFO` & `lexikos-0.0.1rc4/lexikos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikos
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.
 Home-page: https://github.com/bookbot-hive/lexikos
 Author: w11wo
 Author-email: w11wo <wilson@bookbotkids.com>, anantoj <gg.ananto@gmail.com>, DavidSamuell <davidsamuel.7878@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `lexikos-0.0.1rc3/lexikos.egg-info/SOURCES.txt` & `lexikos-0.0.1rc4/lexikos.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
 lexikos/__init__.py
 lexikos/g2p.py
 lexikos/lexicon.py
 lexikos/normalizer.py
 lexikos/t5.py
 lexikos/utils.py
 lexikos.egg-info/PKG-INFO
 lexikos.egg-info/SOURCES.txt
 lexikos.egg-info/dependency_links.txt
+lexikos.egg-info/requires.txt
 lexikos.egg-info/top_level.txt
 lexikos/dict/cmudict-ipa/cmudict-0.7b-ipa-segmented.tsv
 lexikos/dict/cmudict-ipa/librispeech-lexicon-200k-allothers-g2p-ipa.tsv
 lexikos/dict/synthetic/austalk_en_au.tsv
 lexikos/dict/synthetic/sc_cw_en_au.tsv
 lexikos/dict/wikipron/eng_latn.tsv
 lexikos/dict/wikipron/eng_latn_au_broad.tsv
```

### Comparing `lexikos-0.0.1rc3/pyproject.toml` & `lexikos-0.0.1rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexikos"
-version = "0.0.1rc3"
+version = "0.0.1rc4"
 description = "A collection of pronunciation dictionaries and neural grapheme-to-phoneme models."
 readme = "README.md"
 authors = [{ name="w11wo", email="wilson@bookbotkids.com" }, { name="anantoj", email="gg.ananto@gmail.com" }, { name="DavidSamuell", email="davidsamuel.7878@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `lexikos-0.0.1rc3/setup.py` & `lexikos-0.0.1rc4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 this_path = Path(__file__).parent
 module_dir = this_path / "lexikos"
 
 readme_path = this_path / "README.md"
+requirements_path = this_path / "requirements.txt"
+
 long_description = readme_path.read_text(encoding="utf-8")
 
 data_dir = module_dir / "dict"
 data_files = [
     str(f.relative_to(module_dir)) for f in data_dir.rglob("*.tsv") if f.is_file()
 ]
 
+with open(requirements_path, "r", encoding="utf-8") as requirements_file:
+    requirements = requirements_file.read().splitlines()
+
 if __name__ == "__main__":
     setup(
         name="lexikos",
         description="A collection of pronunciation dictionaries and neural grapheme-to-phoneme models.",
         long_description=long_description,
         long_description_content_type="text/markdown",
         author="w11wo",
         author_email="wilson@bookbotkids.com",
         url="https://github.com/bookbot-hive/lexikos",
         license="Apache License",
         packages=find_packages(),
+        install_requires=requirements,
         package_data={"lexikos": data_files},
         include_package_data=True,
         platforms=["linux", "unix", "windows"],
     )
```

