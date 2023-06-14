# Comparing `tmp/texta-lexicon-matcher-1.0.3.tar.gz` & `tmp/texta-lexicon-matcher-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/texta-lexicon-matcher-1.0.3.tar", last modified: Thu Sep 10 12:49:22 2020, max compression
+gzip compressed data, was "dist/texta-lexicon-matcher-1.1.0.tar", last modified: Wed Sep 23 09:56:54 2020, max compression
```

## Comparing `texta-lexicon-matcher-1.0.3.tar` & `texta-lexicon-matcher-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)    35065 2020-08-19 10:22:47.000000 texta-lexicon-matcher-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      755 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      335 2020-09-09 07:46:05.000000 texta-lexicon-matcher-1.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2020-09-10 12:46:34.000000 texta-lexicon-matcher-1.0.3/VERSION
--rw-rw-rw-   0 root         (0) root         (0)       13 2020-08-19 10:22:47.000000 texta-lexicon-matcher-1.0.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      714 2020-08-19 10:22:47.000000 texta-lexicon-matcher-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/texta_lexicon_matcher/
--rw-rw-rw-   0 root         (0) root         (0)    10356 2020-09-10 12:46:34.000000 texta-lexicon-matcher-1.0.3/texta_lexicon_matcher/lexicon_matcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/texta_lexicon_matcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)      755 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/texta_lexicon_matcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      316 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/texta_lexicon_matcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/texta_lexicon_matcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/texta_lexicon_matcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2020-09-10 12:49:22.000000 texta-lexicon-matcher-1.0.3/texta_lexicon_matcher.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2020-08-19 10:22:47.000000 texta-lexicon-matcher-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      755 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      335 2020-09-09 07:46:05.000000 texta-lexicon-matcher-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2020-09-23 09:54:00.000000 texta-lexicon-matcher-1.1.0/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)       13 2020-08-19 10:22:47.000000 texta-lexicon-matcher-1.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      714 2020-08-19 10:22:47.000000 texta-lexicon-matcher-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/texta_lexicon_matcher/
+-rw-rw-rw-   0 root         (0) root         (0)    10349 2020-09-23 09:54:00.000000 texta-lexicon-matcher-1.1.0/texta_lexicon_matcher/lexicon_matcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/texta_lexicon_matcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      755 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/texta_lexicon_matcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      316 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/texta_lexicon_matcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/texta_lexicon_matcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/texta_lexicon_matcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2020-09-23 09:56:54.000000 texta-lexicon-matcher-1.1.0/texta_lexicon_matcher.egg-info/top_level.txt
```

### Comparing `texta-lexicon-matcher-1.0.3/LICENSE` & `texta-lexicon-matcher-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `texta-lexicon-matcher-1.0.3/PKG-INFO` & `texta-lexicon-matcher-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texta-lexicon-matcher
-Version: 1.0.3
+Version: 1.1.0
 Summary: texta-lexicon-matcher
 Home-page: https://git.texta.ee/texta/texta-lexicon-matcher-python
 Author: TEXTA
 Author-email: info@texta.ee
 License: GPLv3
 Description: # Texta Lexicon Matcher
```

### Comparing `texta-lexicon-matcher-1.0.3/setup.py` & `texta-lexicon-matcher-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `texta-lexicon-matcher-1.0.3/texta_lexicon_matcher/lexicon_matcher.py` & `texta-lexicon-matcher-1.1.0/texta_lexicon_matcher/lexicon_matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,20 +141,20 @@
                 words = phrase.split()
                 pattern = slop_pattern.join(words)
                 lex_with_slops.append(pattern)
         return lex_with_slops
 
     def _dispend_counter_matches(self, counter_matches: List[str], unpacked_match, text: str):
         match = unpacked_match[0]
-        match_start = match["spans"][0]
-        match_end = match["spans"][1]
+        match_start = match["span"][0]
+        match_end = match["span"][1]
 
         for counter_match in counter_matches:
-            counter_match_start = counter_match["spans"][0]
-            counter_match_end = counter_match["spans"][1]
+            counter_match_start = counter_match["span"][0]
+            counter_match_end = counter_match["span"][1]
 
             if self._counter_matches_preceeding and counter_match_end < match_start:
                 section = text[counter_match_end:match_start].strip()
                 if not self._ignore_punctuation:
                     if re.search(self._counter_ignore_pattern, section):
                         continue
 
@@ -207,17 +207,17 @@
         raw_end = match.end()
         raw_str_val = match.group()
 
         if re.search(r"^\s", raw_str_val):
             raw_start += 1
         if re.search(r"\s$", raw_str_val):
             raw_end -= 1
-        spans = [raw_start, raw_end]
+        span = [raw_start, raw_end]
         str_val = raw_str_val.strip()
-        unpacked_match = [{"str_val": str_val.lower(), "spans": spans}]
+        unpacked_match = [{"str_val": str_val.lower(), "span": span}]
         return unpacked_match
 
     def _get_counter_matches(self, text: str) -> List[Dict[str, Union[str, List[int]]]]:
         counter_matches = []
         for pattern in self._counter_patterns:
             if self._ignore_case:
                 matches = re.finditer(pattern, text, flags=re.IGNORECASE)
```

### Comparing `texta-lexicon-matcher-1.0.3/texta_lexicon_matcher.egg-info/PKG-INFO` & `texta-lexicon-matcher-1.1.0/texta_lexicon_matcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texta-lexicon-matcher
-Version: 1.0.3
+Version: 1.1.0
 Summary: texta-lexicon-matcher
 Home-page: https://git.texta.ee/texta/texta-lexicon-matcher-python
 Author: TEXTA
 Author-email: info@texta.ee
 License: GPLv3
 Description: # Texta Lexicon Matcher
```

