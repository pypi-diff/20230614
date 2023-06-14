# Comparing `tmp/spark_quality_rules_tools-0.2.5.tar.gz` & `tmp/spark_quality_rules_tools-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.2.5.tar", last modified: Tue Apr 11 23:54:56 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.2.6.tar", last modified: Wed Jun 14 13:40:12 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.2.5.tar` & `spark_quality_rules_tools-0.2.6.tar`

### file list

```diff
@@ -1,33 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.523053 spark_quality_rules_tools-0.2.5/
--rw-rw-rw-   0        0        0     1092 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      155 2023-04-11 23:35:17.000000 spark_quality_rules_tools-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3887 2023-04-11 23:54:56.523053 spark_quality_rules_tools-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3088 2023-04-11 14:27:34.000000 spark_quality_rules_tools-0.2.5/README.md
--rw-rw-rw-   0        0        0       86 2023-04-11 23:54:56.523053 spark_quality_rules_tools-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-04-11 23:54:48.000000 spark_quality_rules_tools-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.469640 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     1728 2023-04-11 14:27:34.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.485270 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    19489 2023-04-11 14:27:34.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.507427 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-11 22:08:20.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2472 2022-07-12 20:46:27.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/dataframe.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.507427 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/external/
--rw-rw-rw-   0        0        0    71803 2022-10-17 12:27:14.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/external/folder_process.png
--rw-rw-rw-   0        0        0     1056 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/memory.py
--rw-rw-rw-   0        0        0     2113 2022-07-28 23:32:51.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.507427 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      716 2022-07-28 16:09:02.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resource/resolve.conf
--rw-rw-rw-   0        0        0    25817 2023-04-11 17:19:50.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3344 2023-04-11 22:30:11.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.523053 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/templates/table.html
-drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.485270 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     3887 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      956 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      243 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 13:40:12.011962 spark_quality_rules_tools-0.2.6/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-06-14 13:40:12.011962 spark_quality_rules_tools-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.2.6/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-14 13:40:12.012963 spark_quality_rules_tools-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-06-14 13:37:36.000000 spark_quality_rules_tools-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:40:11.968323 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     1477 2023-06-14 13:37:36.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:40:11.988328 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    20640 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:40:12.004331 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:40:12.010332 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/resource/resolve.conf
+-rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-06-14 13:40:11.987327 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-06-14 13:40:11.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2023-06-14 13:40:11.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 13:40:11.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-06-14 13:40:11.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-14 13:40:11.000000 spark_quality_rules_tools-0.2.6/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.2.5/LICENSE` & `spark_quality_rules_tools-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.5/PKG-INFO` & `spark_quality_rules_tools-0.2.6/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spark_quality_rules_tools
-Version: 0.2.5
+Name: spark-quality-rules-tools
+Version: 0.2.6
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
@@ -27,85 +27,118 @@
 
 spark_quality_rules_tools is a Python library that implements quality rules in sandbox
 
 ## Installation
 
 The code is packaged for PyPI, so that the installation consists in running:
 
-```sh
-pip install spark-quality-rules-tools --user --upgrade
-```
 
 ## Usage
 
 wrapper run hammurabies
 
-![Process](./spark_quality_rules_tools/utils/external/folder_process.png)
-
-
 ## Sandbox
+## Installation
+```sh
+!yes| pip uninstall spark-quality-rules-tools
+```
 
 ```sh
-import os
+pip install spark-quality-rules-tools --user --upgrade
+```
 
-from spark_quality_rules_tools.functions.generator import dq_path_workspace
-from spark_quality_rules_tools.functions.generator import dq_download_jar
-from spark_quality_rules_tools.functions.generator import dq_extract_parameters
-from spark_quality_rules_tools.functions.generator import dq_run_sandbox
-from spark_quality_rules_tools.functions.generator import dq_spark_session
-from spark_quality_rules_tools.functions.generator import dq_validate_conf
-from spark_quality_rules_tools.functions.generator import dq_validate_rules
+## IMPORTS
+```sh
+import os
+import pyspark
+from spark_quality_rules_tools import dq_path_workspace
+from spark_quality_rules_tools import dq_download_jar
+from spark_quality_rules_tools import dq_spark_session
+from spark_quality_rules_tools import dq_extract_parameters
+from spark_quality_rules_tools import dq_run_sandbox
+from spark_quality_rules_tools import dq_validate_conf
+from spark_quality_rules_tools import dq_validate_rules
+from spark_quality_rules_tools import show_spark_df
+pyspark.sql.dataframe.DataFrame.show2 = show_spark_df
+```
 
+## Variables
+```sh
 project_sda="SDA_37036"
 url_conf = "http://artifactory-gdt.central-02.nextgen.igrupobbva/artifactory/gl-datio-spark-libs-maven-local/com/datiobd/cdd-hammurabi/4.0.9/DQ_LOCAL_CONFS/KCOG/KCOG_branch_MRField.conf"
+```
 
 
-## Create workspace
+## Creating Workspace
+```sh
 dq_path_workspace(project_sda=project_sda)
+```
+
+
+## Download haas jar
+```sh
+dq_download_jar(haas_version="4.8.0", force=True)
+```
 
-## Download Jar Haas
-dq_download_jar(haas_version="4.8.0",
-                force=False)
-                                                      
-## Extract y Show Parameter                                 
+
+## Spark Session
+```sh
+spark, sc = dq_spark_session()
+```
+
+
+## Validate Conf
+```sh
+dq_validate_conf(url_conf=url_conf)
+```
+
+
+## Extract Params
+```sh
 dq_extract_parameters(url_conf=url_conf)
+```
 
 
+## Json params
+```sh
 parameter_conf_list = [
  {      
-    "ARTIFACTORY_UNIQUE_CACHE": "https://globaldevtools.bbva.com",
+    "ARTIFACTORY_UNIQUE_CACHE": "http://artifactory-gdt.central-02.nextgen.igrupobbva",
     "ODATE_DATE": "2022-11-11",
     "COUNTRY_ID": "PE",
     "SCHEMA_PATH": "t_kcog_branch.output.schema",
     "CUTOFF_DATE": "2022-11-11",
-    "SCHEMAS_REPOSITORY": "da-datio/schemas/pe/kcog/master/t_kcog_branch/latest/"
+    "SCHEMAS_REPOSITORY": "gl-datio-da-generic-local/schemas/pe/kcog/master/t_kcog_branch/latest/"
  }
 ]
-                  
-## quality run_sandbox
-dq_run_sandbox(parameter_conf_list=parameter_conf_list,
-               url_conf=url_conf))
-
 ```
 
-## Validations
 
+## Run 
 ```sh
-url_conf = "http://artifactory-gdt.central-02.nextgen.igrupobbva/artifactory/gl-datio-spark-libs-maven-local/com/datiobd/cdd-hammurabi/4.0.9/DQ_LOCAL_CONFS/KCOG/KCOG_branch_MRField.conf"
+dq_run_sandbox(spark=spark,
+               sc=sc,
+               parameter_conf_list=parameter_conf_list,
+               url_conf=url_conf)
+```
 
-## validate conf
-dq_validate_conf(url_conf=url_conf)
+               
+```sh         
+df = spark.read.csv("file:/var/sds/homes/P030772/workspace/data_quality_rules/data_reports/KCOG/KCOG_BRANCH_MRFIELD_202304120046_20221111.csv", 
+                    header=True)                 
+df.show2(100)
+```
 
-## validate rules
-dq_validate_rules(url_conf=url_conf)
 
+## Run 
+```sh
+dq_validate_rules(url_conf=url_conf)
 ```
 
 
-
 ## License
 
 [Apache License 2.0](https://www.dropbox.com/s/8t6xtgk06o3ij61/LICENSE?dl=0).
 
 ## New features v1.0
 
 ## BugFix
```

### Comparing `spark_quality_rules_tools-0.2.5/README.md` & `spark_quality_rules_tools-0.2.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,85 +7,118 @@
 
 spark_quality_rules_tools is a Python library that implements quality rules in sandbox
 
 ## Installation
 
 The code is packaged for PyPI, so that the installation consists in running:
 
-```sh
-pip install spark-quality-rules-tools --user --upgrade
-```
 
 ## Usage
 
 wrapper run hammurabies
 
-![Process](./spark_quality_rules_tools/utils/external/folder_process.png)
-
-
 ## Sandbox
+## Installation
+```sh
+!yes| pip uninstall spark-quality-rules-tools
+```
 
 ```sh
-import os
+pip install spark-quality-rules-tools --user --upgrade
+```
 
-from spark_quality_rules_tools.functions.generator import dq_path_workspace
-from spark_quality_rules_tools.functions.generator import dq_download_jar
-from spark_quality_rules_tools.functions.generator import dq_extract_parameters
-from spark_quality_rules_tools.functions.generator import dq_run_sandbox
-from spark_quality_rules_tools.functions.generator import dq_spark_session
-from spark_quality_rules_tools.functions.generator import dq_validate_conf
-from spark_quality_rules_tools.functions.generator import dq_validate_rules
+## IMPORTS
+```sh
+import os
+import pyspark
+from spark_quality_rules_tools import dq_path_workspace
+from spark_quality_rules_tools import dq_download_jar
+from spark_quality_rules_tools import dq_spark_session
+from spark_quality_rules_tools import dq_extract_parameters
+from spark_quality_rules_tools import dq_run_sandbox
+from spark_quality_rules_tools import dq_validate_conf
+from spark_quality_rules_tools import dq_validate_rules
+from spark_quality_rules_tools import show_spark_df
+pyspark.sql.dataframe.DataFrame.show2 = show_spark_df
+```
 
+## Variables
+```sh
 project_sda="SDA_37036"
 url_conf = "http://artifactory-gdt.central-02.nextgen.igrupobbva/artifactory/gl-datio-spark-libs-maven-local/com/datiobd/cdd-hammurabi/4.0.9/DQ_LOCAL_CONFS/KCOG/KCOG_branch_MRField.conf"
+```
 
 
-## Create workspace
+## Creating Workspace
+```sh
 dq_path_workspace(project_sda=project_sda)
+```
+
+
+## Download haas jar
+```sh
+dq_download_jar(haas_version="4.8.0", force=True)
+```
 
-## Download Jar Haas
-dq_download_jar(haas_version="4.8.0",
-                force=False)
-                                                      
-## Extract y Show Parameter                                 
+
+## Spark Session
+```sh
+spark, sc = dq_spark_session()
+```
+
+
+## Validate Conf
+```sh
+dq_validate_conf(url_conf=url_conf)
+```
+
+
+## Extract Params
+```sh
 dq_extract_parameters(url_conf=url_conf)
+```
 
 
+## Json params
+```sh
 parameter_conf_list = [
  {      
-    "ARTIFACTORY_UNIQUE_CACHE": "https://globaldevtools.bbva.com",
+    "ARTIFACTORY_UNIQUE_CACHE": "http://artifactory-gdt.central-02.nextgen.igrupobbva",
     "ODATE_DATE": "2022-11-11",
     "COUNTRY_ID": "PE",
     "SCHEMA_PATH": "t_kcog_branch.output.schema",
     "CUTOFF_DATE": "2022-11-11",
-    "SCHEMAS_REPOSITORY": "da-datio/schemas/pe/kcog/master/t_kcog_branch/latest/"
+    "SCHEMAS_REPOSITORY": "gl-datio-da-generic-local/schemas/pe/kcog/master/t_kcog_branch/latest/"
  }
 ]
-                  
-## quality run_sandbox
-dq_run_sandbox(parameter_conf_list=parameter_conf_list,
-               url_conf=url_conf))
-
 ```
 
-## Validations
 
+## Run 
 ```sh
-url_conf = "http://artifactory-gdt.central-02.nextgen.igrupobbva/artifactory/gl-datio-spark-libs-maven-local/com/datiobd/cdd-hammurabi/4.0.9/DQ_LOCAL_CONFS/KCOG/KCOG_branch_MRField.conf"
+dq_run_sandbox(spark=spark,
+               sc=sc,
+               parameter_conf_list=parameter_conf_list,
+               url_conf=url_conf)
+```
 
-## validate conf
-dq_validate_conf(url_conf=url_conf)
+               
+```sh         
+df = spark.read.csv("file:/var/sds/homes/P030772/workspace/data_quality_rules/data_reports/KCOG/KCOG_BRANCH_MRFIELD_202304120046_20221111.csv", 
+                    header=True)                 
+df.show2(100)
+```
 
-## validate rules
-dq_validate_rules(url_conf=url_conf)
 
+## Run 
+```sh
+dq_validate_rules(url_conf=url_conf)
 ```
 
 
-
 ## License
 
 [Apache License 2.0](https://www.dropbox.com/s/8t6xtgk06o3ij61/LICENSE?dl=0).
 
 ## New features v1.0
 
 ## BugFix
```

### Comparing `spark_quality_rules_tools-0.2.5/setup.py` & `spark_quality_rules_tools-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.2.5',
+    version='0.2.6',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-from spark_quality_rules_tools.functions.generator import dq_creating_directory
+from spark_quality_rules_tools.functions.generator import dq_creating_directory_sandbox
 from spark_quality_rules_tools.functions.generator import dq_download_jar
 from spark_quality_rules_tools.functions.generator import dq_extract_parameters
 from spark_quality_rules_tools.functions.generator import dq_path_workspace
 from spark_quality_rules_tools.functions.generator import dq_run_sandbox
 from spark_quality_rules_tools.functions.generator import dq_spark_session
 from spark_quality_rules_tools.functions.generator import dq_validate_conf
 from spark_quality_rules_tools.functions.generator import dq_validate_rules
 from spark_quality_rules_tools.utils import BASE_DIR
 from spark_quality_rules_tools.utils.color import get_color
 from spark_quality_rules_tools.utils.color import get_color_b
-from spark_quality_rules_tools.utils.dataframe import show_pd_df
-from spark_quality_rules_tools.utils.dataframe import show_spark_df
 from spark_quality_rules_tools.utils.resolve import get_replace_resolve_parameter
 from spark_quality_rules_tools.utils.rules import get_validate_rules
 
-dataframe_all = ["show_pd_df", "show_spark_df"]
 generator_all = ["dq_creating_directory",
                  "dq_spark_session",
                  "dq_path_workspace",
                  "dq_download_jar",
                  "dq_validate_conf",
                  "dq_extract_parameters",
                  "dq_run_sandbox",
                  "dq_validate_rules", ]
 utils_all = ["BASE_DIR",
              "get_color",
              "get_color_b",
-             "show_pd_df",
-             "show_spark_df",
              "get_replace_resolve_parameter",
              "get_validate_rules"]
 
-__all__ = dataframe_all + generator_all + utils_all
+__all__ = generator_all + utils_all
```

### Comparing `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/functions/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,24 @@
-def dq_creating_directory(path=None):
-    import os
+def dq_creating_directory_hdfs(spark=None, path=None):
+    from spark_quality_rules_tools import get_color, get_color_b
+
+    sc = spark.sparkContext
+    fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
+    if path in ("", None):
+        raise Exception(f'required variable path')
+    if not fs.exists(sc._jvm.org.apache.hadoop.fs.Path(f'{path}')):
+        fs.mkdirs(sc._jvm.org.apache.hadoop.fs.Path(f'{path}'))
+        print(f"{get_color('Directory Created:')} {get_color_b(path)}")
+    else:
+        print(f"{get_color('Directory Exists:')} {get_color_b(path)}")
+
+
+def dq_creating_directory_sandbox(path=None):
     from spark_quality_rules_tools import get_color, get_color_b
+    import os
 
     if path in ("", None):
         raise Exception(f'required variable path')
     if not os.path.exists(f'{path}'):
         os.makedirs(f'{path}')
         print(f"{get_color('Directory Created:')} {get_color_b(path)}")
     else:
@@ -46,15 +60,16 @@
     sc._conf.setExecutorEnv("SANDBOX_DQ_METRICS", os.getenv("SANDBOX_DQ_METRICS"))
     sc._conf.setExecutorEnv("SANDBOX_DQ_REFUSALS", os.getenv("SANDBOX_DQ_REFUSALS"))
 
     print(f"{get_color('Created Session Spark for user:')} {get_color_b(user_sandbox)}")
     return spark, sc
 
 
-def dq_path_workspace(user_sandbox=None,
+def dq_path_workspace(spark=None,
+                      user_sandbox=None,
                       uuaa_code='fina',
                       project_sda='CDD'):
     import os
     import sys
 
     if user_sandbox is None:
         user_sandbox = os.getenv('JPY_USER')
@@ -83,21 +98,23 @@
         pj_dq_dir_artifacts_scala = pj_dq_dir_artifacts_scala.replace("\\", "/")
         pj_dq_dir_name = pj_dq_dir_name.replace("\\", "/")
         pj_dq_dir_confs_name = pj_dq_dir_confs_name.replace("\\", "/")
         pj_dq_dir_hocons_name = pj_dq_dir_hocons_name.replace("\\", "/")
         pj_dq_dir_reports_name = pj_dq_dir_reports_name.replace("\\", "/")
         pj_dq_dir_resolve_name = pj_dq_dir_resolve_name.replace("\\", "/")
 
-    dq_creating_directory(path=pj_dq_dir_name)
-    dq_creating_directory(path=pj_dq_dir_artifacts_python)
-    dq_creating_directory(path=pj_dq_dir_artifacts_scala)
-    dq_creating_directory(path=pj_dq_dir_confs_name)
-    dq_creating_directory(path=pj_dq_dir_hocons_name)
-    dq_creating_directory(path=pj_dq_dir_reports_name)
-    dq_creating_directory(path=pj_dq_dir_resolve_name)
+    dq_creating_directory_sandbox(path=pj_dq_dir_name)
+    dq_creating_directory_sandbox(path=pj_dq_dir_artifacts_python)
+    dq_creating_directory_sandbox(path=pj_dq_dir_artifacts_scala)
+    dq_creating_directory_sandbox(path=pj_dq_dir_confs_name)
+    dq_creating_directory_sandbox(path=pj_dq_dir_hocons_name)
+    dq_creating_directory_sandbox(path=pj_dq_dir_reports_name)
+    dq_creating_directory_sandbox(path=pj_dq_dir_resolve_name)
+    dq_creating_directory_hdfs(spark=spark, path=pj_dq_dir_sandbox_dq_metrics)
+    dq_creating_directory_hdfs(spark=spark, path=pj_dq_dir_sandbox_dq_refusals)
     os.environ['pj_dq_dir_name'] = pj_dq_dir_name
     os.environ['pj_dq_dir_artifacts_python'] = pj_dq_dir_artifacts_python
     os.environ['pj_dq_dir_artifacts_scala'] = pj_dq_dir_artifacts_scala
     os.environ['pj_dq_dir_confs_name'] = pj_dq_dir_confs_name
     os.environ['pj_dq_dir_hocons_name'] = pj_dq_dir_hocons_name
     os.environ['pj_dq_dir_reports_name'] = pj_dq_dir_reports_name
     os.environ['pj_dir_workspace'] = pj_dir_workspace
@@ -180,14 +197,16 @@
     if dir_confs_name is None:
         raise Exception(f'required environment: pj_dq_dir_confs_name')
 
     url = url_conf
     url_conf_extension = str(str(url).split("/")[-1]).replace("-", "_").upper().strip()
     url_conf_name = str(str(url_conf_extension).split(".")[0])
     uuaa_name = str(str(url).split("/")[-2]).upper()
+    if not len(uuaa_name) == 4:
+        uuaa_name = str(str(url).split("/")[-5]).upper()
 
     dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
     dir_confs_filename_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS-{url_conf_name}.json")
 
     if is_windows:
         dir_confs_filename = dir_confs_filename.replace("\\", "/")
         dir_confs_filename_parameters = dir_confs_filename_parameters.replace("\\", "/")
@@ -272,14 +291,16 @@
     if dir_sandbox_dq_metrics is None:
         raise Exception(f'required environment: pj_dq_dir_sandbox_dq_metrics')
 
     url = url_conf
     url_conf_extension = str(str(url).split("/")[-1]).replace("-", "_").upper().strip()
     url_conf_name = str(str(url_conf_extension).split(".")[0])
     uuaa_name = str(str(url).split("/")[-2]).upper()
+    if not len(uuaa_name) == 4:
+        uuaa_name = str(str(url).split("/")[-5]).upper()
 
     now = datetime.now()
     current_datetime = now.strftime("%Y-%m-%d %H:%M:%S")
     current_datetime_str = now.strftime("%Y%m%d%H%M")
 
     dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
     dir_confs_filename_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS-{url_conf_name}.json")
@@ -385,14 +406,16 @@
     is_windows = sys.platform.startswith('win')
     dir_hocons_name = os.getenv('pj_dq_dir_hocons_name')
 
     url = url_conf
     url_conf_extension = str(str(url).split("/")[-1]).replace("-", "_").upper().strip()
     url_conf_name = str(str(url_conf_extension).split(".")[0])
     uuaa_name = str(str(url).split("/")[-2]).upper()
+    if not len(uuaa_name) == 4:
+        uuaa_name = str(str(url).split("/")[-5]).upper()
 
     if url_conf in ("", None):
         raise Exception(f'required variable url_conf')
 
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}.conf")
     if is_windows:
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
```

### Comparing `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resource/resolve.conf` & `spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/resource/resolve.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.2.6/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.2.6/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 spark_quality_rules_tools/__init__.py
 spark_quality_rules_tools.egg-info/PKG-INFO
 spark_quality_rules_tools.egg-info/SOURCES.txt
 spark_quality_rules_tools.egg-info/dependency_links.txt
 spark_quality_rules_tools.egg-info/requires.txt
 spark_quality_rules_tools.egg-info/top_level.txt
 spark_quality_rules_tools/functions/__init__.py
 spark_quality_rules_tools/functions/generator.py
 spark_quality_rules_tools/utils/__init__.py
 spark_quality_rules_tools/utils/color.py
-spark_quality_rules_tools/utils/dataframe.py
-spark_quality_rules_tools/utils/memory.py
 spark_quality_rules_tools/utils/resolve.py
 spark_quality_rules_tools/utils/rules.py
-spark_quality_rules_tools/utils/external/folder_process.png
 spark_quality_rules_tools/utils/resource/resolve.conf
-spark_quality_rules_tools/utils/resource/rules.json
-spark_quality_rules_tools/utils/templates/__init__.py
-spark_quality_rules_tools/utils/templates/table.html
+spark_quality_rules_tools/utils/resource/rules.json
```

