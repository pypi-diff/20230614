# Comparing `tmp/seedot-2.1.tar.gz` & `tmp/seedot-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedot-2.1.tar", last modified: Sat Jun 10 15:22:37 2023, max compression
+gzip compressed data, was "seedot-3.0.tar", last modified: Wed Jun 14 07:55:25 2023, max compression
```

## Comparing `seedot-2.1.tar` & `seedot-3.0.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 15:22:37.204462 seedot-2.1/
--rw-rw-r--   0 Vittom     (505) staff       (20)     1046 2022-05-25 14:57:47.000000 seedot-2.1/LICENSE.txt
--rw-r--r--   0 Vittom     (505) staff       (20)       60 2023-06-09 17:22:08.000000 seedot-2.1/MANIFEST.in
--rw-r--r--   0 Vittom     (505) staff       (20)     6057 2023-06-10 15:22:37.204611 seedot-2.1/PKG-INFO
--rw-r--r--   0 Vittom     (505) staff       (20)     5020 2023-06-10 15:19:12.000000 seedot-2.1/README.md
--rw-rw-rw-   0 Vittom     (505) staff       (20)        0 2022-05-25 14:52:50.000000 seedot-2.1/__init__.py
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 15:22:37.201096 seedot-2.1/seedot/
--rw-r--r--   0 Vittom     (505) staff       (20)   111054 2023-06-09 14:07:59.000000 seedot-2.1/seedot/SEEDOT_lexicon_electronic.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   122566 2023-06-09 14:08:17.000000 seedot-2.1/seedot/SEEDOT_lexicon_finance.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   107729 2023-06-09 14:07:23.000000 seedot-2.1/seedot/SEEDOT_lexicon_food.txt
--rw-r--r--   0 Vittom     (505) staff       (20)   112307 2023-06-09 14:08:30.000000 seedot-2.1/seedot/SEEDOT_lexicon_hotel.txt
--rw-rw-rw-   0 Vittom     (505) staff       (20)       17 2023-06-09 15:09:32.000000 seedot-2.1/seedot/__init__.py
--rw-rw-r--   0 Vittom     (505) staff       (20)   121986 2022-05-25 15:33:30.000000 seedot-2.1/seedot/emoji_utf8_lexicon.txt
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34337 2023-06-10 14:02:50.000000 seedot-2.1/seedot/seedot_electronic.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    33893 2023-06-10 14:02:13.000000 seedot-2.1/seedot/seedot_finance.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34308 2023-06-10 14:02:32.000000 seedot-2.1/seedot/seedot_food.py
--rw-rw-rw-   0 Vittom     (505) staff       (20)    34313 2023-06-10 14:03:23.000000 seedot-2.1/seedot/seedot_hotel.py
-drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-10 15:22:37.204113 seedot-2.1/seedot.egg-info/
--rw-r--r--   0 Vittom     (505) staff       (20)     6057 2023-06-10 15:22:37.000000 seedot-2.1/seedot.egg-info/PKG-INFO
--rw-r--r--   0 Vittom     (505) staff       (20)      494 2023-06-10 15:22:37.000000 seedot-2.1/seedot.egg-info/SOURCES.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        1 2023-06-10 15:22:37.000000 seedot-2.1/seedot.egg-info/dependency_links.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        9 2023-06-10 15:22:37.000000 seedot-2.1/seedot.egg-info/requires.txt
--rw-r--r--   0 Vittom     (505) staff       (20)        7 2023-06-10 15:22:37.000000 seedot-2.1/seedot.egg-info/top_level.txt
--rw-rw-r--   0 Vittom     (505) staff       (20)     1359 2023-06-10 15:22:37.205292 seedot-2.1/setup.cfg
--rw-rw-rw-   0 Vittom     (505) staff       (20)     1848 2023-06-10 15:22:12.000000 seedot-2.1/setup.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-14 07:55:25.094792 seedot-3.0/
+-rw-rw-r--   0 Vittom     (505) staff       (20)     1046 2022-05-25 14:57:47.000000 seedot-3.0/LICENSE.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)       60 2023-06-09 17:22:08.000000 seedot-3.0/MANIFEST.in
+-rw-r--r--   0 Vittom     (505) staff       (20)    11405 2023-06-14 07:55:25.095331 seedot-3.0/PKG-INFO
+-rw-r--r--   0 Vittom     (505) staff       (20)    10369 2023-06-13 23:02:22.000000 seedot-3.0/README.md
+-rw-rw-rw-   0 Vittom     (505) staff       (20)        0 2022-05-25 14:52:50.000000 seedot-3.0/__init__.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-14 07:55:25.090066 seedot-3.0/seedot/
+-rw-r--r--   0 Vittom     (505) staff       (20)   111054 2023-06-09 14:07:59.000000 seedot-3.0/seedot/SEEDOT_lexicon_electronic.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   122566 2023-06-09 14:08:17.000000 seedot-3.0/seedot/SEEDOT_lexicon_finance.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   107729 2023-06-09 14:07:23.000000 seedot-3.0/seedot/SEEDOT_lexicon_food.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)   112307 2023-06-09 14:08:30.000000 seedot-3.0/seedot/SEEDOT_lexicon_hotel.txt
+-rw-rw-rw-   0 Vittom     (505) staff       (20)       17 2023-06-09 15:09:32.000000 seedot-3.0/seedot/__init__.py
+-rw-rw-r--   0 Vittom     (505) staff       (20)   121986 2022-05-25 15:33:30.000000 seedot-3.0/seedot/emoji_utf8_lexicon.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)    17359 2023-06-13 20:21:13.000000 seedot-3.0/seedot/seedot_procedure.py
+-rw-rw-rw-   0 Vittom     (505) staff       (20)    35047 2023-06-13 20:44:47.000000 seedot-3.0/seedot/sentiment_analyzer.py
+drwxr-xr-x   0 Vittom     (505) staff       (20)        0 2023-06-14 07:55:25.093954 seedot-3.0/seedot.egg-info/
+-rw-r--r--   0 Vittom     (505) staff       (20)    11405 2023-06-14 07:55:25.000000 seedot-3.0/seedot.egg-info/PKG-INFO
+-rw-r--r--   0 Vittom     (505) staff       (20)      452 2023-06-14 07:55:25.000000 seedot-3.0/seedot.egg-info/SOURCES.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        1 2023-06-14 07:55:25.000000 seedot-3.0/seedot.egg-info/dependency_links.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        9 2023-06-14 07:55:25.000000 seedot-3.0/seedot.egg-info/requires.txt
+-rw-r--r--   0 Vittom     (505) staff       (20)        7 2023-06-14 07:55:25.000000 seedot-3.0/seedot.egg-info/top_level.txt
+-rw-rw-r--   0 Vittom     (505) staff       (20)     1371 2023-06-14 07:55:25.096950 seedot-3.0/setup.cfg
+-rw-rw-rw-   0 Vittom     (505) staff       (20)     1848 2023-06-14 07:51:56.000000 seedot-3.0/setup.py
```

### Comparing `seedot-2.1/LICENSE.txt` & `seedot-3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seedot-2.1/seedot/SEEDOT_lexicon_electronic.txt` & `seedot-3.0/seedot/SEEDOT_lexicon_electronic.txt`

 * *Files identical despite different names*

### Comparing `seedot-2.1/seedot/SEEDOT_lexicon_finance.txt` & `seedot-3.0/seedot/SEEDOT_lexicon_finance.txt`

 * *Files identical despite different names*

### Comparing `seedot-2.1/seedot/SEEDOT_lexicon_food.txt` & `seedot-3.0/seedot/SEEDOT_lexicon_food.txt`

 * *Files identical despite different names*

### Comparing `seedot-2.1/seedot/SEEDOT_lexicon_hotel.txt` & `seedot-3.0/seedot/SEEDOT_lexicon_hotel.txt`

 * *Files identical despite different names*

### Comparing `seedot-2.1/seedot/emoji_utf8_lexicon.txt` & `seedot-3.0/seedot/emoji_utf8_lexicon.txt`

 * *Files identical despite different names*

### Comparing `seedot-2.1/seedot/seedot_electronic.py` & `seedot-3.0/seedot/sentiment_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             if valence > 0:
                 scalar += C_INCR
             else:
                 scalar -= C_INCR
     return scalar
 
 
-class electronic_ST(object):
+class ST(object):
     """
     Identify sentiment-relevant string-level properties of input text.
     """
 
     def __init__(self, text):
         if not isinstance(text, str):
             text = str(text).encode('utf-8')
@@ -175,25 +175,47 @@
         Leaves contractions and most emoticons
             Does not preserve punc-plus-letter emoticons (e.g. :D)
         """
         wes = self.text.split()
         stripped = list(map(self._strip_punc_if_word, wes))
         return stripped
 
-class electronic_SIA(object):
+lexicon_files = ["food", "finance", "electronic", "hotel"]
+
+class SIA(object):
     """
-    Give a sentiment intensity score to sentences.
+    Give a sentiment intensity score to sentences. 
     """
 
-    def __init__(self, lexicon_file="SEEDOT_lexicon_electronic.txt", emoji_lexicon="emoji_utf8_lexicon.txt"):
+    def __init__(self, domain= None, emoji_lexicon="emoji_utf8_lexicon.txt"):
+        if domain == "food":
+            lex = "SEEDOT_lexicon_food.txt"
+            d = {}
+        elif domain == "finance":
+            lex = "SEEDOT_lexicon_finance.txt"
+            d = {}
+        elif domain == "electronic":
+            lex = "SEEDOT_lexicon_electronic.txt"
+            d = {}
+        elif domain == "hotel":
+            lex = "SEEDOT_lexicon_hotel.txt"
+            d = {} 
+        elif isinstance(domain, dict):
+            lex = ""
+        else: 
+            raise ValueError("A valid domain ('electronic', 'finance', 'food', 'hotel') or a seedot_dictionary must be specified.")
+
         _this_module_file_path_ = os.path.abspath(getsourcefile(lambda: 0))
-        lexicon_full_filepath = os.path.join(os.path.dirname(_this_module_file_path_), lexicon_file)
-        with codecs.open(lexicon_full_filepath, encoding='utf-8') as f:
-            self.lexicon_full_filepath = f.read()
-        self.lexicon = self.make_lex_dict()
+        lexicon_full_filepath = os.path.join(os.path.dirname(_this_module_file_path_), lex)
+        if domain in lexicon_files:             
+            with codecs.open(lexicon_full_filepath, encoding='utf-8') as f:
+                self.lexicon_full_filepath = f.read()
+            self.lexicon = self.make_lex_dict()
+        else:
+            self.lexicon = domain
 
         emoji_full_filepath = os.path.join(os.path.dirname(_this_module_file_path_), emoji_lexicon)
         with codecs.open(emoji_full_filepath, encoding='utf-8') as f:
             self.emoji_full_filepath = f.read()
         self.emojis = self.make_emoji_dict()
 
     def make_lex_dict(self):
@@ -236,15 +258,15 @@
                 text_no_emoji += description
                 prev_space = False
             else:
                 text_no_emoji += chr
                 prev_space = chr == ' '
         text = text_no_emoji.strip()
 
-        sentitext = electronic_ST(text)
+        sentitext = ST(text)
 
         sentiments = []
         words_and_emoticons = sentitext.words_and_emoticons
         for i, item in enumerate(words_and_emoticons):
             valence = 0
             # check for SEEDOT_lexicon words that may be used as modifiers or negations
             if item.lower() in BOOSTER_DICT:
@@ -523,15 +545,15 @@
                  "Today only kinda sux! But I'll get by, lol",
                  # mixed sentiment example with slang and constrastive conjunction "but"
                  "Make sure you :) or :D today!",  # emoticons handled
                  "Catch utf-8 emoji such as ðŸ’˜ and ðŸ’‹ and ðŸ˜",  # emojis handled
                  "Not bad at all"  # Capitalized negation
                  ]
 
-    analyzer = Electronic_SIA()
+    analyzer = SIA()
 
     print("----------------------------------------------------")
     print(" - Analyze typical example cases, including handling of:")
     print("  -- negations")
     print("  -- punctuation emphasis & punctuation flooding")
     print("  -- word-shape as emphasis (capitalization difference)")
     print("  -- degree modifiers (intensifiers such as 'very' and dampeners such as 'kind of')")
```

### Comparing `seedot-2.1/setup.cfg` & `seedot-3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = seedot
 author = Seedot
 Author-email = seedotvsvader@gmail.com
 license = MIT
 license-file = LICENSE.txt
 url = https://github.com/SEEDOT1/SEEDOT
-description = This package have 4 dictornaries for doing domain-specific sentiment analysis, the domain are: Food, Finance, Electornic, Hotel. This package work as an extension of the VADER package.
+description = This package allow you to create your own domain oriented dictionary for sentiment analysis by using the seedot procedure, or to use one of the pre built ones (food, financial, electronic, hotel).
 platforms = any
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Topic :: Text Processing :: Linguistic
```

### Comparing `seedot-2.1/setup.py` & `seedot-3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         return f.read()
 
 setup(
   name = 'seedot',
   #packages = ['GROGU'], # this must be the same as the name above
   packages = find_packages(exclude=['tests*']), # a better way to do it than the line above -- this way no typo/transpo errors
   include_package_data=True,
-  version = '2.1',
+  version = '3.0',
   author = ['Seedot'],
   author_email = 'seedotvsvader@gmail.com',
   description = 'SEEDOT: Tool for Enhancing Sentiment Lexicon with Machine Learning',
   long_description = read("README.md"),
   long_description_content_type = "text/markdown",
   license = 'MIT License: http://opensource.org/licenses/MIT',
   #url = 'https://github.com/Lucaa00/Vader_new', # use the URL to the github repo
```

