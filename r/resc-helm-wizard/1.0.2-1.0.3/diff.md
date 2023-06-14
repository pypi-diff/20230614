# Comparing `tmp/resc_helm_wizard-1.0.2.tar.gz` & `tmp/resc_helm_wizard-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_helm_wizard-1.0.2.tar", last modified: Tue Jun  6 15:11:22 2023, max compression
+gzip compressed data, was "resc_helm_wizard-1.0.3.tar", last modified: Wed Jun 14 09:14:11 2023, max compression
```

## Comparing `resc_helm_wizard-1.0.2.tar` & `resc_helm_wizard-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.495168 resc_helm_wizard-1.0.2/images/
--rw-r--r--   0 runner    (1001) docker     (123)  5798246 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/images/RESC_Installation.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.499168 resc_helm_wizard-1.0.2/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/resources/example-values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.491167 resc_helm_wizard-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/src/resc_helm_wizard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/helm_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/helm_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/kubernetes_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/questions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/run_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-06 15:11:14.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:11:22.503168 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 15:11:22.000000 resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:11.064704 resc_helm_wizard-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/src/resc_helm_wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14145 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/helm_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/helm_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/kubernetes_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/questions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/run_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 09:14:05.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:14:11.068704 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 09:14:11.000000 resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/top_level.txt
```

### Comparing `resc_helm_wizard-1.0.2/PKG-INFO` & `resc_helm_wizard-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: resc_helm_wizard
-Version: 1.0.2
+Version: 1.0.3
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-# Helm Values YAML Wizard
+# Repository Scanner Helm Wizard (resc-helm-wizard)
 
 <!-- TABLE OF CONTENTS -->
 ## Table of contents
 1. [About the component](#about-the-component)
 2. [Getting started](#getting-started)
     - [Prerequisites](#prerequisites)
     - [Usage](#usage)
```

### Comparing `resc_helm_wizard-1.0.2/setup.cfg` & `resc_helm_wizard-1.0.3/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [metadata]
 name = resc_helm_wizard
 description = Repository Scanner - Helm Wizard
-version = 1.0.2
+version = 1.0.3
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 requires_python = >=3.9
-include_package_data = False
+include_package_data = True
 zip_safe = False
 package_dir = = src
 packages = find:
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 resc_helm_wizard = 
-	static/*.ini
+	static/*.ini, config/*.yaml
 
 [options.entry_points]
 console_scripts = 
 	resc-helm-wizard = resc_helm_wizard.run_wizard:prompt_questions
 
 [egg_info]
 tag_build =
```

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard/common.py` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import os
 import subprocess
 import sys
 from typing import List
 from urllib.parse import urlparse
 
 # Third Party
+import pkg_resources
 import requests
 import yaml
 
 # First Party
 from resc_helm_wizard import constants, questions
 from resc_helm_wizard.helm_utilities import (
     add_helm_repository,
     install_or_upgrade_helm_release,
-    is_chart_version_already_installed,
-    update_helm_repository
+    is_chart_already_installed,
+    update_helm_repository,
+    validate_helm_deployment_status
 )
 from resc_helm_wizard.helm_value import HelmValue
 from resc_helm_wizard.kubernetes_utilities import create_namespace_if_not_exists
 from resc_helm_wizard.vcs_instance import VcsInstance
 
 logging.basicConfig(level=logging.INFO)
 
@@ -156,16 +158,15 @@
     """
     output_file_generated = False
     output_values_yaml_file = constants.VALUES_FILE
     helm_deployment_help_link = "https://github.com/abnamro/repository-scanner/" \
                                 "blob/main/deployment/kubernetes/README.md"
 
     try:
-        with open(input_values_yaml_file, "r", encoding="utf-8") as file_in:
-            values_dict = yaml.safe_load(file_in)
+        values_dict = read_yaml_file(input_values_yaml_file)
 
         values_dict["resc-database"]["hostOS"] = helm_values.operating_system
         values_dict["resc-database"]["database"]["pvc_path"] = helm_values.db_storage_path
 
         values_dict["resc-rabbitmq"]["filemountType"] = helm_values.operating_system
         values_dict["resc-rabbitmq"]["rabbitMQ"]["pvc_path"] = helm_values.rabbitmq_storage_path
 
@@ -191,14 +192,27 @@
         sys.exit(1)
     except KeyError as error:
         logging.error(f"Aborting the program! {error} was missing in {input_values_yaml_file}")
         sys.exit(1)
     return output_file_generated
 
 
+def read_yaml_file(file_path):
+    """
+        Read content of yaml file
+    :param file_path:
+        path of yaml file
+    :return: stream
+        Returns yaml content
+    """
+    with pkg_resources.resource_stream(__name__, file_path) as file_in:
+        data = yaml.safe_load(file_in)
+    return data
+
+
 def get_scheme_host_port_from_url(url: str):
     """
         Get scheme, host, port from url
     :param url:
         url of VCS instance
     :return: str, str, str
         Returns scheme, host, port
@@ -318,21 +332,23 @@
 
     if rule_file_downloaded:
         namespace_created = create_namespace_if_not_exists(namespace_name=constants.NAMESPACE)
 
     if namespace_created:
         # Check if release is already installed
         output = subprocess.run(["helm", "list", "-n", constants.NAMESPACE], capture_output=True, text=True, check=True)
-        # Check if same chart version is already installed
-        version_installed = is_chart_version_already_installed()
-        if constants.RELEASE_NAME in output.stdout and version_installed is True:
+        # Check if deployment is already running
+        chart_installed = is_chart_already_installed()
+        if constants.RELEASE_NAME in output.stdout and chart_installed:
             run_upgrade_confirm_msg = f"Release {constants.RELEASE_NAME} is already installed in " \
                                       f"{constants.NAMESPACE} namespace. Do you want to upgrade the release?"
             run_upgrade_confirm = questions.ask_user_confirmation(msg=run_upgrade_confirm_msg)
             if run_upgrade_confirm is True:
                 deployment_status = install_or_upgrade_helm_release(action="upgrade")
+                validate_helm_deployment_status()
             else:
                 logging.info("Skipping deployment...")
 
         else:
             deployment_status = install_or_upgrade_helm_release(action="install")
+            validate_helm_deployment_status()
     return deployment_status
```

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard/helm_utilities.py` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard/helm_utilities.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,39 +27,38 @@
         logging.info(output.decode("utf-8"))
         return True
     except subprocess.CalledProcessError:
         logging.error(f"An error occurred during {constants.CHART_NAME} deployment")
         return False
 
 
-def is_chart_version_already_installed() -> bool:
+def get_deployment_status_from_installed_chart() -> str:
     """
-        Checks if chart installed or not
-    :return: bool
-        Returns true if chart already installed else returns false
-    """
-    downloaded_version = get_version_from_downloaded_chart()
-    installed_version = get_version_from_installed_chart()
-    return downloaded_version == installed_version
-
-
-def get_version_from_installed_chart() -> str:
-    """
-        Get version of the installed chart
+        Get status of the installed chart
     :return: str
-        Returns version of the installed chart
+        Returns status of the installed chart
     """
     cmd = f"helm list -f {constants.CHART_NAME} -n {constants.NAMESPACE} -o json"
     output = subprocess.check_output(cmd, shell=True)
     chart_info = json.loads(output.decode("utf-8"))
-    if chart_info and "chart" in chart_info[0]:
-        return chart_info[0]["chart"].split("-")[1]
+    if chart_info and "status" in chart_info[0]:
+        return chart_info[0]["status"]
     return None
 
 
+def is_chart_already_installed() -> bool:
+    """
+        Checks if chart installed or not
+    :return: bool
+        Returns true if chart already installed else returns false
+    """
+    status = get_deployment_status_from_installed_chart()
+    return bool(status == "deployed")
+
+
 def get_version_from_downloaded_chart() -> str:
     """
         Get version of the downloaded chart
     :return: str
         Returns version of the downloaded chart
     """
     cmd = f"helm search repo {constants.HELM_REPO_NAME} -n {constants.NAMESPACE} -o json"
@@ -89,7 +88,22 @@
     """
     cmd = ["helm", "repo", "update", constants.HELM_REPO_NAME]
     try:
         subprocess.run(cmd, check=True)
     except subprocess.CalledProcessError:
         logging.error("An error occurred while updating the helm repository")
         sys.exit(1)
+
+
+def validate_helm_deployment_status():
+    """
+        Validate the status of the helm deployment
+    """
+    try:
+        result = subprocess.run(['helm', 'status', constants.RELEASE_NAME, "-n", constants.NAMESPACE],
+                                capture_output=True, check=True, text=True)
+        output = result.stdout.strip()
+        if "STATUS: deployed" in output:
+            logging.info("The deployment was successful. Visit http://127.0.0.1:30000 to get started with RESC!")
+    except subprocess.CalledProcessError:
+        logging.error("An error occurred during deployment.")
+        sys.exit(1)
```

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard/helm_value.py` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard/helm_value.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard/kubernetes_utilities.py` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard/kubernetes_utilities.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard/questions.py` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard/questions.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard/run_wizard.py` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard/run_wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                     db_password=db_password,
                     db_storage_path=db_storage_path,
                     rabbitmq_storage_path=rabbitmq_storage_path,
                     vcs_instances=vcs_instances
                 )
 
                 common.create_helm_values_yaml(helm_values=helm_values,
-                                               input_values_yaml_file="resources/example-values.yaml")
+                                               input_values_yaml_file="config/example-values.yaml")
                 common.run_deployment_as_per_user_confirmation()
     except KeyboardInterrupt:
         logging.error("Aborting the program! operation cancelled by user")
         sys.exit(-1)
 
 
 if __name__ == '__main__':
```

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard/validator.py` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard/validator.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard/vcs_instance.py` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/PKG-INFO` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: resc-helm-wizard
-Version: 1.0.2
+Version: 1.0.3
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-# Helm Values YAML Wizard
+# Repository Scanner Helm Wizard (resc-helm-wizard)
 
 <!-- TABLE OF CONTENTS -->
 ## Table of contents
 1. [About the component](#about-the-component)
 2. [Getting started](#getting-started)
     - [Prerequisites](#prerequisites)
     - [Usage](#usage)
```

### Comparing `resc_helm_wizard-1.0.2/src/resc_helm_wizard.egg-info/SOURCES.txt` & `resc_helm_wizard-1.0.3/src/resc_helm_wizard.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 setup.cfg
 setup.py
-images/RESC_Installation.gif
-resources/example-values.yaml
 src/resc_helm_wizard/__init__.py
 src/resc_helm_wizard/common.py
 src/resc_helm_wizard/constants.py
 src/resc_helm_wizard/helm_utilities.py
 src/resc_helm_wizard/helm_value.py
 src/resc_helm_wizard/kubernetes_utilities.py
 src/resc_helm_wizard/questions.py
```

