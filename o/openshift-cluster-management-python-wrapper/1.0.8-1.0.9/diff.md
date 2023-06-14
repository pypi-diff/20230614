# Comparing `tmp/openshift-cluster-management-python-wrapper-1.0.8.tar.gz` & `tmp/openshift-cluster-management-python-wrapper-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-cluster-management-python-wrapper-1.0.8.tar", last modified: Tue Mar 28 12:19:35 2023, max compression
+gzip compressed data, was "openshift-cluster-management-python-wrapper-1.0.9.tar", last modified: Thu Mar 30 08:43:55 2023, max compression
```

## Comparing `openshift-cluster-management-python-wrapper-1.0.8.tar` & `openshift-cluster-management-python-wrapper-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:19:35.115068 openshift-cluster-management-python-wrapper-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-03-28 12:19:31.000000 openshift-cluster-management-python-wrapper-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2076 2023-03-28 12:19:35.115068 openshift-cluster-management-python-wrapper-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1322 2023-03-28 12:19:31.000000 openshift-cluster-management-python-wrapper-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:19:35.115068 openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:19:31.000000 openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12584 2023-03-28 12:19:31.000000 openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/cluster.py
--rw-r--r--   0 root         (0) root         (0)      554 2023-03-28 12:19:31.000000 openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2432 2023-03-28 12:19:31.000000 openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/logger.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-03-28 12:19:31.000000 openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/ocm_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 12:19:35.115068 openshift-cluster-management-python-wrapper-1.0.8/openshift_cluster_management_python_wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2076 2023-03-28 12:19:35.000000 openshift-cluster-management-python-wrapper-1.0.8/openshift_cluster_management_python_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-03-28 12:19:35.000000 openshift-cluster-management-python-wrapper-1.0.8/openshift_cluster_management_python_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 12:19:35.000000 openshift-cluster-management-python-wrapper-1.0.8/openshift_cluster_management_python_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-03-28 12:19:35.000000 openshift-cluster-management-python-wrapper-1.0.8/openshift_cluster_management_python_wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-28 12:19:35.000000 openshift-cluster-management-python-wrapper-1.0.8/openshift_cluster_management_python_wrapper.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      227 2023-03-28 12:19:31.000000 openshift-cluster-management-python-wrapper-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      724 2023-03-28 12:19:35.116068 openshift-cluster-management-python-wrapper-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      496 2023-03-28 12:19:31.000000 openshift-cluster-management-python-wrapper-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 08:43:55.231131 openshift-cluster-management-python-wrapper-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-03-30 08:43:50.000000 openshift-cluster-management-python-wrapper-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-03-30 08:43:55.231131 openshift-cluster-management-python-wrapper-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-03-30 08:43:50.000000 openshift-cluster-management-python-wrapper-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 08:43:55.230131 openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 08:43:50.000000 openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12588 2023-03-30 08:43:50.000000 openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/cluster.py
+-rw-r--r--   0 root         (0) root         (0)      554 2023-03-30 08:43:50.000000 openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-03-30 08:43:50.000000 openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-03-30 08:43:50.000000 openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/ocm_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 08:43:55.230131 openshift-cluster-management-python-wrapper-1.0.9/openshift_cluster_management_python_wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-03-30 08:43:55.000000 openshift-cluster-management-python-wrapper-1.0.9/openshift_cluster_management_python_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2023-03-30 08:43:55.000000 openshift-cluster-management-python-wrapper-1.0.9/openshift_cluster_management_python_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 08:43:55.000000 openshift-cluster-management-python-wrapper-1.0.9/openshift_cluster_management_python_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-03-30 08:43:55.000000 openshift-cluster-management-python-wrapper-1.0.9/openshift_cluster_management_python_wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-03-30 08:43:55.000000 openshift-cluster-management-python-wrapper-1.0.9/openshift_cluster_management_python_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2023-03-30 08:43:50.000000 openshift-cluster-management-python-wrapper-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      724 2023-03-30 08:43:55.231131 openshift-cluster-management-python-wrapper-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      496 2023-03-30 08:43:50.000000 openshift-cluster-management-python-wrapper-1.0.9/setup.py
```

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/LICENSE` & `openshift-cluster-management-python-wrapper-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/PKG-INFO` & `openshift-cluster-management-python-wrapper-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-wrapper
-Version: 1.0.8
+Version: 1.0.9
 Summary: Wrapper around https://github.com/RedHatQE/openshift-cluster-management-python-client
 Home-page: https://github.com/RedHatQE/openshift-cluster-management-python-wrapper
 Author: Ruth Netser
 Author-email: rnetser@redhat.com
 License: apache-2.0
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-cluster-management-python-wrapper/issues
 Project-URL: Documentation, https://openshift-cluster-management-python-wrapper.readthedocs.io/en/latest/
```

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/README.md` & `openshift-cluster-management-python-wrapper-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/cluster.py` & `openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             cluster_id=self.cluster_id
         )
 
     @property
     def kubeconfig(self):
         kubeconfig = yaml.safe_load(self.credentials.kubeconfig)
         # TODO: Remove once https://issues.redhat.com/browse/OCPBUGS-8101 is resolved
-        if self.hosted:
+        if self.hypershift:
             del kubeconfig["clusters"][0]["cluster"]["certificate-authority-data"]
         return kubeconfig
 
     @property
     def ocp_client(self):
         return get_client(config_dict=self.kubeconfig)
```

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/exceptions.py` & `openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/logger.py` & `openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/logger.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/ocm_python_wrapper/ocm_client.py` & `openshift-cluster-management-python-wrapper-1.0.9/ocm_python_wrapper/ocm_client.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/openshift_cluster_management_python_wrapper.egg-info/PKG-INFO` & `openshift-cluster-management-python-wrapper-1.0.9/openshift_cluster_management_python_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-wrapper
-Version: 1.0.8
+Version: 1.0.9
 Summary: Wrapper around https://github.com/RedHatQE/openshift-cluster-management-python-client
 Home-page: https://github.com/RedHatQE/openshift-cluster-management-python-wrapper
 Author: Ruth Netser
 Author-email: rnetser@redhat.com
 License: apache-2.0
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-cluster-management-python-wrapper/issues
 Project-URL: Documentation, https://openshift-cluster-management-python-wrapper.readthedocs.io/en/latest/
```

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/openshift_cluster_management_python_wrapper.egg-info/SOURCES.txt` & `openshift-cluster-management-python-wrapper-1.0.9/openshift_cluster_management_python_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-wrapper-1.0.8/setup.cfg` & `openshift-cluster-management-python-wrapper-1.0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = openshift-cluster-management-python-wrapper
-version = 1.0.8
+version = 1.0.9
 author = Ruth Netser
 author_email = rnetser@redhat.com
 description = Wrapper around https://github.com/RedHatQE/openshift-cluster-management-python-client
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/RedHatQE/openshift-cluster-management-python-wrapper
 project_urls =
```

