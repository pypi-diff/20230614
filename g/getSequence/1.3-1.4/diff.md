# Comparing `tmp/getSequence-1.3.tar.gz` & `tmp/getSequence-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getSequence-1.3.tar", last modified: Fri Jul  8 17:13:57 2022, max compression
+gzip compressed data, was "getSequence-1.4.tar", last modified: Tue Nov 22 20:05:05 2022, max compression
```

## Comparing `getSequence-1.3.tar` & `getSequence-1.4.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.362241 getSequence-1.3/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6148 2022-07-08 17:00:45.000000 getSequence-1.3/.DS_Store
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      257 2022-02-07 14:17:58.000000 getSequence-1.3/.codecov.yml
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.358536 getSequence-1.3/.github/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2257 2022-02-07 14:17:58.000000 getSequence-1.3/.github/CONTRIBUTING.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      224 2022-02-07 14:17:58.000000 getSequence-1.3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.358659 getSequence-1.3/.github/workflows/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2049 2022-03-09 18:03:44.000000 getSequence-1.3/.github/workflows/CI.yaml
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1392 2022-07-08 16:38:45.000000 getSequence-1.3/.gitignore
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      328 2022-02-07 14:17:58.000000 getSequence-1.3/.lgtm.yml
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3556 2022-02-07 14:17:58.000000 getSequence-1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1072 2022-02-07 14:17:58.000000 getSequence-1.3/LICENSE
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      145 2022-02-07 14:17:58.000000 getSequence-1.3/MANIFEST.in
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6035 2022-07-08 17:13:57.362303 getSequence-1.3/PKG-INFO
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5724 2022-07-08 16:41:31.000000 getSequence-1.3/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.358796 getSequence-1.3/devtools/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3518 2022-02-07 14:17:58.000000 getSequence-1.3/devtools/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.358938 getSequence-1.3/devtools/conda-envs/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      208 2022-02-07 14:17:58.000000 getSequence-1.3/devtools/conda-envs/test_env.yaml
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.359078 getSequence-1.3/devtools/legacy-miniconda-setup/
--rwxr-xr-x   0 ryanemenecker   (501) staff       (20)     1344 2022-02-07 14:17:58.000000 getSequence-1.3/devtools/legacy-miniconda-setup/before_install.sh
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.359199 getSequence-1.3/devtools/scripts/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3860 2022-02-07 14:17:58.000000 getSequence-1.3/devtools/scripts/create_conda_env.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.360005 getSequence-1.3/docs/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      608 2022-02-07 14:17:58.000000 getSequence-1.3/docs/Makefile
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      590 2022-02-07 14:17:58.000000 getSequence-1.3/docs/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.360123 getSequence-1.3/docs/_static/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      507 2022-02-07 14:17:58.000000 getSequence-1.3/docs/_static/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.360244 getSequence-1.3/docs/_templates/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      470 2022-02-07 14:17:58.000000 getSequence-1.3/docs/_templates/README.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5343 2022-02-07 14:17:58.000000 getSequence-1.3/docs/conf.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1472 2022-03-09 18:25:45.000000 getSequence-1.3/docs/getting_started.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      536 2022-03-09 18:03:00.000000 getSequence-1.3/docs/index.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      779 2022-02-07 14:17:58.000000 getSequence-1.3/docs/make.bat
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.360483 getSequence-1.3/docs/usage/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3433 2022-03-09 17:56:01.000000 getSequence-1.3/docs/usage/command-line.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1620 2022-03-09 17:55:47.000000 getSequence-1.3/docs/usage/using-in-python.rst
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.362660 getSequence-1.3/getSequence/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      306 2022-03-09 17:44:54.000000 getSequence-1.3/getSequence/__init__.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      496 2022-07-08 17:13:57.362692 getSequence-1.3/getSequence/_version.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.361767 getSequence-1.3/getSequence/data/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1139 2022-02-07 14:17:58.000000 getSequence-1.3/getSequence/data/README.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      333 2022-02-07 14:17:58.000000 getSequence-1.3/getSequence/data/look_and_say.dat
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6944 2022-07-08 17:12:03.000000 getSequence-1.3/getSequence/get_sequence.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1048 2022-07-08 16:37:26.000000 getSequence-1.3/getSequence/getseq.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       47 2022-03-09 16:51:05.000000 getSequence-1.3/getSequence/getsequence_exceptions.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.361998 getSequence-1.3/getSequence/tests/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      113 2022-02-07 14:17:58.000000 getSequence-1.3/getSequence/tests/__init__.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      319 2022-02-07 14:17:58.000000 getSequence-1.3/getSequence/tests/test_getSequence.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.361555 getSequence-1.3/getSequence.egg-info/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6035 2022-07-08 17:13:57.000000 getSequence-1.3/getSequence.egg-info/PKG-INFO
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1006 2022-07-08 17:13:57.000000 getSequence-1.3/getSequence.egg-info/SOURCES.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)        1 2022-07-08 17:13:57.000000 getSequence-1.3/getSequence.egg-info/dependency_links.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       17 2022-07-08 17:13:57.000000 getSequence-1.3/getSequence.egg-info/requires.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       12 2022-07-08 17:13:57.000000 getSequence-1.3/getSequence.egg-info/top_level.txt
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-07-08 17:13:57.362134 getSequence-1.3/scripts/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1460 2022-07-08 16:37:31.000000 getSequence-1.3/scripts/getseq
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      360 2022-07-08 17:13:57.362533 getSequence-1.3/setup.cfg
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2269 2022-07-08 17:11:58.000000 getSequence-1.3/setup.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    68611 2022-02-07 14:17:58.000000 getSequence-1.3/versioneer.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.969765 getSequence-1.4/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     6148 2022-07-08 17:00:45.000000 getSequence-1.4/.DS_Store
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      257 2022-02-07 14:17:58.000000 getSequence-1.4/.codecov.yml
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.965085 getSequence-1.4/.github/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2257 2022-02-07 14:17:58.000000 getSequence-1.4/.github/CONTRIBUTING.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      224 2022-02-07 14:17:58.000000 getSequence-1.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.965247 getSequence-1.4/.github/workflows/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2049 2022-03-09 18:03:44.000000 getSequence-1.4/.github/workflows/CI.yaml
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1392 2022-07-08 16:38:45.000000 getSequence-1.4/.gitignore
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      328 2022-02-07 14:17:58.000000 getSequence-1.4/.lgtm.yml
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3556 2022-02-07 14:17:58.000000 getSequence-1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1072 2022-02-07 14:17:58.000000 getSequence-1.4/LICENSE
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      145 2022-02-07 14:17:58.000000 getSequence-1.4/MANIFEST.in
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     6035 2022-11-22 20:05:05.969869 getSequence-1.4/PKG-INFO
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5724 2022-07-08 16:41:31.000000 getSequence-1.4/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.965381 getSequence-1.4/devtools/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3518 2022-02-07 14:17:58.000000 getSequence-1.4/devtools/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.965518 getSequence-1.4/devtools/conda-envs/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      208 2022-02-07 14:17:58.000000 getSequence-1.4/devtools/conda-envs/test_env.yaml
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.965669 getSequence-1.4/devtools/legacy-miniconda-setup/
+-rwxr-xr-x   0 ryanemenecker   (501) staff       (20)     1344 2022-02-07 14:17:58.000000 getSequence-1.4/devtools/legacy-miniconda-setup/before_install.sh
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.965821 getSequence-1.4/devtools/scripts/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3860 2022-02-07 14:17:58.000000 getSequence-1.4/devtools/scripts/create_conda_env.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.966483 getSequence-1.4/docs/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      608 2022-02-07 14:17:58.000000 getSequence-1.4/docs/Makefile
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      590 2022-02-07 14:17:58.000000 getSequence-1.4/docs/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.966595 getSequence-1.4/docs/_static/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      507 2022-02-07 14:17:58.000000 getSequence-1.4/docs/_static/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.966702 getSequence-1.4/docs/_templates/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      470 2022-02-07 14:17:58.000000 getSequence-1.4/docs/_templates/README.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5343 2022-02-07 14:17:58.000000 getSequence-1.4/docs/conf.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1472 2022-03-09 18:25:45.000000 getSequence-1.4/docs/getting_started.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      536 2022-03-09 18:03:00.000000 getSequence-1.4/docs/index.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      779 2022-02-07 14:17:58.000000 getSequence-1.4/docs/make.bat
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.966930 getSequence-1.4/docs/usage/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3433 2022-03-09 17:56:01.000000 getSequence-1.4/docs/usage/command-line.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1620 2022-03-09 17:55:47.000000 getSequence-1.4/docs/usage/using-in-python.rst
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.970291 getSequence-1.4/getSequence/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      306 2022-03-09 17:44:54.000000 getSequence-1.4/getSequence/__init__.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      496 2022-11-22 20:05:05.970326 getSequence-1.4/getSequence/_version.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.969192 getSequence-1.4/getSequence/data/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1139 2022-02-07 14:17:58.000000 getSequence-1.4/getSequence/data/README.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      333 2022-02-07 14:17:58.000000 getSequence-1.4/getSequence/data/look_and_say.dat
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     6944 2022-08-10 16:19:51.000000 getSequence-1.4/getSequence/get_sequence.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1681 2022-11-22 19:59:39.000000 getSequence-1.4/getSequence/getseq.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       47 2022-03-09 16:51:05.000000 getSequence-1.4/getSequence/getsequence_exceptions.py
+-rw-------   0 ryanemenecker   (501) staff       (20)  1154428 2022-11-22 16:52:54.000000 getSequence-1.4/getSequence/screenshot.png
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.969423 getSequence-1.4/getSequence/tests/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      113 2022-02-07 14:17:58.000000 getSequence-1.4/getSequence/tests/__init__.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      319 2022-02-07 14:17:58.000000 getSequence-1.4/getSequence/tests/test_getSequence.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     4366 2022-11-22 19:49:31.000000 getSequence-1.4/getSequence/vis_sequence.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.968970 getSequence-1.4/getSequence.egg-info/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     6035 2022-11-22 20:05:05.000000 getSequence-1.4/getSequence.egg-info/PKG-INFO
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1076 2022-11-22 20:05:05.000000 getSequence-1.4/getSequence.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)        1 2022-11-22 20:05:05.000000 getSequence-1.4/getSequence.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       17 2022-11-22 20:05:05.000000 getSequence-1.4/getSequence.egg-info/requires.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       12 2022-11-22 20:05:05.000000 getSequence-1.4/getSequence.egg-info/top_level.txt
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2022-11-22 20:05:05.969634 getSequence-1.4/scripts/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1460 2022-07-08 16:37:31.000000 getSequence-1.4/scripts/getseq
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1342 2022-11-22 20:02:42.000000 getSequence-1.4/scripts/visseq
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      360 2022-11-22 20:05:05.970150 getSequence-1.4/setup.cfg
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2299 2022-11-22 19:56:28.000000 getSequence-1.4/setup.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    68611 2022-02-07 14:17:58.000000 getSequence-1.4/versioneer.py
```

### Comparing `getSequence-1.3/.DS_Store` & `getSequence-1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/.github/CONTRIBUTING.md` & `getSequence-1.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/.github/workflows/CI.yaml` & `getSequence-1.4/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/.gitignore` & `getSequence-1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/CODE_OF_CONDUCT.md` & `getSequence-1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/LICENSE` & `getSequence-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/PKG-INFO` & `getSequence-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getSequence
-Version: 1.3
+Version: 1.4
 Summary: A CLI to get a uniprot sequence returned to terminal
 Home-page: UNKNOWN
 Author: Ryan Emenecker
 Author-email: remenecker@wustl.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

### Comparing `getSequence-1.3/README.md` & `getSequence-1.4/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/devtools/README.md` & `getSequence-1.4/devtools/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/devtools/legacy-miniconda-setup/before_install.sh` & `getSequence-1.4/devtools/legacy-miniconda-setup/before_install.sh`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/devtools/scripts/create_conda_env.py` & `getSequence-1.4/devtools/scripts/create_conda_env.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/docs/Makefile` & `getSequence-1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/docs/README.md` & `getSequence-1.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/docs/conf.py` & `getSequence-1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/docs/getting_started.rst` & `getSequence-1.4/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/docs/index.rst` & `getSequence-1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/docs/make.bat` & `getSequence-1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/docs/usage/command-line.rst` & `getSequence-1.4/docs/usage/command-line.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/docs/usage/using-in-python.rst` & `getSequence-1.4/docs/usage/using-in-python.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/getSequence/data/README.md` & `getSequence-1.4/getSequence/data/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/getSequence/get_sequence.py` & `getSequence-1.4/getSequence/get_sequence.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/getSequence.egg-info/PKG-INFO` & `getSequence-1.4/getSequence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getSequence
-Version: 1.3
+Version: 1.4
 Summary: A CLI to get a uniprot sequence returned to terminal
 Home-page: UNKNOWN
 Author: Ryan Emenecker
 Author-email: remenecker@wustl.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

### Comparing `getSequence-1.3/scripts/getseq` & `getSequence-1.4/scripts/getseq`

 * *Files identical despite different names*

### Comparing `getSequence-1.3/setup.py` & `getSequence-1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     # Optional include package data to ship with your package
     # Customize MANIFEST.in if the general case does not suit your needs
     # Comment out this line to prevent the files from being packaged with your software
     include_package_data=True,
 
     # Allows `setup.py test` to work correctly with pytest
     setup_requires=[] + pytest_runner,
-    scripts=['scripts/getseq'],
+    scripts=['scripts/getseq',
+            'scripts/visseq'],
 
     # Additional entries you may want simply uncomment the lines you want and fill in the data
     # url='http://www.my_package.com',  # Website
     install_requires=['urllib3',
                     'requests'],              # Required packages, pulls from pip if needed; do not use for Conda deployment
     # platforms=['Linux',
     #            'Mac OS-X',
```

### Comparing `getSequence-1.3/versioneer.py` & `getSequence-1.4/versioneer.py`

 * *Files identical despite different names*

