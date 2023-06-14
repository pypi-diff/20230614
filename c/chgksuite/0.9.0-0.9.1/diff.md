# Comparing `tmp/chgksuite-0.9.0.tar.gz` & `tmp/chgksuite-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chgksuite-0.9.0.tar", last modified: Wed Nov 30 21:48:09 2022, max compression
+gzip compressed data, was "chgksuite-0.9.1.tar", last modified: Sun Dec 25 15:30:47 2022, max compression
```

## Comparing `chgksuite-0.9.0.tar` & `chgksuite-0.9.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2022-11-30 21:48:09.509391 chgksuite-0.9.0/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1074 2021-11-20 11:32:47.000000 chgksuite-0.9.0/LICENSE
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      206 2021-11-20 11:32:47.000000 chgksuite-0.9.0/MANIFEST.in
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      709 2022-11-30 21:48:09.508795 chgksuite-0.9.0/PKG-INFO
--rwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)      245 2022-10-08 20:05:46.000000 chgksuite-0.9.0/README.md
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2022-11-30 21:48:09.430960 chgksuite-0.9.0/chgksuite/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/__init__.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      140 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/__main__.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     7718 2022-08-21 17:15:38.000000 chgksuite-0.9.0/chgksuite/common.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)   106200 2022-11-30 21:02:32.000000 chgksuite-0.9.0/chgksuite/composer.py
--rwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)    33100 2022-11-30 21:24:40.000000 chgksuite-0.9.0/chgksuite/gui.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    28867 2022-11-30 21:14:44.000000 chgksuite-0.9.0/chgksuite/parser.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    11775 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/parser_db.py
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2022-11-30 21:48:09.507708 chgksuite-0.9.0/chgksuite/resources/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     3454 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/resources/cheader.tex
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1409 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/resources/fix-unnumbered-sections.sty
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      842 2022-10-22 10:44:36.000000 chgksuite-0.9.0/chgksuite/resources/labels_by.toml
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      616 2022-10-22 10:45:44.000000 chgksuite-0.9.0/chgksuite/resources/labels_en.toml
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      817 2022-10-22 10:46:45.000000 chgksuite-0.9.0/chgksuite/resources/labels_ru.toml
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      823 2022-10-22 10:46:34.000000 chgksuite-0.9.0/chgksuite/resources/labels_ua.toml
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      609 2022-10-23 20:55:10.000000 chgksuite-0.9.0/chgksuite/resources/labels_uz.toml
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      814 2022-10-23 20:55:13.000000 chgksuite-0.9.0/chgksuite/resources/labels_uz_cyr.toml
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      570 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/resources/pptx_config.toml
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1094 2022-10-17 20:20:38.000000 chgksuite-0.9.0/chgksuite/resources/regexes_by.json
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      850 2022-10-17 20:17:16.000000 chgksuite-0.9.0/chgksuite/resources/regexes_en.json
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1470 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/resources/regexes_ru.json
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1145 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/resources/regexes_ua.json
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      886 2022-10-18 20:08:15.000000 chgksuite-0.9.0/chgksuite/resources/regexes_uz_cyr.json
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    11359 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/resources/template.docx
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    29777 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/resources/template.pptx
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      555 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/resources/trello.json
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    11632 2021-11-20 11:32:47.000000 chgksuite-0.9.0/chgksuite/trello.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     7126 2022-11-01 17:19:49.000000 chgksuite-0.9.0/chgksuite/typotools.py
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       22 2022-11-30 21:16:44.000000 chgksuite-0.9.0/chgksuite/version.py
-drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2022-11-30 21:48:09.438571 chgksuite-0.9.0/chgksuite.egg-info/
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      709 2022-11-30 21:48:09.000000 chgksuite-0.9.0/chgksuite.egg-info/PKG-INFO
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1074 2022-11-30 21:48:09.000000 chgksuite-0.9.0/chgksuite.egg-info/SOURCES.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)        1 2022-11-30 21:48:09.000000 chgksuite-0.9.0/chgksuite.egg-info/dependency_links.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       54 2022-11-30 21:48:09.000000 chgksuite-0.9.0/chgksuite.egg-info/entry_points.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      154 2022-11-30 21:48:09.000000 chgksuite-0.9.0/chgksuite.egg-info/requires.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       10 2022-11-30 21:48:09.000000 chgksuite-0.9.0/chgksuite.egg-info/top_level.txt
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    18616 2022-11-30 21:46:16.000000 chgksuite-0.9.0/history.md
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       38 2022-11-30 21:48:09.509578 chgksuite-0.9.0/setup.cfg
--rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1718 2022-08-13 12:09:57.000000 chgksuite-0.9.0/setup.py
+drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2022-12-25 15:30:47.155099 chgksuite-0.9.1/
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1074 2021-11-20 11:32:47.000000 chgksuite-0.9.1/LICENSE
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      206 2021-11-20 11:32:47.000000 chgksuite-0.9.1/MANIFEST.in
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      708 2022-12-25 15:30:47.154814 chgksuite-0.9.1/PKG-INFO
+-rwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)      245 2022-10-08 20:05:46.000000 chgksuite-0.9.1/README.md
+drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2022-12-25 15:30:47.108985 chgksuite-0.9.1/chgksuite/
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/__init__.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      140 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/__main__.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     7718 2022-08-21 17:15:38.000000 chgksuite-0.9.1/chgksuite/common.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)   106200 2022-11-30 21:02:32.000000 chgksuite-0.9.1/chgksuite/composer.py
+-rwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)    33100 2022-11-30 21:24:40.000000 chgksuite-0.9.1/chgksuite/gui.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    28829 2022-12-10 11:42:47.000000 chgksuite-0.9.1/chgksuite/parser.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    11775 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/parser_db.py
+drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2022-12-25 15:30:47.154251 chgksuite-0.9.1/chgksuite/resources/
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     3454 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/resources/cheader.tex
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1409 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/resources/fix-unnumbered-sections.sty
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      842 2022-10-22 10:44:36.000000 chgksuite-0.9.1/chgksuite/resources/labels_by.toml
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      616 2022-10-22 10:45:44.000000 chgksuite-0.9.1/chgksuite/resources/labels_en.toml
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      817 2022-10-22 10:46:45.000000 chgksuite-0.9.1/chgksuite/resources/labels_ru.toml
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      823 2022-10-22 10:46:34.000000 chgksuite-0.9.1/chgksuite/resources/labels_ua.toml
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      609 2022-10-23 20:55:10.000000 chgksuite-0.9.1/chgksuite/resources/labels_uz.toml
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      814 2022-10-23 20:55:13.000000 chgksuite-0.9.1/chgksuite/resources/labels_uz_cyr.toml
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      570 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/resources/pptx_config.toml
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1094 2022-10-17 20:20:38.000000 chgksuite-0.9.1/chgksuite/resources/regexes_by.json
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      850 2022-10-17 20:17:16.000000 chgksuite-0.9.1/chgksuite/resources/regexes_en.json
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1470 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/resources/regexes_ru.json
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1145 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/resources/regexes_ua.json
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      886 2022-10-18 20:08:15.000000 chgksuite-0.9.1/chgksuite/resources/regexes_uz_cyr.json
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    11359 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/resources/template.docx
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    29777 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/resources/template.pptx
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      555 2021-11-20 11:32:47.000000 chgksuite-0.9.1/chgksuite/resources/trello.json
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    11968 2022-12-25 15:21:38.000000 chgksuite-0.9.1/chgksuite/trello.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     7126 2022-11-01 17:19:49.000000 chgksuite-0.9.1/chgksuite/typotools.py
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       22 2022-12-25 15:25:40.000000 chgksuite-0.9.1/chgksuite/version.py
+drwxr-xr-x   0 pecheny  (1432018558) LD\Domain Users (593637566)        0 2022-12-25 15:30:47.116566 chgksuite-0.9.1/chgksuite.egg-info/
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      708 2022-12-25 15:30:46.000000 chgksuite-0.9.1/chgksuite.egg-info/PKG-INFO
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1074 2022-12-25 15:30:46.000000 chgksuite-0.9.1/chgksuite.egg-info/SOURCES.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)        1 2022-12-25 15:30:46.000000 chgksuite-0.9.1/chgksuite.egg-info/dependency_links.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       54 2022-12-25 15:30:46.000000 chgksuite-0.9.1/chgksuite.egg-info/entry_points.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)      154 2022-12-25 15:30:46.000000 chgksuite-0.9.1/chgksuite.egg-info/requires.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       10 2022-12-25 15:30:46.000000 chgksuite-0.9.1/chgksuite.egg-info/top_level.txt
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)    19077 2022-12-25 15:25:31.000000 chgksuite-0.9.1/history.md
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)       38 2022-12-25 15:30:47.155164 chgksuite-0.9.1/setup.cfg
+-rw-r--r--   0 pecheny  (1432018558) LD\Domain Users (593637566)     1733 2022-12-25 15:28:06.000000 chgksuite-0.9.1/setup.py
```

### Comparing `chgksuite-0.9.0/LICENSE` & `chgksuite-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/PKG-INFO` & `chgksuite-0.9.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chgksuite
-Version: 0.9.0
+Version: 0.9.1
 Summary: A package for chgk automation
 Home-page: https://gitlab.com/peczony/chgksuite
 Author: Alexander Pecheny
 Author-email: peczony@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,8 +13,8 @@
 
 **chgksuite** is an utility that helps chgk editors.
 
 [Chgk](https://en.wikipedia.org/wiki/What%3F_Where%3F_When%3F) (short for Chto? Gde? Kogda?) is a popular russian quiz.
 
 Project home on gitlab: https://gitlab.com/peczony/chgksuite
 
-Documentation (in Russian): https://peczony.gitbook.io/chgksuite
+Documentation (in Russian): https://peczony.gitlab.io/chgksuite
```

### Comparing `chgksuite-0.9.0/chgksuite/common.py` & `chgksuite-0.9.1/chgksuite/common.py`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/composer.py` & `chgksuite-0.9.1/chgksuite/composer.py`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/gui.py` & `chgksuite-0.9.1/chgksuite/gui.py`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/parser.py` & `chgksuite-0.9.1/chgksuite/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,16 +654,15 @@
         if args.fix_spans:
             for tag in bsoup.find_all("span"):
                 tag.unwrap()
         for h in ["h1", "h2", "h3", "h4"]:
             for tag in bsoup.find_all(h):
                 ensure_line_breaks(tag)
         for tag in bsoup.find_all("li"):
-            if tag.string:
-                tag.string = "- " + tag.string
+            ensure_line_breaks(tag)
         for tag in bsoup.find_all("table"):
             table = dashtable.html2md(str(tag))
             tag.insert_before(table)
             tag.extract()
         for tag in bsoup.find_all("hr"):
             tag.extract()
         if args.links == "unwrap":
```

### Comparing `chgksuite-0.9.0/chgksuite/parser_db.py` & `chgksuite-0.9.1/chgksuite/parser_db.py`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/cheader.tex` & `chgksuite-0.9.1/chgksuite/resources/cheader.tex`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/fix-unnumbered-sections.sty` & `chgksuite-0.9.1/chgksuite/resources/fix-unnumbered-sections.sty`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/labels_by.toml` & `chgksuite-0.9.1/chgksuite/resources/labels_by.toml`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/labels_en.toml` & `chgksuite-0.9.1/chgksuite/resources/labels_en.toml`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/labels_ru.toml` & `chgksuite-0.9.1/chgksuite/resources/labels_ru.toml`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/labels_ua.toml` & `chgksuite-0.9.1/chgksuite/resources/labels_ua.toml`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/labels_uz.toml` & `chgksuite-0.9.1/chgksuite/resources/labels_uz.toml`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/labels_uz_cyr.toml` & `chgksuite-0.9.1/chgksuite/resources/labels_uz_cyr.toml`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/pptx_config.toml` & `chgksuite-0.9.1/chgksuite/resources/pptx_config.toml`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/regexes_by.json` & `chgksuite-0.9.1/chgksuite/resources/regexes_by.json`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/regexes_en.json` & `chgksuite-0.9.1/chgksuite/resources/regexes_en.json`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/regexes_ru.json` & `chgksuite-0.9.1/chgksuite/resources/regexes_ru.json`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/regexes_ua.json` & `chgksuite-0.9.1/chgksuite/resources/regexes_ua.json`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/regexes_uz_cyr.json` & `chgksuite-0.9.1/chgksuite/resources/regexes_uz_cyr.json`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/template.docx` & `chgksuite-0.9.1/chgksuite/resources/template.docx`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/template.pptx` & `chgksuite-0.9.1/chgksuite/resources/template.pptx`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/resources/trello.json` & `chgksuite-0.9.1/chgksuite/resources/trello.json`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite/trello.py` & `chgksuite-0.9.1/chgksuite/trello.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         elif card["name"].startswith("#"):
             card_title = card["name"]
             _list_counters[list_id] = 0
         else:
             card_title = "Тема {}. {}".format(_list_counters[list_id], card["name"])
             clear_card_title = card["name"]
 
-        id_ = "singlefile" if args.singlefile else list_name
+        id_ = list_name
 
         if args.si:
             doc_ = _docs[id_]
             group_ = _groups[id_]
             if group_ is None:  # new doc
                 group_ = _groups[id_] = {
                     "paragraph": init_doc(doc_, id_),
@@ -294,20 +294,30 @@
             p = qb_doc.add_paragraph()
             p = qb_doc.add_paragraph()
             p.add_run(pair[1])
             p = qb_doc.add_paragraph()
             p = qb_doc.add_paragraph()
         qb_doc.save("quizbowl.docx")
 
-    for _list in _lists:
-        filename = "{}.4s".format(_list)
+    if args.singlefile:
+        result = []
+        for _list in open_lists:
+            result.extend(_lists[_list["name"]])
+        filename = "singlefile.4s"
         print("outputting {}".format(filename))
         with codecs.open(filename, "w", "utf8") as f:
-            for item in _lists[_list]:
+            for item in result:
                 f.write("\n" + item + "\n")
+    else:
+        for _list in _lists:
+            filename = "{}.4s".format(_list)
+            print("outputting {}".format(filename))
+            with codecs.open(filename, "w", "utf8") as f:
+                for item in _lists[_list]:
+                    f.write("\n" + item + "\n")
 
 
 def get_board_id(path=None):
     print("To communicate with your trello board we need its board_id.")
     print("Your board link looks like this:")
     print()
     print("https://trello.com/b/Bi0z2H49/title-of-your-board")
```

### Comparing `chgksuite-0.9.0/chgksuite/typotools.py` & `chgksuite-0.9.1/chgksuite/typotools.py`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/chgksuite.egg-info/PKG-INFO` & `chgksuite-0.9.1/chgksuite.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chgksuite
-Version: 0.9.0
+Version: 0.9.1
 Summary: A package for chgk automation
 Home-page: https://gitlab.com/peczony/chgksuite
 Author: Alexander Pecheny
 Author-email: peczony@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,8 +13,8 @@
 
 **chgksuite** is an utility that helps chgk editors.
 
 [Chgk](https://en.wikipedia.org/wiki/What%3F_Where%3F_When%3F) (short for Chto? Gde? Kogda?) is a popular russian quiz.
 
 Project home on gitlab: https://gitlab.com/peczony/chgksuite
 
-Documentation (in Russian): https://peczony.gitbook.io/chgksuite
+Documentation (in Russian): https://peczony.gitlab.io/chgksuite
```

### Comparing `chgksuite-0.9.0/chgksuite.egg-info/SOURCES.txt` & `chgksuite-0.9.1/chgksuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chgksuite-0.9.0/history.md` & `chgksuite-0.9.1/history.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # What’s new
 
+## v0.9.1
+
+- **Трелло**: исправлен баг режима `--singlefile` («Склеить всё в один файл»), раньше там перепутывался порядок карточек, теперь не перепутывается. Также задокументировал некоторые флаги для скачивания из Трелло, которые ранее не были задокументированы.
+
 ## v0.9.0
 - **Интернационализация**: теперь язык можно выбирать прямо из интерфейса. Добавлены беларусский, английский, узбекский (латиница и кириллица) языки.
 - **Телеграм**: исправлен баг: теперь длинные комментарии и картинки в ответах не теряются в чате, а прикрепляются реплаем к соответствующему вопросу.
 - **Паверпойнт**: теперь не только картинки, но и текстовые раздаточные материалы оформляются отдельным слайдом перед текстом вопроса.
 
 ## v0.8.8
 Перешёл на новое api Pyrogram.
```

### Comparing `chgksuite-0.9.0/setup.py` & `chgksuite-0.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup
 
 
 def get_version():
     version = {}
-    with open("chgksuite/version.py") as f:
+    with open("chgksuite/version.py", encoding="utf8") as f:
         exec(f.read(), version)
     return version["__version__"]
 
-
 long_description = """**chgksuite** is an utility that helps chgk editors.
 
 [Chgk](https://en.wikipedia.org/wiki/What%3F_Where%3F_When%3F) (short for Chto? Gde? Kogda?) is a popular russian quiz.
 
 Project home on gitlab: https://gitlab.com/peczony/chgksuite
 
-Documentation (in Russian): https://peczony.gitbook.io/chgksuite
+Documentation (in Russian): https://peczony.gitlab.io/chgksuite
 """
 
 
 setup(
     name="chgksuite",
     version=get_version(),
     author="Alexander Pecheny",
```

