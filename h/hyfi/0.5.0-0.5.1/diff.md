# Comparing `tmp/hyfi-0.5.0.tar.gz` & `tmp/hyfi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.5.0.tar", max compression
+gzip compressed data, was "hyfi-0.5.1.tar", max compression
```

## Comparing `hyfi-0.5.0.tar` & `hyfi-0.5.1.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0     1071 2023-06-12 08:47:30.230064 hyfi-0.5.0/LICENSE
--rw-r--r--   0        0        0     1632 2023-06-12 08:47:30.230064 hyfi-0.5.0/README.md
--rw-r--r--   0        0        0     4515 2023-06-12 08:47:58.534763 hyfi-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3596 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0      331 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-12 08:47:58.450761 hyfi-0.5.0/src/hyfi/_version.py
--rw-r--r--   0        0        0        0 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-12 08:47:58.450761 hyfi-0.5.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      701 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      717 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      496 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0     1518 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      669 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       21 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    13966 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/config/batch.py
--rw-r--r--   0        0        0    24289 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/env.py
--rw-r--r--   0        0        0    12839 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8383 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4318 2023-06-12 08:47:30.234064 hyfi-0.5.0/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2494 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3313 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     7015 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12468 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/io/file.py
--rw-r--r--   0        0        0    28486 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/main.py
--rw-r--r--   0        0        0        0 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2885 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     1997 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    16580 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     1206 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/cached_path/version.py
--rw-r--r--   0        0        0     6131 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/copier.py
--rw-r--r--   0        0        0     5603 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/env.py
--rw-r--r--   0        0        0     9920 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1064 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3595 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4129 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1986 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9760 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     2022 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/pipe.py
--rw-r--r--   0        0        0     5466 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      154 2023-06-12 08:47:30.238064 hyfi-0.5.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-14 02:57:55.744163 hyfi-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1632 2023-06-14 02:57:55.744163 hyfi-0.5.1/README.md
+-rw-r--r--   0        0        0     4515 2023-06-14 02:58:19.940555 hyfi-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3608 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0      359 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-14 02:58:19.868553 hyfi-0.5.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0        0 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-14 02:58:19.868553 hyfi-0.5.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      320 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      701 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      717 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      123 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      554 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1518 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      669 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       29 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    12765 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0     5800 2023-06-14 02:57:55.748164 hyfi-0.5.1/src/hyfi/config/path.py
+-rw-r--r--   0        0        0    24230 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/env.py
+-rw-r--r--   0        0        0    12839 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8383 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4318 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2494 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3313 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     6819 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12468 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    28965 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/main.py
+-rw-r--r--   0        0        0        0 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    16580 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     1206 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/cached_path/version.py
+-rw-r--r--   0        0        0     6131 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/copier.py
+-rw-r--r--   0        0        0     5603 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0     9920 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1064 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3595 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4129 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1986 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9760 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     2022 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/pipe.py
+-rw-r--r--   0        0        0     5466 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-14 02:57:55.752164 hyfi-0.5.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.5.1/PKG-INFO
```

### Comparing `hyfi-0.5.0/LICENSE` & `hyfi-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/README.md` & `hyfi-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/pyproject.toml` & `hyfi-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.5.0"
+version = "0.5.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.5.0/src/hyfi/__cli__.py` & `hyfi-0.5.1/src/hyfi/__cli__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Command line interface for HyFI"""
 import os
 from typing import Optional
 
 import hydra
 
-from .env import HyfiConfig, __about__, __hydra_version_base__
-from .main import DictConfig, HyFI, _about, getLogger
-from .utils.copier import Copier
+from hyfi.env import HyfiConfig, __about__, __hydra_version_base__
+from hyfi.main import DictConfig, HyFI, _about, getLogger
+from hyfi.utils.copier import Copier
 
 logger = getLogger(__name__)
 
 
 __config_path__ = "conf"
 __config_name__ = "config"
```

### Comparing `hyfi-0.5.0/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.5.1/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.5.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.5.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.5.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.5.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.5.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/config/batch.py` & `hyfi-0.5.1/src/hyfi/config/batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,23 @@
+import contextlib
 import random
 from pathlib import Path
-from typing import Any, Optional, Union
+from typing import Optional, Union
 
 from omegaconf import DictConfig
 from pydantic import BaseModel, validator
 
-from ..env import ProjectConfig, _to_config, _to_dict, getLogger
-from ..hydra import _compose, _load, _merge, _methods, _print, _save, _save_json
-from ..utils.lib import ensure_import_module
+from hyfi.config.path import PathConfig
+from hyfi.env import ProjectConfig, _to_config, _to_dict, getLogger
+from hyfi.hydra import _compose, _load, _merge, _methods, _print, _save, _save_json
+from hyfi.utils.lib import ensure_import_module
 
 logger = getLogger(__name__)
 
 
-class PathConfig(BaseModel):
-    task_name: str = "default-task"
-    task_root: str = ""
-    batch_name: str = ""
-
-    class Config:
-        extra = "ignore"
-
-    def __init__(self, **data: Any):
-        if not data:
-            data = _compose("path=__batch__")
-            logger.info(
-                "There are no arguments to initilize a config, using default config."
-            )
-        super().__init__(**data)
-
-    @property
-    def root_dir(self):
-        # return as an absolute path
-        return Path(self.task_root).absolute()
-
-    @property
-    def output_dir(self):
-        return self.root_dir / "outputs"
-
-    @property
-    def batch_dir(self):
-        return self.output_dir / self.batch_name
-
-    @property
-    def library_dir(self):
-        return self.root_dir / "libs"
-
-    @property
-    def data_dir(self):
-        return self.root_dir / "data"
-
-    @property
-    def model_dir(self):
-        return self.root_dir / "models"
-
-    @property
-    def cache_dir(self):
-        return self.root_dir / "cache"
-
-    @property
-    def tmp_dir(self):
-        return self.root_dir / "tmp"
-
-    @property
-    def log_dir(self):
-        log_dir = self.root_dir / "logs"
-        log_dir.mkdir(parents=True, exist_ok=True)
-        return log_dir
-
-
 class BaseBatchConfig(BaseModel):
     batch_name: str
     batch_num: int = None
     output_dir: Path = Path.cwd() / "outputs"
     output_suffix: str = None
     output_extention: Optional[str] = ""
     random_seed: bool = True
@@ -312,20 +258,18 @@
             ensure_import_module(name, libpath, liburi, specname, syspath)
 
     def reset(self, objects=None):
         """Reset the memory cache"""
         if isinstance(objects, list):
             for obj in objects:
                 del obj
-        try:
-            from ..utils.gpu import GPUMon
+        with contextlib.suppress(ImportError):
+            from hyfi.utils.gpu import GPUMon
 
             GPUMon.release_gpu_memory()
-        except ImportError:
-            pass
 
 
 class BaseBatchModel(BaseConfigModel):
     batch: BaseBatchConfig = None
 
     class Config:
         arbitrary_types_allowed = True
@@ -390,16 +334,16 @@
         return self.batch.seed
 
     @property
     def batch_dir(self):
         return self.batch.batch_dir
 
     @property
-    def data_dir(self):
-        return self.path.data_dir
+    def dataset_dir(self):
+        return self.path.dataset_dir
 
     @property
     def verbose(self):
         return self.batch.verbose
 
     @property
     def device(self):
```

### Comparing `hyfi-0.5.0/src/hyfi/env.py` & `hyfi-0.5.1/src/hyfi/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import os
-from enum import Enum
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import hydra
 from omegaconf import DictConfig, ListConfig, OmegaConf, SCMode
 from pydantic import BaseModel, BaseSettings, SecretStr, root_validator, validator
 from pydantic.env_settings import SettingsSourceCallable
 
-from .utils.batch import batcher
-from .utils.env import _check_and_set_value, expand_posix_vars, load_dotenv
-from .utils.logging import getLogger, setLogger
-from .utils.notebook import is_notebook, load_extentions, set_matplotlib_formats
+from hyfi.utils.batch import batcher
+from hyfi.utils.env import _check_and_set_value, expand_posix_vars, load_dotenv
+from hyfi.utils.logging import getLogger, setLogger
+from hyfi.utils.notebook import is_notebook, load_extentions, set_matplotlib_formats
 
 logger = getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
 
-DictKeyType = Union[str, bytes, int, Enum, float, bool]
-
 
 def __version__():
     """Returns the version of HyFI"""
-    from ._version import __version__
+    from hyfi._version import __version__
 
     return __version__
 
 
 def _select(
     cfg: Any,
     key: str,
```

### Comparing `hyfi-0.5.0/src/hyfi/hydra.py` & `hyfi-0.5.1/src/hyfi/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/image/collage.py` & `hyfi-0.5.1/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/image/motion.py` & `hyfi-0.5.1/src/hyfi/image/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/image/plot.py` & `hyfi-0.5.1/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/image/utils.py` & `hyfi-0.5.1/src/hyfi/image/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/io/cached_path.py` & `hyfi-0.5.1/src/hyfi/io/cached_path.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,32 +113,32 @@
     cache_dir.mkdir(parents=True, exist_ok=True)
 
     gd_prefix = "gd://"
     if url.startswith(gd_prefix):
         url = url[len(gd_prefix) :]
         _url = url.split(":")
         if len(_url) == 2:
-            id, path = _url
+            id_, path = _url
         else:
-            id = _url[0]
-            path = id
+            id_ = _url[0]
+            path = id_
 
         # If we're using the path!c/d/file.txt syntax, handle it here.
         fname = None
         extraction_path = path
         exclamation_index = path.find("!")
         if extract_archive and exclamation_index >= 0:
             extraction_path = path[:exclamation_index]
             fname = path[exclamation_index + 1 :]
 
-        cache_path = cache_dir / f".{id}" / extraction_path
+        cache_path = cache_dir / f".{id_}" / extraction_path
         cache_path.parent.mkdir(parents=True, exist_ok=True)
 
         cache_path = gdown.cached_download(
-            id=id,
+            id=id_,
             path=cache_path.as_posix(),
             quiet=not verbose,
         )
 
         if extract_archive:
             extraction_path, files = extractall(cache_path, force_extract=force_extract)
 
@@ -193,27 +193,24 @@
         for fname in namelist(f):
             fname = os.path.join(to, fname)
             files.append(fname)
         return files
 
     extraction_name = Path(path).stem
     extraction_path = f"{to}/{extraction_name}"
-    if extraction_path is not None:
-        # If the extracted directory already exists (and is non-empty), then no
-        # need to extract again unless `force_extract=True`.
-        if (
-            os.path.isdir(extraction_path)
-            and os.listdir(extraction_path)
-            and not force_extract
-        ):
-            files = [
-                os.path.join(dirpath, filename)
-                for dirpath, _, filenames in os.walk(extraction_path)
-                for filename in filenames
-            ]
+    if extraction_path and (
+        os.path.isdir(extraction_path)
+        and os.listdir(extraction_path)
+        and not force_extract
+    ):
+        files = [
+            os.path.join(dirpath, filename)
+            for dirpath, _, filenames in os.walk(extraction_path)
+            for filename in filenames
+        ]
 
-            return to, files
+        return to, files
 
     with opener(path, mode) as f:
         f.extractall(path=to)
 
     return to, filelist(f)
```

### Comparing `hyfi-0.5.0/src/hyfi/io/file.py` & `hyfi-0.5.1/src/hyfi/io/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/main.py` & `hyfi-0.5.1/src/hyfi/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import IO, Any, Dict, List, Tuple, Union
 
 from omegaconf import DictConfig, ListConfig, SCMode
 
-from .env import DotEnvConfig, ProjectConfig, __global_config__, _to_config
-from .hydra import (
+from hyfi.env import DotEnvConfig, ProjectConfig, __global_config__, _to_config
+from hyfi.hydra import (
     DictKeyType,
     SpecialKeys,
     __home_path__,
     __hyfi_path__,
     _compose,
     _ensure_kwargs,
     _ensure_list,
@@ -30,29 +30,29 @@
     _select,
     _to_container,
     _to_dict,
     _to_yaml,
     _update,
     _viewsource,
 )
-from .io.cached_path import cached_path
-from .io.file import exists, is_dir, is_file, join_path, mkdir
-from .utils.env import expand_posix_vars, get_osenv, load_dotenv, set_osenv
-from .utils.func import (
+from hyfi.io.cached_path import cached_path
+from hyfi.io.file import exists, is_dir, is_file, join_path, mkdir
+from hyfi.utils.env import expand_posix_vars, get_osenv, load_dotenv, set_osenv
+from hyfi.utils.func import (
     dict_product,
     dict_to_dataframe,
     records_to_dataframe,
     to_dateparm,
     to_datetime,
     to_numeric,
 )
-from .utils.google import mount_google_drive
-from .utils.gpu import nvidia_smi, set_cuda
-from .utils.logging import getLogger, setLogger
-from .utils.notebook import (
+from hyfi.utils.google import mount_google_drive
+from hyfi.utils.gpu import nvidia_smi, set_cuda
+from hyfi.utils.logging import getLogger, setLogger
+from hyfi.utils.notebook import (
     clear_output,
     cprint,
     create_button,
     create_dropdown,
     create_floatslider,
     create_image,
     create_radiobutton,
@@ -60,15 +60,15 @@
     display,
     display_image,
     get_display,
     hide_code_in_slideshow,
     is_colab,
     is_notebook,
 )
-from .utils.pipe import _apply, _pipe
+from hyfi.utils.pipe import _apply, _pipe
 
 logger = getLogger(__name__)
 
 
 def _about(cfg):
     pkg_name = cfg.about.__package_name__
     name = cfg.about.name
@@ -340,44 +340,17 @@
         If it's a remote resource, download the file and cache it, and
         then return the path to the cached file. If it's already a local path,
         make sure the file exists and return the path.
 
         For URLs, the following schemes are all supported out-of-the-box:
 
         * ``http`` and ``https``,
-        * ``s3`` for objects on `AWS S3`_,
-        * ``gs`` for objects on `Google Cloud Storage (GCS)`_, and
         * ``gd`` for objects on `Google Drive`_, and
         * ``hf`` for objects or repositories on `HuggingFace Hub`_.
 
-        Examples
-        --------
-
-        To download a file over ``https``::
-
-            cached_path("https://github.com/allenai/cached_path/blob/main/README.md")
-
-        To download an object on GCS::
-
-            cached_path("gs://allennlp-public-models/lerc-2020-11-18.tar.gz")
-
-        To download the PyTorch weights for the model `epwalsh/bert-xsmall-dummy`_
-        on HuggingFace, you could do::
-
-            cached_path("hf://epwalsh/bert-xsmall-dummy/pytorch_model.bin")
-
-        For paths or URLs that point to a tarfile or zipfile, you can append the path
-        to a specific file within the archive to the ``url_or_filename``, preceeded by a "!".
-        The archive will be automatically extracted (provided you set ``extract_archive`` to ``True``),
-        returning the local path to the specific file. For example::
-
-            cached_path("model.tar.gz!weights.th", extract_archive=True)
-
-        .. _epwalsh/bert-xsmall-dummy: https://huggingface.co/epwalsh/bert-xsmall-dummy
-
         Parameters
         ----------
 
         url_or_filename :
             A URL or path to parse and possibly download.
 
         extract_archive :
@@ -491,15 +464,15 @@
         columns=None,
         index=False,
         filetype="parquet",
         suffix=None,
         verbose=False,
         **kwargs,
     ):
-        from .io.file import save_data
+        from hyfi.io.file import save_data
 
         if filename is None:
             raise ValueError("filename must be specified")
         save_data(
             data,
             filename,
             base_dir=base_dir,
@@ -509,15 +482,15 @@
             suffix=suffix,
             verbose=verbose,
             **kwargs,
         )
 
     @staticmethod
     def load_data(filename=None, base_dir=None, filetype=None, verbose=False, **kwargs):
-        from .io.file import load_data
+        from hyfi.io.file import load_data
 
         if filename is not None:
             filename = str(filename)
         if SpecialKeys.TARGET in kwargs:
             return _instantiate(
                 kwargs,
                 filename=filename,
@@ -535,15 +508,15 @@
             **kwargs,
         )
 
     @staticmethod
     def get_filepaths(
         filename_patterns=None, base_dir=None, recursive=True, verbose=True, **kwargs
     ):
-        from .io.file import get_filepaths
+        from hyfi.io.file import get_filepaths
 
         if filename_patterns is None:
             raise ValueError("filename must be specified")
         return get_filepaths(
             filename_patterns,
             base_dir=base_dir,
             recursive=recursive,
@@ -557,29 +530,29 @@
         columns=None,
         add_key_as_name=False,
         name_column="_name_",
         ignore_index=True,
         verbose=False,
         **kwargs,
     ):
-        from .io.file import concat_data
+        from hyfi.io.file import concat_data
 
         return concat_data(
             data,
             columns=columns,
             add_key_as_name=add_key_as_name,
             name_column=name_column,
             ignore_index=ignore_index,
             verbose=verbose,
             **kwargs,
         )
 
     @staticmethod
     def is_dataframe(data):
-        from .io.file import is_dataframe
+        from hyfi.io.file import is_dataframe
 
         return is_dataframe(data)
 
     @staticmethod
     def is_colab():
         return is_colab()
 
@@ -597,15 +570,15 @@
 
     @staticmethod
     def nvidia_smi():
         return nvidia_smi()
 
     @staticmethod
     def ensure_import_module(name, libpath, liburi, specname=None, syspath=None):
-        from .utils.lib import ensure_import_module
+        from hyfi.utils.lib import ensure_import_module
 
         return ensure_import_module(name, libpath, liburi, specname, syspath)
 
     @staticmethod
     def collage(
         images_or_uris,
         collage_filepath=None,
@@ -618,15 +591,15 @@
         show_filename=False,
         filename_offset=(5, 5),
         fontname=None,
         fontsize=12,
         fontcolor="#000",
         **kwargs,
     ):
-        from .image.collage import collage as _collage
+        from hyfi.image.collage import collage as _collage
 
         return _collage(
             images_or_uris,
             collage_filepath=collage_filepath,
             ncols=ncols,
             max_images=max_images,
             collage_width=collage_width,
@@ -652,15 +625,15 @@
         width=None,
         optimize=True,
         quality=50,
         show=False,
         force=False,
         **kwargs,
     ):
-        from .image.motion import make_gif as _make_gif
+        from hyfi.image.motion import make_gif as _make_gif
 
         return _make_gif(
             image_filepaths=image_filepaths,
             filename_patterns=filename_patterns,
             base_dir=base_dir,
             output_filepath=output_filepath,
             duration=duration,
@@ -778,15 +751,15 @@
         quiet=False,
         find_links=None,
         requirement=None,
         force_reinstall=False,
         verbose=False,
         **kwargs,
     ):
-        from .utils.lib import pip as _pip
+        from hyfi.utils.lib import pip as _pip
 
         return _pip(
             name,
             upgrade,
             prelease,
             editable,
             quiet,
@@ -795,15 +768,15 @@
             force_reinstall,
             verbose,
             **kwargs,
         )
 
     @staticmethod
     def upgrade(prelease=False, quiet=False, force_reinstall=False, **kwargs):
-        from .utils.lib import pip
+        from hyfi.utils.lib import pip
 
         return pip(
             name="hyfi",
             upgrade=True,
             prelease=prelease,
             quiet=quiet,
             force_reinstall=force_reinstall,
@@ -944,21 +917,21 @@
             style,
             layout,
             **kwargs,
         )
 
     @staticmethod
     def get_image_font(fontname=None, fontsize=12):
-        from .image.collage import get_image_font
+        from hyfi.image.collage import get_image_font
 
         return get_image_font(fontname, fontsize)
 
     @staticmethod
     def read(uri, mode="rb", encoding=None, head=None, **kwargs):
-        from .io.file import read as _read
+        from hyfi.io.file import read as _read
 
         return _read(uri, mode, encoding, head, **kwargs)
 
     @staticmethod
     def load_image(
         image_or_uri,
         max_width: int = None,
@@ -966,15 +939,15 @@
         max_pixels: int = None,
         scale: float = 1.0,
         resize_to_multiple_of: int = None,
         crop_box=None,
         mode="RGB",
         **kwargs,
     ):
-        from .image.utils import load_image as _load_image
+        from hyfi.image.utils import load_image as _load_image
 
         return _load_image(
             image_or_uri,
             max_width,
             max_height,
             max_pixels,
             scale,
@@ -1028,47 +1001,76 @@
     ):
         """
         Scale an image to a maximum width, height, or number of pixels.
 
         resample:   Image.NEAREST (0), Image.LANCZOS (1), Image.BILINEAR (2),
                     Image.BICUBIC (3), Image.BOX (4) or Image.HAMMING (5)
         """
-        from .image.utils import scale_image as _scale_image
+        from hyfi.image.utils import scale_image as _scale_image
 
         return _scale_image(
             image,
             max_width,
             max_height,
             max_pixels,
             scale,
             resize_to_multiple_of,
             resample,
         )
 
     @staticmethod
     def copy(src, dst, *, follow_symlinks=True):
+        """
+        Copy a file or directory. This is a wrapper around shutil.copy.
+        If you need to copy an entire directory (including all of its contents), or if you need to overwrite existing files in the destination directory, shutil.copy() would be a better choice.
+
+        Args:
+                src: Path to the file or directory to be copied.
+                dst: Path to the destination directory. If the destination directory does not exist it will be created.
+                follow_symlinks: Whether or not symlinks should be followed
+        """
         import shutil
 
         src = str(src)
         dst = str(dst)
         mkdir(dst)
         shutil.copy(src, dst, follow_symlinks=follow_symlinks)
         logger.info(f"copied {src} to {dst}")
 
     @staticmethod
     def copyfile(src, dst, *, follow_symlinks=True):
+        """
+        Copy a file or directory. This is a wrapper around shutil.copyfile.
+        If you want to copy a single file from one location to another, shutil.copyfile() is the appropriate function to use.
+
+        Args:
+                src: Path to the file or directory to copy.
+                dst: Path to the destination file or directory. If the destination file already exists it will be overwritten.
+                follow_symlinks: Whether to follow symbolic links or not
+        """
         import shutil
 
         src = str(src)
         dst = str(dst)
         shutil.copyfile(src, dst, follow_symlinks=follow_symlinks)
         logger.info(f"copied {src} to {dst}")
 
     @staticmethod
     def gpu_usage(all=False, attrList=None, useOldCode=False):
+        """
+        Show GPU utilization in human readable format. This is a wrapper around the GPUtil library.
+
+        Args:
+                all: If True show all available GPUs ( default : False )
+                attrList: List of attributes to show ( default : None )
+                useOldCode: If True use old code instead of new code ( default : False )
+
+        Returns:
+                A string with the
+        """
         try:
             from GPUtil import showUtilization  # type: ignore
         except ImportError:
             logger.error("GPUtil is not installed. To install, run: pip install GPUtil")
             return
 
         return showUtilization(all, attrList, useOldCode)
```

### Comparing `hyfi-0.5.0/src/hyfi/utils/batch/apply.py` & `hyfi-0.5.1/src/hyfi/utils/batch/apply.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,20 +47,24 @@
 
 class Apply(object):
     # Applies a function to each row of a minibatch
     def __init__(
         self,
         function,
         batcher=None,
-        args=[],
-        kwargs={},
+        args=None,
+        kwargs=None,
         cache=None,
         vectorize=None,
         description="batch_apply",
     ):
+        if args is None:
+            args = []
+        if kwargs is None:
+            kwargs = {}
         self.batcher = Batcher() if batcher is None else batcher
         self.function = function
         self.args = [args]
         self.kwargs = [kwargs]
         self.cache = [cache]
         self.vectorize = [vectorize]
         self.description = description
```

### Comparing `hyfi-0.5.0/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.5.1/src/hyfi/utils/batch/apply_batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,19 @@
     return f(args[0], *f_args, **f_kwargs)
 
 
 class ApplyBatch(object):
     # Applies a function to the entire minibatch. Use this for example on Pandas dataframes, to avoid per-row overhead.
     # Function needs to be applicable to the array/list of values!
     # If not, modify/wrap the function to process a list, or use Apply
-    def __init__(self, function, batcher=None, args=[], kwargs={}):
+    def __init__(self, function, batcher=None, args=None, kwargs=None):
+        if args is None:
+            args = []
+        if kwargs is None:
+            kwargs = {}
         self.batcher = Batcher() if batcher is None else batcher
         self.function = function
         self.args = [args]
         self.kwargs = [kwargs]
 
     def fit(self, data, input_split=False):
         return self
```

### Comparing `hyfi-0.5.0/src/hyfi/utils/batch/batcher.py` & `hyfi-0.5.1/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/__init__.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/_cached_path.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/cache_file.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/common.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/file_lock.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/meta.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/progress.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/__init__.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/beaker.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/hf.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/http.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/schemes/scheme_client.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/testing.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/cached_path/util.py` & `hyfi-0.5.1/src/hyfi/utils/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/copier.py` & `hyfi-0.5.1/src/hyfi/utils/copier.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/env.py` & `hyfi-0.5.1/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/func.py` & `hyfi-0.5.1/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/google.py` & `hyfi-0.5.1/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/gpu.py` & `hyfi-0.5.1/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/lib.py` & `hyfi-0.5.1/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/logging.py` & `hyfi-0.5.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/notebook.py` & `hyfi-0.5.1/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/pipe.py` & `hyfi-0.5.1/src/hyfi/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/src/hyfi/utils/tools.py` & `hyfi-0.5.1/src/hyfi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.5.0/PKG-INFO` & `hyfi-0.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.5.0
+Version: 0.5.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

