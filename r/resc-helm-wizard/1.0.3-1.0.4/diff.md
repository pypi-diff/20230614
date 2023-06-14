# Comparing `tmp/resc_helm_wizard-1.0.3.tar.gz` & `tmp/resc_helm_wizard-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_helm_wizard-1.0.3.tar", last modified: Wed Jun 14 09:14:11 2023, max compression
+gzip compressed data, was "resc_helm_wizard-1.0.4.tar", last modified: Wed Jun 14 14:13:24 2023, max compression
```

## Comparing `resc_helm_wizard-1.0.3.tar` & `resc_helm_wizard-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:11.064704 resc_helm_wizard-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/src/resc_helm_wizard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14145 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/helm_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/helm_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/kubernetes_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/questions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/run_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.695875 resc_helm_wizard-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/src/resc_helm_wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14145 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/src/resc_helm_wizard/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/config/example-values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/helm_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/helm_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/kubernetes_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/questions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/run_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/top_level.txt
```

### Comparing `resc_helm_wizard-1.0.3/PKG-INFO` & `resc_helm_wizard-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_helm_wizard
-Version: 1.0.3
+Version: 1.0.4
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_helm_wizard-1.0.3/setup.cfg` & `resc_helm_wizard-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_helm_wizard
 description = Repository Scanner - Helm Wizard
-version = 1.0.3
+version = 1.0.4
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard/common.py` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard/common.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard/helm_utilities.py` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard/helm_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,27 +70,27 @@
     return None
 
 
 def add_helm_repository():
     """
         Adds a helm repository
     """
-    cmd = ["helm", "repo", "add", constants.HELM_REPO_NAME, constants.RESC_HELM_REPO_URL]
+    cmd = ["helm", "repo", "add", constants.HELM_REPO_NAME, constants.RESC_HELM_REPO_URL, "-n", constants.NAMESPACE]
     try:
         subprocess.run(cmd, check=True)
     except subprocess.CalledProcessError:
         logging.error("An error occurred while adding the helm repository")
         sys.exit(1)
 
 
 def update_helm_repository():
     """
         Updates a helm repository
     """
-    cmd = ["helm", "repo", "update", constants.HELM_REPO_NAME]
+    cmd = ["helm", "repo", "update", "-n", constants.NAMESPACE]
     try:
         subprocess.run(cmd, check=True)
     except subprocess.CalledProcessError:
         logging.error("An error occurred while updating the helm repository")
         sys.exit(1)
```

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard/helm_value.py` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard/helm_value.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard/kubernetes_utilities.py` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard/kubernetes_utilities.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard/questions.py` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard/questions.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard/run_wizard.py` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard/run_wizard.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard/validator.py` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard/validator.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard/vcs_instance.py` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/PKG-INFO` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-helm-wizard
-Version: 1.0.3
+Version: 1.0.4
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/SOURCES.txt` & `resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 src/resc_helm_wizard/vcs_instance.py
 src/resc_helm_wizard.egg-info/PKG-INFO
 src/resc_helm_wizard.egg-info/SOURCES.txt
 src/resc_helm_wizard.egg-info/dependency_links.txt
 src/resc_helm_wizard.egg-info/entry_points.txt
 src/resc_helm_wizard.egg-info/not-zip-safe
 src/resc_helm_wizard.egg-info/requires.txt
-src/resc_helm_wizard.egg-info/top_level.txt
+src/resc_helm_wizard.egg-info/top_level.txt
+src/resc_helm_wizard/config/example-values.yaml
```

