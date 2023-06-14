# Comparing `tmp/taichu-dataflow-1.0.7.tar.gz` & `tmp/taichu-dataflow-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-dataflow-1.0.7.tar", last modified: Mon Jun 12 08:58:54 2023, max compression
+gzip compressed data, was "dist/taichu-dataflow-1.0.8.tar", last modified: Mon Jun 12 09:26:13 2023, max compression
```

## Comparing `taichu-dataflow-1.0.7.tar` & `taichu-dataflow-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:58:54.478292 taichu-dataflow-1.0.7/
--rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 08:58:54.477875 taichu-dataflow-1.0.7/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)      194 2023-06-12 02:53:15.000000 taichu-dataflow-1.0.7/README.md
--rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-06-12 08:58:54.478405 taichu-dataflow-1.0.7/setup.cfg
--rw-r--r--   0 wangkun    (501) staff       (20)      699 2023-06-12 08:58:51.000000 taichu-dataflow-1.0.7/setup.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:58:54.474876 taichu-dataflow-1.0.7/taichu_dataflow/
--rw-r--r--   0 wangkun    (501) staff       (20)      534 2023-06-12 08:21:43.000000 taichu-dataflow-1.0.7/taichu_dataflow/__init__.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1928 2023-06-12 08:58:26.000000 taichu-dataflow-1.0.7/taichu_dataflow/export_back.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:58:54.477147 taichu-dataflow-1.0.7/taichu_dataflow/storage/
--rw-r--r--   0 wangkun    (501) staff       (20)      475 2023-06-12 08:56:58.000000 taichu-dataflow-1.0.7/taichu_dataflow/storage/__init__.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1340 2023-06-12 08:56:58.000000 taichu-dataflow-1.0.7/taichu_dataflow/storage/alluxio.py
--rw-r--r--   0 wangkun    (501) staff       (20)      437 2023-06-12 02:48:22.000000 taichu-dataflow-1.0.7/taichu_dataflow/storage/env.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:58:54.476148 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/
--rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)      373 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/SOURCES.txt
--rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/dependency_links.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       13 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/requires.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       16 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/top_level.txt
+drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/
+-rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/PKG-INFO
+drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/
+-rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/PKG-INFO
+-rw-r--r--   0 shenli     (501) staff       (20)      401 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/SOURCES.txt
+-rw-r--r--   0 shenli     (501) staff       (20)       13 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/requires.txt
+-rw-r--r--   0 shenli     (501) staff       (20)       16 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/top_level.txt
+-rw-r--r--   0 shenli     (501) staff       (20)        1 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/dependency_links.txt
+-rw-r--r--   0 shenli     (501) staff       (20)      194 2023-06-12 03:14:29.000000 taichu-dataflow-1.0.8/README.md
+-rw-r--r--   0 shenli     (501) staff       (20)      699 2023-06-12 09:25:57.000000 taichu-dataflow-1.0.8/setup.py
+-rw-r--r--   0 shenli     (501) staff       (20)       38 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/setup.cfg
+drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow/
+-rwxrwxrwx   0 shenli     (501) staff       (20)     1151 2023-06-12 08:16:05.000000 taichu-dataflow-1.0.8/taichu_dataflow/filebeat.sh
+-rw-r--r--   0 shenli     (501) staff       (20)      534 2023-06-12 08:16:05.000000 taichu-dataflow-1.0.8/taichu_dataflow/__init__.py
+-rw-r--r--   0 shenli     (501) staff       (20)     1928 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/export_back.py
+drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/
+-rw-r--r--   0 shenli     (501) staff       (20)      437 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/env.py
+-rw-r--r--   0 shenli     (501) staff       (20)     1340 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/alluxio.py
+-rw-r--r--   0 shenli     (501) staff       (20)      475 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `taichu-dataflow-1.0.7/setup.py` & `taichu-dataflow-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     long_description = ''
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='1.0.7',
+        version='1.0.8',
         description='taichu serve is a tool for serving dataflow',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
```

### Comparing `taichu-dataflow-1.0.7/taichu_dataflow/__init__.py` & `taichu-dataflow-1.0.8/taichu_dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-dataflow-1.0.7/taichu_dataflow/export_back.py` & `taichu-dataflow-1.0.8/taichu_dataflow/export_back.py`

 * *Files identical despite different names*

### Comparing `taichu-dataflow-1.0.7/taichu_dataflow/storage/alluxio.py` & `taichu-dataflow-1.0.8/taichu_dataflow/storage/alluxio.py`

 * *Files identical despite different names*

