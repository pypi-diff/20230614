# Comparing `tmp/rubbrband-0.2.1.tar.gz` & `tmp/rubbrband-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubbrband-0.2.1.tar", last modified: Wed Jun  7 21:46:01 2023, max compression
+gzip compressed data, was "rubbrband-0.2.2.tar", last modified: Wed Jun 14 18:11:28 2023, max compression
```

## Comparing `rubbrband-0.2.1.tar` & `rubbrband-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-07 21:46:01.536896 rubbrband-0.2.1/
--rw-r--r--   0 llewyn     (501) staff       (20)    11357 2023-03-07 10:22:28.000000 rubbrband-0.2.1/LICENSE
--rw-r--r--   0 llewyn     (501) staff       (20)       48 2023-02-24 08:26:52.000000 rubbrband-0.2.1/MANIFEST.in
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-07 21:46:01.536950 rubbrband-0.2.1/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)       54 2023-06-07 21:39:04.000000 rubbrband-0.2.1/README.md
--rw-r--r--   0 llewyn     (501) staff       (20)       93 2023-06-07 21:38:14.000000 rubbrband-0.2.1/pyproject.toml
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-07 21:46:01.536200 rubbrband-0.2.1/rubbrband/
--rw-r--r--   0 llewyn     (501) staff       (20)       61 2023-06-07 21:45:01.000000 rubbrband-0.2.1/rubbrband/__init__.py
--rw-r--r--   0 llewyn     (501) staff       (20)      755 2023-06-07 21:36:24.000000 rubbrband-0.2.1/rubbrband/main.py
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-07 21:46:01.536787 rubbrband-0.2.1/rubbrband.egg-info/
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-07 21:46:01.000000 rubbrband-0.2.1/rubbrband.egg-info/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)      267 2023-06-07 21:46:01.000000 rubbrband-0.2.1/rubbrband.egg-info/SOURCES.txt
--rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-06-07 21:46:01.000000 rubbrband-0.2.1/rubbrband.egg-info/dependency_links.txt
--rw-r--r--   0 llewyn     (501) staff       (20)        9 2023-06-07 21:46:01.000000 rubbrband-0.2.1/rubbrband.egg-info/requires.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-06-07 21:46:01.000000 rubbrband-0.2.1/rubbrband.egg-info/top_level.txt
--rw-r--r--   0 llewyn     (501) staff       (20)      251 2023-06-07 21:46:01.537154 rubbrband-0.2.1/setup.cfg
--rw-r--r--   0 llewyn     (501) staff       (20)      172 2023-06-07 21:37:58.000000 rubbrband-0.2.1/setup.py
+drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-06-14 18:11:28.859135 rubbrband-0.2.2/
+-rw-r--r--   0 darren     (501) staff       (20)    11357 2023-06-13 23:04:48.000000 rubbrband-0.2.2/LICENSE
+-rw-r--r--   0 darren     (501) staff       (20)       48 2023-06-13 23:04:48.000000 rubbrband-0.2.2/MANIFEST.in
+-rw-r--r--   0 darren     (501) staff       (20)      125 2023-06-14 18:11:28.859204 rubbrband-0.2.2/PKG-INFO
+-rw-r--r--   0 darren     (501) staff       (20)       54 2023-06-13 23:22:30.000000 rubbrband-0.2.2/README.md
+-rw-r--r--   0 darren     (501) staff       (20)       93 2023-06-13 23:22:30.000000 rubbrband-0.2.2/pyproject.toml
+drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-06-14 18:11:28.857937 rubbrband-0.2.2/rubbrband/
+-rw-r--r--   0 darren     (501) staff       (20)       61 2023-06-13 23:28:05.000000 rubbrband-0.2.2/rubbrband/__init__.py
+-rw-r--r--   0 darren     (501) staff       (20)     2059 2023-06-14 18:11:23.000000 rubbrband-0.2.2/rubbrband/main.py
+drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-06-14 18:11:28.858939 rubbrband-0.2.2/rubbrband.egg-info/
+-rw-r--r--   0 darren     (501) staff       (20)      125 2023-06-14 18:11:28.000000 rubbrband-0.2.2/rubbrband.egg-info/PKG-INFO
+-rw-r--r--   0 darren     (501) staff       (20)      267 2023-06-14 18:11:28.000000 rubbrband-0.2.2/rubbrband.egg-info/SOURCES.txt
+-rw-r--r--   0 darren     (501) staff       (20)        1 2023-06-14 18:11:28.000000 rubbrband-0.2.2/rubbrband.egg-info/dependency_links.txt
+-rw-r--r--   0 darren     (501) staff       (20)        9 2023-06-14 18:11:28.000000 rubbrband-0.2.2/rubbrband.egg-info/requires.txt
+-rw-r--r--   0 darren     (501) staff       (20)       10 2023-06-14 18:11:28.000000 rubbrband-0.2.2/rubbrband.egg-info/top_level.txt
+-rw-r--r--   0 darren     (501) staff       (20)      251 2023-06-14 18:11:28.859527 rubbrband-0.2.2/setup.cfg
+-rw-r--r--   0 darren     (501) staff       (20)      172 2023-06-13 23:22:30.000000 rubbrband-0.2.2/setup.py
```

### Comparing `rubbrband-0.2.1/LICENSE` & `rubbrband-0.2.2/LICENSE`

 * *Files identical despite different names*

