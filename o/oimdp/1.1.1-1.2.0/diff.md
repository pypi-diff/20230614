# Comparing `tmp/oimdp-1.1.1.tar.gz` & `tmp/oimdp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oimdp-1.1.1.tar", last modified: Tue Feb 22 16:39:57 2022, max compression
+gzip compressed data, was "oimdp-1.2.0.tar", last modified: Wed Jun 15 20:32:21 2022, max compression
```

## Comparing `oimdp-1.1.1.tar` & `oimdp-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2022-02-22 16:39:57.099437 oimdp-1.1.1/
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1997 2022-02-22 16:39:57.099437 oimdp-1.1.1/PKG-INFO
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1208 2022-02-22 16:34:17.000000 oimdp-1.1.1/README.md
-drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2022-02-22 16:39:57.095437 oimdp-1.1.1/oimdp/
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      119 2022-02-22 16:37:43.000000 oimdp-1.1.1/oimdp/__init__.py
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)    12760 2022-02-22 16:34:17.000000 oimdp-1.1.1/oimdp/parser.py
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     6756 2022-02-22 16:34:17.000000 oimdp-1.1.1/oimdp/structures.py
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1825 2022-02-22 16:34:17.000000 oimdp-1.1.1/oimdp/tags.py
-drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2022-02-22 16:39:57.095437 oimdp-1.1.1/oimdp.egg-info/
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1997 2022-02-22 16:39:56.000000 oimdp-1.1.1/oimdp.egg-info/PKG-INFO
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      202 2022-02-22 16:39:57.000000 oimdp-1.1.1/oimdp.egg-info/SOURCES.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        1 2022-02-22 16:39:56.000000 oimdp-1.1.1/oimdp.egg-info/dependency_links.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        6 2022-02-22 16:39:56.000000 oimdp-1.1.1/oimdp.egg-info/top_level.txt
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)       38 2022-02-22 16:39:57.099437 oimdp-1.1.1/setup.cfg
--rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      480 2022-02-22 16:37:34.000000 oimdp-1.1.1/setup.py
+drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2022-06-15 20:32:21.795644 oimdp-1.2.0/
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1082 2022-02-22 16:34:17.000000 oimdp-1.2.0/LICENSE
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1512 2022-06-15 20:32:21.795644 oimdp-1.2.0/PKG-INFO
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1208 2022-02-22 16:34:17.000000 oimdp-1.2.0/README.md
+drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2022-06-15 20:32:21.795644 oimdp-1.2.0/oimdp/
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      143 2022-06-07 15:22:05.000000 oimdp-1.2.0/oimdp/__init__.py
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)    13117 2022-06-07 19:35:03.000000 oimdp-1.2.0/oimdp/parser.py
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     7112 2022-06-07 15:57:26.000000 oimdp-1.2.0/oimdp/structures.py
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1655 2022-06-07 16:06:14.000000 oimdp-1.2.0/oimdp/tags.py
+drwxrwxr-x   0 rviglian  (1001) rviglian  (1001)        0 2022-06-15 20:32:21.795644 oimdp-1.2.0/oimdp.egg-info/
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)     1512 2022-06-15 20:32:21.000000 oimdp-1.2.0/oimdp.egg-info/PKG-INFO
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      210 2022-06-15 20:32:21.000000 oimdp-1.2.0/oimdp.egg-info/SOURCES.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        1 2022-06-15 20:32:21.000000 oimdp-1.2.0/oimdp.egg-info/dependency_links.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)        6 2022-06-15 20:32:21.000000 oimdp-1.2.0/oimdp.egg-info/top_level.txt
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)       38 2022-06-15 20:32:21.795644 oimdp-1.2.0/setup.cfg
+-rw-rw-r--   0 rviglian  (1001) rviglian  (1001)      480 2022-06-07 15:21:10.000000 oimdp-1.2.0/setup.py
```

### Comparing `oimdp-1.1.1/PKG-INFO` & `oimdp-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 Metadata-Version: 2.1
 Name: oimdp
-Version: 1.1.1
+Version: 1.2.0
 Summary: OpenITI mARkdown Parser
 Home-page: http://github.com/OpenITI/oimdp
 Author: Raff Viglianti
 Author-email: rviglian@umd.edu
 License: UNKNOWN
-Description: # oimdp: OpenITI mARkdown Parser
-        
-        This Python library will parse an [OpenITI mARkdown](https://alraqmiyyat.github.io/mARkdown/) document and return a python class
-        representation of the document structures.
-        
-        ## Usage
-        
-        ```py
-        import oimdp
-        
-        md_file = open("mARkdownfile", "r")
-        text = md_file.read()
-        md_file.close()
-        parsed = oimdp.parse(text)
-        ```
-        
-        ## Parsed structure
-        
-        Please see [the docs](https://openiti.github.io/oimdp/), but here are some highlights:
-        
-        ### Document API
-        
-        `content`: a list of content structures
-        
-        `get_clean_text()`: get the text stripped of markup
-        
-        ### Content structures
-        
-        `Content` classes contain an original value from the document and some extracted content such as a text string or a specific value.
-        
-        Most other structures are listed in sequence (e.g. a `Paragraph` is followed by a `Line`). 
-        
-        `Line` objects and other line-level structures are divided in `PhrasePart` objects.
-        
-        `PhrasePart` are phrase-level tags
-        
-        ## Develop
-        
-        Set up a virtual environment with `venv`
-        
-        ```py
-        python3 -m venv .env
-        ```
-        
-        Activate the virtual environment
-        
-        ```py
-        source .env/bin/activate
-        ```
-        
-        Install
-        
-        ```py
-        python setup.py install
-        ```
-        
-        ## Tests
-        
-        With the environment activated:
-        
-        ```py
-        python tests/test.py
-        ```
 Platform: UNKNOWN
 Requires-Python: >=3.8.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# oimdp: OpenITI mARkdown Parser
+
+This Python library will parse an [OpenITI mARkdown](https://alraqmiyyat.github.io/mARkdown/) document and return a python class
+representation of the document structures.
+
+## Usage
+
+```py
+import oimdp
+
+md_file = open("mARkdownfile", "r")
+text = md_file.read()
+md_file.close()
+parsed = oimdp.parse(text)
+```
+
+## Parsed structure
+
+Please see [the docs](https://openiti.github.io/oimdp/), but here are some highlights:
+
+### Document API
+
+`content`: a list of content structures
+
+`get_clean_text()`: get the text stripped of markup
+
+### Content structures
+
+`Content` classes contain an original value from the document and some extracted content such as a text string or a specific value.
+
+Most other structures are listed in sequence (e.g. a `Paragraph` is followed by a `Line`). 
+
+`Line` objects and other line-level structures are divided in `PhrasePart` objects.
+
+`PhrasePart` are phrase-level tags
+
+## Develop
+
+Set up a virtual environment with `venv`
+
+```py
+python3 -m venv .env
+```
+
+Activate the virtual environment
+
+```py
+source .env/bin/activate
+```
+
+Install
+
+```py
+python setup.py install
+```
+
+## Tests
+
+With the environment activated:
+
+```py
+python tests/test.py
+```
+
```

### Comparing `oimdp-1.1.1/README.md` & `oimdp-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oimdp-1.1.1/oimdp/parser.py` & `oimdp-1.2.0/oimdp/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import sys
 import re
 from .structures import Age, Date, Document, Hemistich, Hukm, Isnad, Matn, NamedEntity, OpenTagAuto, OpenTagUser, PageNumber, Paragraph, Line, RouteDist, RouteFrom, RouteTowa, Verse, Milestone
-from .structures import SectionHeader, Editorial, DictionaryUnit, BioOrEvent
+from .structures import SectionHeader, Editorial, Appendix, Paratext, DictionaryUnit, BioOrEvent
 from .structures import DoxographicalItem, MorphologicalPattern, TextPart
 from .structures import AdministrativeRegion, RouteOrDistance, Riwayat
 from . import tags as t
 
-PAGE_PATTERN = re.compile(r"PageV(\d+)P(\d+)")
+PAGE_PATTERN = rf"{t.PAGE}[^P]+P\d+[AB]?"
+PAGE_PATTERN_GROUPED = rf"{t.PAGE}([^P]+)P(\d+[AB]?)"
+PAGE_RE = re.compile(PAGE_PATTERN_GROUPED)
+MILESTONE_PATTERN = r"Milestone300|ms[A-Z]?\d+"
+HEADER_PATTERN = r"### \|+"
+HEADER_PATTERN_GROUPED = r"### (\|+)"
 OPEN_TAG_CUSTOM_PATTERN = r"@[^@]+?@[^_@]+?_[^_@]+?(?:_[^_@]+?)?@"
 OPEN_TAG_CUSTOM_PATTERN_GROUPED = re.compile(
     r"@([^@]+?)@([^_@]+?)_([^_@]+?)(_([^_@]+?))?@"
 )
 OPEN_TAG_AUTO_PATTERN = r"@[A-Z]{3}@[A-Z]{3,}@[A-Za-z]+@(?:-@[0tf][ftalmr]@)?"
 OPEN_TAG_AUTO_PATTERN_GROUPED = re.compile(
     r"@([A-Z]{3})@([A-Z]{3,})@([A-Za-z]+)@(-@([0tf][ftalmr])@)?"
@@ -31,15 +36,15 @@
     for tag in t.PHRASE_LV_TAGS:
         text_only = text_only.replace(tag, '')
     for tag in NAMED_ENTITIES_PATTERN:
         text_only = re.compile(tag).sub('', text_only)
     # Open tag
     text_only = OPEN_TAG_CUSTOM_PATTERN_GROUPED.sub('', text_only)
     text_only = OPEN_TAG_AUTO_PATTERN_GROUPED.sub('', text_only)
-    text_only = PAGE_PATTERN.sub('', text_only)
+    text_only = PAGE_RE.sub('', text_only)
     return text_only
 
 
 def parse_line(tagged_il: str, index: int, obj=Line, first_token=None):
     """ parse a line text into LineParts by splitting it by tags and patterns """
     # remove line tag
     il = tagged_il.replace(t.LINE, '')
@@ -50,15 +55,15 @@
 
     if text_only == "":
         return None
 
     line = obj(il, text_only)
 
     # Split the line by tags. Make sure patterns do not include subgroups!
-    tokens = re.split(rf"(PageV\d+P\d+|{OPEN_TAG_AUTO_PATTERN}|{OPEN_TAG_CUSTOM_PATTERN}|{'|'.join([re.escape(t) for t in t.PHRASE_LV_TAGS])}|{'|'.join([t for t in NAMED_ENTITIES_PATTERN])})", il)
+    tokens = re.split(rf"({PAGE_PATTERN}|{MILESTONE_PATTERN}|{OPEN_TAG_AUTO_PATTERN}|{OPEN_TAG_CUSTOM_PATTERN}|{'|'.join([re.escape(t) for t in t.PHRASE_LV_TAGS])}|{'|'.join([t for t in NAMED_ENTITIES_PATTERN])})", il)
 
     # Some structures inject a token at the beginning of a line, like a riwāyaŧ's isnād
     if first_token:
         line.add_part(first_token(""))
 
     # Named entities include in their `text` property a given number of words from the following text token
     # This variable is used to keep track. A "word" is just a space-separated token.
@@ -72,37 +77,37 @@
         opentagauto_match = None
 
         if token.startswith('@'):
             opentag_match = OPEN_TAG_CUSTOM_PATTERN_GROUPED.match(token)
             opentagauto_match = OPEN_TAG_AUTO_PATTERN_GROUPED.match(token)
 
         if t.PAGE in token:
-            m = PAGE_PATTERN.search(token)
+            m = PAGE_RE.search(token)
             try:
                 line.add_part(PageNumber(token, m.group(1), m.group(2)))
             except Exception:
                 raise Exception(
                     'Could not parse page number at line: ' + str(index+1)
                 )
+        elif re.compile(MILESTONE_PATTERN).match(token):
+            line.add_part(Milestone(token))
         elif opentag_match:
             line.add_part(OpenTagUser(token, 
                 opentag_match.group(1),  # user
                 opentag_match.group(2),  # t_type
                 opentag_match.group(3),  # t_subtype
                 opentag_match.group(5))) # t_subsubtype
         elif opentagauto_match:
             line.add_part(OpenTagAuto(token, 
                 opentagauto_match.group(1),  # resp
                 opentagauto_match.group(2),  # t_type                
                 opentagauto_match.group(3),  # category
                 opentagauto_match.group(5))) # review
         elif t.HEMI in token:
             line.add_part(Hemistich(token))
-        elif t.MILESTONE in token:
-            line.add_part(Milestone(token))
         elif t.MATN in token:
             line.add_part(Matn(token))
         elif t.HUKM in token:
             line.add_part(Hukm(token))
         elif t.ROUTE_FROM in token:
             line.add_part(RouteFrom(token))
         elif t.ROUTE_TOWA in token:
@@ -145,38 +150,42 @@
             val = token.replace(t.PER, '')
             include_words = int(val[1])
             line.add_part(NamedEntity(token, int(val[0]), include_words, "", 'per'))
         else:
             if include_words > 0:
                 rest = ""
                 words = token.strip().split()
-                for pos, word in enumerate(reversed(words)): # reversing split for r-t-l script
+                for pos, word in enumerate(words):
                     if (pos < include_words):
                         line.parts[-1].text = line.parts[-1].text + word + " "
                     else:
                         rest = rest + word + " "
                 if len(rest):
                     line.add_part(TextPart(rest))
                 include_words = 0
             else:
                 line.add_part(TextPart(token))
     return line
 
 
-def parser(text: str):
+def parser(text: str, strict: bool = False):
     """Parses an OpenITI mARkdown file and returns a Document object"""
     document = Document(text)
 
     # Split input text into lines
     ilines = text.splitlines()
 
     # Magic value
     magic_value = ilines[0]
-
-    if magic_value.strip() != "######OpenITI#":
+    
+    if strict and magic_value.strip() != "######OpenITI#":
+        raise Exception(
+            "This does not appear to be an OpenITI mARkdown document (strict mode)")
+        sys.exit(1)
+    elif not magic_value.strip().startswith("######OpenITI#"):
         raise Exception(
             "This does not appear to be an OpenITI mARkdown document")
         sys.exit(1)
 
     document.set_magic_value(magic_value)
 
     # RE patterns
@@ -198,15 +207,15 @@
             if (il.strip() == t.METAEND):
                 continue
             value = il.split(t.META, 1)[1].strip()
             document.set_simple_metadata_field(il, value)
 
         # Content-level page numbers
         elif (il.startswith(t.PAGE)):
-            pv = PAGE_PATTERN.search(il)
+            pv = PAGE_RE.search(il)
             try:
                 document.add_content(PageNumber(il, pv.group(1), pv.group(2)))
             except Exception:
                 raise Exception(
                     'Could not parse page number at line: ' + str(i+1)
                 )
 
@@ -238,36 +247,31 @@
                 if first_line:
                     document.add_content(first_line)
 
         # Lines
         elif (il.startswith(t.LINE)):
             document.add_content(parse_line(il, i))
 
-        # Editorial section
+        # Sections
         elif (il.startswith(t.EDITORIAL)):
             document.add_content(Editorial(il))
+        elif (il.startswith(t.APPENDIX)):
+            document.add_content(Appendix(il))
+        elif (il.startswith(t.PARATEXT)):
+            document.add_content(Paratext(il))
 
         # Section headers
-        elif (il.startswith(t.HEADER1)):
+        elif (il.startswith(t.HEADER)):
             value = il
-            for tag in t.HEADERS:
-                value = value.replace(tag, '')
+            header_re = re.compile(HEADER_PATTERN_GROUPED)
+            value = header_re.sub('', value)
             # remove other phrase level tags
             value = remove_phrase_lv_tags(value)
-            # TODO: capture tags as PhraseParts
-            level = 1
-            if (t.HEADER5 in il):
-                level = 5
-            elif (t.HEADER4 in il):
-                level = 4
-            elif (t.HEADER3 in il):
-                level = 3
-            elif (t.HEADER2 in il):
-                level = 2
-            
+            level = len(header_re.match(il).group(1))
+
             document.add_content(SectionHeader(il, value, level))
 
         # Dictionary entry
         elif (il.startswith(t.DIC)):
             no_tag = il
             for tag in t.DICTIONARIES:
                 no_tag = no_tag.replace(tag, '')
```

### Comparing `oimdp-1.1.1/oimdp/structures.py` & `oimdp-1.2.0/oimdp/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,30 @@
     """Marks the beginning of an editorial section"""
     def __init__(self, orig: str):
         self.orig = orig
 
     def __str__(self):
         return ""
 
+class Appendix(Content):
+    """Marks the beginning of an appendix"""
+    def __init__(self, orig: str):
+        self.orig = orig
+
+    def __str__(self):
+        return ""
+
+class Paratext(Content):
+    """Marks the beginning of a paratextual section"""
+    def __init__(self, orig: str):
+        self.orig = orig
+
+    def __str__(self):
+        return ""
+
 
 class DictionaryUnit(Content):
     """Marks a dictionary unit"""
     def __init__(self, orig: str, dic_type: str):
         self.orig = orig
         self.dic_type: Literal["nit", "top", "lex", "bib"] = dic_type
```

### Comparing `oimdp-1.1.1/oimdp.egg-info/PKG-INFO` & `oimdp-1.2.0/oimdp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 Metadata-Version: 2.1
 Name: oimdp
-Version: 1.1.1
+Version: 1.2.0
 Summary: OpenITI mARkdown Parser
 Home-page: http://github.com/OpenITI/oimdp
 Author: Raff Viglianti
 Author-email: rviglian@umd.edu
 License: UNKNOWN
-Description: # oimdp: OpenITI mARkdown Parser
-        
-        This Python library will parse an [OpenITI mARkdown](https://alraqmiyyat.github.io/mARkdown/) document and return a python class
-        representation of the document structures.
-        
-        ## Usage
-        
-        ```py
-        import oimdp
-        
-        md_file = open("mARkdownfile", "r")
-        text = md_file.read()
-        md_file.close()
-        parsed = oimdp.parse(text)
-        ```
-        
-        ## Parsed structure
-        
-        Please see [the docs](https://openiti.github.io/oimdp/), but here are some highlights:
-        
-        ### Document API
-        
-        `content`: a list of content structures
-        
-        `get_clean_text()`: get the text stripped of markup
-        
-        ### Content structures
-        
-        `Content` classes contain an original value from the document and some extracted content such as a text string or a specific value.
-        
-        Most other structures are listed in sequence (e.g. a `Paragraph` is followed by a `Line`). 
-        
-        `Line` objects and other line-level structures are divided in `PhrasePart` objects.
-        
-        `PhrasePart` are phrase-level tags
-        
-        ## Develop
-        
-        Set up a virtual environment with `venv`
-        
-        ```py
-        python3 -m venv .env
-        ```
-        
-        Activate the virtual environment
-        
-        ```py
-        source .env/bin/activate
-        ```
-        
-        Install
-        
-        ```py
-        python setup.py install
-        ```
-        
-        ## Tests
-        
-        With the environment activated:
-        
-        ```py
-        python tests/test.py
-        ```
 Platform: UNKNOWN
 Requires-Python: >=3.8.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# oimdp: OpenITI mARkdown Parser
+
+This Python library will parse an [OpenITI mARkdown](https://alraqmiyyat.github.io/mARkdown/) document and return a python class
+representation of the document structures.
+
+## Usage
+
+```py
+import oimdp
+
+md_file = open("mARkdownfile", "r")
+text = md_file.read()
+md_file.close()
+parsed = oimdp.parse(text)
+```
+
+## Parsed structure
+
+Please see [the docs](https://openiti.github.io/oimdp/), but here are some highlights:
+
+### Document API
+
+`content`: a list of content structures
+
+`get_clean_text()`: get the text stripped of markup
+
+### Content structures
+
+`Content` classes contain an original value from the document and some extracted content such as a text string or a specific value.
+
+Most other structures are listed in sequence (e.g. a `Paragraph` is followed by a `Line`). 
+
+`Line` objects and other line-level structures are divided in `PhrasePart` objects.
+
+`PhrasePart` are phrase-level tags
+
+## Develop
+
+Set up a virtual environment with `venv`
+
+```py
+python3 -m venv .env
+```
+
+Activate the virtual environment
+
+```py
+source .env/bin/activate
+```
+
+Install
+
+```py
+python setup.py install
+```
+
+## Tests
+
+With the environment activated:
+
+```py
+python tests/test.py
+```
+
```

