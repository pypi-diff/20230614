# Comparing `tmp/utils-pandas-0.0.1.tar.gz` & `tmp/utils-pandas-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils-pandas-0.0.1.tar", last modified: Tue Jun 13 20:30:17 2023, max compression
+gzip compressed data, was "utils-pandas-0.0.2.tar", last modified: Wed Jun 14 19:06:06 2023, max compression
```

## Comparing `utils-pandas-0.0.1.tar` & `utils-pandas-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 20:30:17.607833 utils-pandas-0.0.1/
--rw-rw-rw-   0        0        0     1224 2023-06-13 20:30:17.607833 utils-pandas-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-06-13 20:25:09.000000 utils-pandas-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 20:30:17.608997 utils-pandas-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      475 2023-06-13 20:30:12.000000 utils-pandas-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 20:30:17.595866 utils-pandas-0.0.1/utils-pandas/
--rw-rw-rw-   0        0        0        0 2023-06-13 20:23:50.000000 utils-pandas-0.0.1/utils-pandas/__init__.py
--rw-rw-rw-   0        0        0      317 2023-06-13 20:29:14.000000 utils-pandas-0.0.1/utils-pandas/convert.py
-drwxrwxrwx   0        0        0        0 2023-06-13 20:30:17.606835 utils-pandas-0.0.1/utils_pandas.egg-info/
--rw-rw-rw-   0        0        0     1224 2023-06-13 20:30:17.000000 utils-pandas-0.0.1/utils_pandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-13 20:30:17.000000 utils-pandas-0.0.1/utils_pandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 20:30:17.000000 utils-pandas-0.0.1/utils_pandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 20:30:17.000000 utils-pandas-0.0.1/utils_pandas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 19:06:06.814934 utils-pandas-0.0.2/
+-rw-rw-rw-   0        0        0     1224 2023-06-14 19:06:06.813937 utils-pandas-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2023-06-13 20:25:09.000000 utils-pandas-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 19:06:06.814934 utils-pandas-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      475 2023-06-14 19:05:57.000000 utils-pandas-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:06:06.800482 utils-pandas-0.0.2/utils-pandas/
+-rw-rw-rw-   0        0        0        0 2023-06-13 20:23:50.000000 utils-pandas-0.0.2/utils-pandas/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-06-14 19:05:34.000000 utils-pandas-0.0.2/utils-pandas/convert.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:06:06.812939 utils-pandas-0.0.2/utils_pandas.egg-info/
+-rw-rw-rw-   0        0        0     1224 2023-06-14 19:06:06.000000 utils-pandas-0.0.2/utils_pandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-14 19:06:06.000000 utils-pandas-0.0.2/utils_pandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 19:06:06.000000 utils-pandas-0.0.2/utils_pandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-14 19:06:06.000000 utils-pandas-0.0.2/utils_pandas.egg-info/top_level.txt
```

### Comparing `utils-pandas-0.0.1/PKG-INFO` & `utils-pandas-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-pandas
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pacote Python destinado a criar novas funcionalidades para o Pandas
 Description-Content-Type: text/markdown
 
 <h1>Python Package: utils-pandas</h1>
 
 <b>Descrição:</b>
 <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: utils-pandas Version: 0.0.1 Summary: Pacote Python
+Metadata-Version: 2.1 Name: utils-pandas Version: 0.0.2 Summary: Pacote Python
 destinado a criar novas funcionalidades para o Pandas Description-Content-Type:
 text/markdown
 ****** Python Package: utils-pandas ******
 DescriÃ§Ã£o:
 Biblioteca Python com objetivo de criar funcionalidades adicionais para a
 Biblioteca pandas.
 ===============================================================================
```

### Comparing `utils-pandas-0.0.1/README.md` & `utils-pandas-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `utils-pandas-0.0.1/utils_pandas.egg-info/PKG-INFO` & `utils-pandas-0.0.2/utils_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-pandas
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pacote Python destinado a criar novas funcionalidades para o Pandas
 Description-Content-Type: text/markdown
 
 <h1>Python Package: utils-pandas</h1>
 
 <b>Descrição:</b>
 <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: utils-pandas Version: 0.0.1 Summary: Pacote Python
+Metadata-Version: 2.1 Name: utils-pandas Version: 0.0.2 Summary: Pacote Python
 destinado a criar novas funcionalidades para o Pandas Description-Content-Type:
 text/markdown
 ****** Python Package: utils-pandas ******
 DescriÃ§Ã£o:
 Biblioteca Python com objetivo de criar funcionalidades adicionais para a
 Biblioteca pandas.
 ===============================================================================
```

