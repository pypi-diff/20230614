# Comparing `tmp/gaohn-common-utils-0.0.51.tar.gz` & `tmp/gaohn-common-utils-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.51.tar", last modified: Wed Jun 14 10:17:40 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.52.tar", last modified: Wed Jun 14 11:00:39 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.51.tar` & `gaohn-common-utils-0.0.52.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.182505 gaohn-common-utils-0.0.51/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 10:17:40.182505 gaohn-common-utils-0.0.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.178504 gaohn-common-utils-0.0.51/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.178504 gaohn-common-utils-0.0.51/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.174504 gaohn-common-utils-0.0.51/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.178504 gaohn-common-utils-0.0.51/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.178504 gaohn-common-utils-0.0.51/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.182505 gaohn-common-utils-0.0.51/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.182505 gaohn-common-utils-0.0.51/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.174504 gaohn-common-utils-0.0.51/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.182505 gaohn-common-utils-0.0.51/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.182505 gaohn-common-utils-0.0.51/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 10:17:40.182505 gaohn-common-utils-0.0.51/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 10:17:40.000000 gaohn-common-utils-0.0.51/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-14 10:17:40.000000 gaohn-common-utils-0.0.51/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 10:17:40.000000 gaohn-common-utils-0.0.51/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 10:17:40.000000 gaohn-common-utils-0.0.51/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 10:17:40.000000 gaohn-common-utils-0.0.51/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-14 10:17:22.000000 gaohn-common-utils-0.0.51/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 10:17:40.182505 gaohn-common-utils-0.0.51/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.388921 gaohn-common-utils-0.0.52/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 11:00:39.388921 gaohn-common-utils-0.0.52/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.384921 gaohn-common-utils-0.0.52/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.384921 gaohn-common-utils-0.0.52/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.384921 gaohn-common-utils-0.0.52/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.384921 gaohn-common-utils-0.0.52/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.384921 gaohn-common-utils-0.0.52/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.388921 gaohn-common-utils-0.0.52/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.388921 gaohn-common-utils-0.0.52/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.388921 gaohn-common-utils-0.0.52/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.384921 gaohn-common-utils-0.0.52/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.388921 gaohn-common-utils-0.0.52/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.388921 gaohn-common-utils-0.0.52/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:00:39.388921 gaohn-common-utils-0.0.52/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 11:00:39.000000 gaohn-common-utils-0.0.52/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-14 11:00:39.000000 gaohn-common-utils-0.0.52/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:00:39.000000 gaohn-common-utils-0.0.52/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 11:00:39.000000 gaohn-common-utils-0.0.52/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 11:00:39.000000 gaohn-common-utils-0.0.52/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-14 11:00:12.000000 gaohn-common-utils-0.0.52/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:00:39.392921 gaohn-common-utils-0.0.52/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.51/LICENSE` & `gaohn-common-utils-0.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/PKG-INFO` & `gaohn-common-utils-0.0.52/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.51
+Version: 0.0.52
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.51/README.md` & `gaohn-common-utils-0.0.52/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.52/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.52/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.52/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/core/base.py` & `gaohn-common-utils-0.0.52/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/core/common.py` & `gaohn-common-utils-0.0.52/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.52/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.52/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/core/logger.py` & `gaohn-common-utils-0.0.52/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.52/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.51/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.52/common_utils/versioning/git/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,48 @@
 # Setup logging
 logger = Logger(
     module_name=__name__, propagate=False, log_root_dir=None, log_file=None
 ).logger
 
 
 def check_git_status(working_dir: Optional[str] = None) -> Literal[True, False]:
+    """
+    Check the Git status of the working directory. If there are untracked or
+    uncommitted changes, return False.
+
+    Parameters
+    ----------
+    working_dir : str, optional
+        The path of the working directory where the Git command should be executed,
+        by default None. If None, it uses the current working directory.
+
+    Returns
+    -------
+    Literal[True, False]
+        True if there are no untracked or uncommitted changes in the working directory,
+        False otherwise.
+    """
     status_output = (
         subprocess.check_output(["git", "status", "--porcelain"], cwd=working_dir)
         .decode("utf-8")
         .strip()
     )
     return len(status_output) == 0
 
 
 def log_message_if_working_dir_is_none(working_dir: Optional[str] = None) -> None:
+    """
+    Log an informative message if no working directory is provided.
+
+    Parameters
+    ----------
+    working_dir : str, optional
+        The path of the working directory, by default None.
+            If None, an info message is logged.
+    """
     if working_dir is None:
         logger.info("Working directory not provided. Defaulting to current directory.")
     logger.info(f"Working directory: {working_dir}")
 
 
 def get_git_commit_hash(
     working_dir: Optional[str] = None, check_git_status: Literal[True, False] = False
@@ -40,14 +65,17 @@
     the function returns "N/A".
 
     Parameters
     ----------
     working_dir : str, optional
         The path of the working directory where the Git command should be executed,
         by default None. If None, it uses the current working directory ".".
+    check_git_status : Literal[True, False], optional
+        Whether to check if there are untracked or uncommitted changes in the
+        working directory, by default False.
 
     Returns
     -------
     commit_hash : str
         The Git commit hash, or "N/A" if Git is not installed or the working
         directory is not a Git repository.
     """
```

### Comparing `gaohn-common-utils-0.0.51/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.52/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.51
+Version: 0.0.52
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.51/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.52/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 common_utils/core/__init__.py
 common_utils/core/artifacts.py
 common_utils/core/base.py
 common_utils/core/common.py
 common_utils/core/decorators.py
 common_utils/core/file_system_utils.py
 common_utils/core/logger.py
+common_utils/data_validator/base.py
+common_utils/data_validator/core.py
 common_utils/orchestrator/base.py
 common_utils/versioning/dvc/base.py
 common_utils/versioning/dvc/core.py
 common_utils/versioning/git/base.py
 common_utils/versioning/git/core.py
 gaohn_common_utils.egg-info/PKG-INFO
 gaohn_common_utils.egg-info/SOURCES.txt
```

### Comparing `gaohn-common-utils-0.0.51/pyproject.toml` & `gaohn-common-utils-0.0.52/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.51"
+version = "0.0.52"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

