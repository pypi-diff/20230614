# Comparing `tmp/cutlet-0.1.8a1.tar.gz` & `tmp/cutlet-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cutlet-0.1.8a1.tar", last modified: Mon Aug  3 07:44:07 2020, max compression
+gzip compressed data, was "dist/cutlet-0.1.9.tar", last modified: Tue Aug  4 07:49:57 2020, max compression
```

## Comparing `cutlet-0.1.8a1.tar` & `cutlet-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2020-08-03 07:44:07.729139 cutlet-0.1.8a1/
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2020-08-03 07:44:07.729139 cutlet-0.1.8a1/.github/
--rw-r--r--   0 23        (1000) u23       (1000)       13 2020-05-03 11:25:13.000000 cutlet-0.1.8a1/.github/FUNDING.yml
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2020-08-03 07:44:07.729139 cutlet-0.1.8a1/.github/workflows/
--rw-r--r--   0 23        (1000) u23       (1000)      961 2020-07-26 07:36:26.000000 cutlet-0.1.8a1/.github/workflows/linux.yml
--rw-r--r--   0 23        (1000) u23       (1000)       34 2020-04-16 14:31:50.000000 cutlet-0.1.8a1/.gitignore
--rw-r--r--   0 23        (1000) u23       (1000)     1076 2020-04-17 07:15:44.000000 cutlet-0.1.8a1/LICENSE
--rw-r--r--   0 23        (1000) u23       (1000)       64 2020-04-17 07:15:36.000000 cutlet-0.1.8a1/MANIFEST.in
--rw-r--r--   0 23        (1000) u23       (1000)     4171 2020-08-03 07:44:07.729139 cutlet-0.1.8a1/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)     3033 2020-07-10 18:29:55.000000 cutlet-0.1.8a1/README.md
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2020-08-03 07:44:07.729139 cutlet-0.1.8a1/bin/
--rwxr-xr-x   0 23        (1000) u23       (1000)      450 2020-08-03 07:40:14.000000 cutlet-0.1.8a1/bin/cutlet
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2020-08-03 07:44:07.729139 cutlet-0.1.8a1/cutlet/
--rw-r--r--   0 23        (1000) u23       (1000)       22 2020-04-16 08:23:03.000000 cutlet-0.1.8a1/cutlet/__init__.py
--rw-r--r--   0 23        (1000) u23       (1000)     8811 2020-07-28 10:45:06.000000 cutlet-0.1.8a1/cutlet/cutlet.py
--rw-r--r--   0 23        (1000) u23       (1000)       83 2020-07-12 15:29:43.000000 cutlet-0.1.8a1/cutlet/exceptions.tsv
--rw-r--r--   0 23        (1000) u23       (1000)     1973 2020-07-25 12:25:54.000000 cutlet-0.1.8a1/cutlet/mapping.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2020-08-03 07:44:07.729139 cutlet-0.1.8a1/cutlet/test/
--rw-r--r--   0 23        (1000) u23       (1000)     5186 2020-07-26 16:31:08.000000 cutlet-0.1.8a1/cutlet/test/test_basic.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2020-08-03 07:44:07.729139 cutlet-0.1.8a1/cutlet.egg-info/
--rw-r--r--   0 23        (1000) u23       (1000)     4171 2020-08-03 07:44:07.000000 cutlet-0.1.8a1/cutlet.egg-info/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)      381 2020-08-03 07:44:07.000000 cutlet-0.1.8a1/cutlet.egg-info/SOURCES.txt
--rw-r--r--   0 23        (1000) u23       (1000)        1 2020-08-03 07:44:07.000000 cutlet-0.1.8a1/cutlet.egg-info/dependency_links.txt
--rw-r--r--   0 23        (1000) u23       (1000)       24 2020-08-03 07:44:07.000000 cutlet-0.1.8a1/cutlet.egg-info/requires.txt
--rw-r--r--   0 23        (1000) u23       (1000)        7 2020-08-03 07:44:07.000000 cutlet-0.1.8a1/cutlet.egg-info/top_level.txt
--rw-r--r--   0 23        (1000) u23       (1000)   340278 2020-04-16 13:03:07.000000 cutlet-0.1.8a1/cutlet.png
--rw-r--r--   0 23        (1000) u23       (1000)       85 2020-04-16 09:01:54.000000 cutlet-0.1.8a1/pytest.ini
--rw-r--r--   0 23        (1000) u23       (1000)       38 2020-08-03 07:44:07.729139 cutlet-0.1.8a1/setup.cfg
--rw-r--r--   0 23        (1000) u23       (1000)      896 2020-08-03 07:41:27.000000 cutlet-0.1.8a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 07:49:57.482553 cutlet-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 07:49:57.482553 cutlet-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2020-08-04 07:49:20.000000 cutlet-0.1.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 07:49:57.482553 cutlet-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      976 2020-08-04 07:49:20.000000 cutlet-0.1.9/.github/workflows/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       34 2020-08-04 07:49:20.000000 cutlet-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     1076 2020-08-04 07:49:20.000000 cutlet-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       64 2020-08-04 07:49:20.000000 cutlet-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     4169 2020-08-04 07:49:57.482553 cutlet-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3033 2020-08-04 07:49:20.000000 cutlet-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 07:49:57.482553 cutlet-0.1.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (116)      450 2020-08-04 07:49:20.000000 cutlet-0.1.9/bin/cutlet
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 07:49:57.482553 cutlet-0.1.9/cutlet/
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2020-08-04 07:49:20.000000 cutlet-0.1.9/cutlet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8932 2020-08-04 07:49:20.000000 cutlet-0.1.9/cutlet/cutlet.py
+-rw-r--r--   0 runner    (1001) docker     (116)       83 2020-08-04 07:49:20.000000 cutlet-0.1.9/cutlet/exceptions.tsv
+-rw-r--r--   0 runner    (1001) docker     (116)     1973 2020-08-04 07:49:20.000000 cutlet-0.1.9/cutlet/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 07:49:57.482553 cutlet-0.1.9/cutlet/test/
+-rw-r--r--   0 runner    (1001) docker     (116)     5293 2020-08-04 07:49:20.000000 cutlet-0.1.9/cutlet/test/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-04 07:49:57.482553 cutlet-0.1.9/cutlet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4169 2020-08-04 07:49:57.000000 cutlet-0.1.9/cutlet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      381 2020-08-04 07:49:57.000000 cutlet-0.1.9/cutlet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-04 07:49:57.000000 cutlet-0.1.9/cutlet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       24 2020-08-04 07:49:57.000000 cutlet-0.1.9/cutlet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2020-08-04 07:49:57.000000 cutlet-0.1.9/cutlet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)   340278 2020-08-04 07:49:20.000000 cutlet-0.1.9/cutlet.png
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2020-08-04 07:49:20.000000 cutlet-0.1.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-04 07:49:57.482553 cutlet-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      896 2020-08-04 07:49:20.000000 cutlet-0.1.9/setup.py
```

### Comparing `cutlet-0.1.8a1/.github/workflows/linux.yml` & `cutlet-0.1.9/.github/workflows/linux.yml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install deps
       shell: bash
       run: |
-        python -m pip install --upgrade setuptools wheel pip
+        python -m pip install --upgrade setuptools wheel pip setuptools-scm
         pip install fugashi[unidic-lite] jaconv pytest
         pip install .
     - name: Run tests
       run: |
         pytest
     - name: Publish to PyPI if tagged
       if: startsWith(github.ref, 'refs/tags') && matrix.python-version == 3.8
```

### Comparing `cutlet-0.1.8a1/LICENSE` & `cutlet-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cutlet-0.1.8a1/PKG-INFO` & `cutlet-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutlet
-Version: 0.1.8a1
+Version: 0.1.9
 Summary: Romaji converter
 Home-page: https://github.com/polm/cutlet
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: UNKNOWN
 Description: [![Current PyPI packages](https://badge.fury.io/py/cutlet.svg)](https://pypi.org/project/cutlet/)
```

### Comparing `cutlet-0.1.8a1/README.md` & `cutlet-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cutlet-0.1.8a1/cutlet/cutlet.py` & `cutlet-0.1.9/cutlet/cutlet.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,16 @@
         complete sentence.
         """
         if not text:
             return ''
 
         # convert all full-width alphanum to half-width, since it can go out as-is
         text = mojimoji.zen_to_han(text, kana=False)
+        # replace half-width katakana with full-width
+        text = mojimoji.han_to_zen(text, digit=False, ascii=False)
 
         words = self.tagger(text)
 
         out = ''
 
         for wi, word in enumerate(words):
             pw = words[wi - 1] if wi > 0 else None
```

### Comparing `cutlet-0.1.8a1/cutlet/mapping.py` & `cutlet-0.1.9/cutlet/mapping.py`

 * *Files identical despite different names*

### Comparing `cutlet-0.1.8a1/cutlet/test/test_basic.py` & `cutlet-0.1.9/cutlet/test/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,17 @@
             "Amagami Sincerely Y o u r S shinshiariiyuaazu"),
         ("ケメコデラックス", "Kemekoderakkusu"),
         ("プププランド", "Pupupurando"),
         # Add some non-Japanese tests
         ("панда", "?????"),
         ("팬더", "??"),
         ("「彁」は幽霊文字のひとつ", '"?" wa yuurei moji no hitotsu'),
+        # Do half-width katakana
+        ("ﾎﾟｰﾙ", "Paul"),
+        ("ｳｽｲﾎﾝ", "Usuihon"),
         ]
 
 SENTENCES_KUNREI = [
         ("富士見坂", "Huzimi saka"),
         ]
 
 SLUGS = [
```

### Comparing `cutlet-0.1.8a1/cutlet.egg-info/PKG-INFO` & `cutlet-0.1.9/cutlet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutlet
-Version: 0.1.8a1
+Version: 0.1.9
 Summary: Romaji converter
 Home-page: https://github.com/polm/cutlet
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: UNKNOWN
 Description: [![Current PyPI packages](https://badge.fury.io/py/cutlet.svg)](https://pypi.org/project/cutlet/)
```

### Comparing `cutlet-0.1.8a1/cutlet.png` & `cutlet-0.1.9/cutlet.png`

 * *Files identical despite different names*

### Comparing `cutlet-0.1.8a1/setup.py` & `cutlet-0.1.9/setup.py`

 * *Files identical despite different names*

