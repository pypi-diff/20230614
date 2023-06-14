# Comparing `tmp/defog-0.9.1.tar.gz` & `tmp/defog-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defog-0.9.1.tar", last modified: Mon Jan 30 01:09:24 2023, max compression
+gzip compressed data, was "defog-0.9.2.tar", last modified: Mon Jan 30 01:33:40 2023, max compression
```

## Comparing `defog-0.9.1.tar` & `defog-0.9.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rishabh    (501) staff       (20)        0 2023-01-30 01:09:24.177092 defog-0.9.1/
--rw-r--r--   0 rishabh    (501) staff       (20)     1065 2023-01-13 21:41:47.000000 defog-0.9.1/LICENSE
--rw-r--r--   0 rishabh    (501) staff       (20)      463 2023-01-30 01:09:24.177167 defog-0.9.1/PKG-INFO
--rw-r--r--   0 rishabh    (501) staff       (20)     4119 2023-01-28 00:07:21.000000 defog-0.9.1/README.md
-drwxr-xr-x   0 rishabh    (501) staff       (20)        0 2023-01-30 01:09:24.176050 defog-0.9.1/defog/
--rw-r--r--   0 rishabh    (501) staff       (20)    19752 2023-01-29 23:26:42.000000 defog-0.9.1/defog/__init__.py
-drwxr-xr-x   0 rishabh    (501) staff       (20)        0 2023-01-30 01:09:24.176972 defog-0.9.1/defog.egg-info/
--rw-r--r--   0 rishabh    (501) staff       (20)      463 2023-01-30 01:09:23.000000 defog-0.9.1/defog.egg-info/PKG-INFO
--rw-r--r--   0 rishabh    (501) staff       (20)      198 2023-01-30 01:09:24.000000 defog-0.9.1/defog.egg-info/SOURCES.txt
--rw-r--r--   0 rishabh    (501) staff       (20)        1 2023-01-30 01:09:23.000000 defog-0.9.1/defog.egg-info/dependency_links.txt
--rw-r--r--   0 rishabh    (501) staff       (20)       78 2023-01-30 01:09:24.000000 defog-0.9.1/defog.egg-info/requires.txt
--rw-r--r--   0 rishabh    (501) staff       (20)        6 2023-01-30 01:09:24.000000 defog-0.9.1/defog.egg-info/top_level.txt
--rw-r--r--   0 rishabh    (501) staff       (20)       79 2023-01-30 01:09:24.177406 defog-0.9.1/setup.cfg
--rw-r--r--   0 rishabh    (501) staff       (20)      717 2023-01-30 01:08:53.000000 defog-0.9.1/setup.py
+drwxr-xr-x   0 rishabh    (501) staff       (20)        0 2023-01-30 01:33:40.818140 defog-0.9.2/
+-rw-r--r--   0 rishabh    (501) staff       (20)     1065 2023-01-13 21:41:47.000000 defog-0.9.2/LICENSE
+-rw-r--r--   0 rishabh    (501) staff       (20)      463 2023-01-30 01:33:40.818216 defog-0.9.2/PKG-INFO
+-rw-r--r--   0 rishabh    (501) staff       (20)     4119 2023-01-28 00:07:21.000000 defog-0.9.2/README.md
+drwxr-xr-x   0 rishabh    (501) staff       (20)        0 2023-01-30 01:33:40.817068 defog-0.9.2/defog/
+-rw-r--r--   0 rishabh    (501) staff       (20)    19752 2023-01-29 23:26:42.000000 defog-0.9.2/defog/__init__.py
+drwxr-xr-x   0 rishabh    (501) staff       (20)        0 2023-01-30 01:33:40.818035 defog-0.9.2/defog.egg-info/
+-rw-r--r--   0 rishabh    (501) staff       (20)      463 2023-01-30 01:33:40.000000 defog-0.9.2/defog.egg-info/PKG-INFO
+-rw-r--r--   0 rishabh    (501) staff       (20)      198 2023-01-30 01:33:40.000000 defog-0.9.2/defog.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabh    (501) staff       (20)        1 2023-01-30 01:33:40.000000 defog-0.9.2/defog.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabh    (501) staff       (20)      115 2023-01-30 01:33:40.000000 defog-0.9.2/defog.egg-info/requires.txt
+-rw-r--r--   0 rishabh    (501) staff       (20)        6 2023-01-30 01:33:40.000000 defog-0.9.2/defog.egg-info/top_level.txt
+-rw-r--r--   0 rishabh    (501) staff       (20)       79 2023-01-30 01:33:40.818469 defog-0.9.2/setup.cfg
+-rw-r--r--   0 rishabh    (501) staff       (20)      754 2023-01-30 01:33:10.000000 defog-0.9.2/setup.py
```

### Comparing `defog-0.9.1/LICENSE` & `defog-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `defog-0.9.1/README.md` & `defog-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `defog-0.9.1/defog/__init__.py` & `defog-0.9.2/defog/__init__.py`

 * *Files identical despite different names*

