# Comparing `tmp/cohort-generator-0.1.0.tar.gz` & `tmp/cohort-generator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohort-generator-0.1.0.tar", last modified: Tue Jun 13 14:53:57 2023, max compression
+gzip compressed data, was "cohort-generator-0.2.0.tar", last modified: Wed Jun 14 08:26:51 2023, max compression
```

## Comparing `cohort-generator-0.1.0.tar` & `cohort-generator-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:57.788293 cohort-generator-0.1.0/
--rw-rw-rw-   0        0        0      945 2023-06-13 14:53:57.786720 cohort-generator-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:57.773675 cohort-generator-0.1.0/cohort_generator.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-13 14:53:57.000000 cohort-generator-0.1.0/cohort_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-13 14:53:57.000000 cohort-generator-0.1.0/cohort_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:53:57.000000 cohort-generator-0.1.0/cohort_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-13 14:53:57.000000 cohort-generator-0.1.0/cohort_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 14:53:57.000000 cohort-generator-0.1.0/cohort_generator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:57.743814 cohort-generator-0.1.0/ohdsi/
-drwxrwxrwx   0        0        0        0 2023-06-13 14:53:57.782763 cohort-generator-0.1.0/ohdsi/cohort_generator/
--rw-rw-rw-   0        0        0     2878 2023-06-13 14:11:14.000000 cohort-generator-0.1.0/ohdsi/cohort_generator/__init__.py
--rw-rw-rw-   0        0        0     1758 2023-06-13 12:57:07.000000 cohort-generator-0.1.0/ohdsi/cohort_generator/main.py
--rw-rw-rw-   0        0        0       42 2023-06-13 14:53:57.788315 cohort-generator-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1092 2023-06-13 13:18:04.000000 cohort-generator-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/cohort_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 08:26:51.000000 cohort-generator-0.2.0/cohort_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/ohdsi/cohort_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-14 08:26:29.000000 cohort-generator-0.2.0/ohdsi/cohort_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-14 08:26:29.000000 cohort-generator-0.2.0/ohdsi/cohort_generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:26:51.073502 cohort-generator-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-14 08:26:29.000000 cohort-generator-0.2.0/setup.py
```

### Comparing `cohort-generator-0.1.0/PKG-INFO` & `cohort-generator-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: cohort-generator
-Version: 0.1.0
-Summary: Python wrapper for the OHDSI R packages
-Home-page: https://github.com/vantage6/python-ohdsi
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-# python-ohdsi
-Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
-OMOP data sources in vantage6.
-
-# TODO
-Packages to be wrapped:
-- [ ] [Capr](https://github.com/OHDSI/Capr)
-- [X] [CirceR](https://github.com/OHDSI/CirceR)
-- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
-- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
-- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
-- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
-
-Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
+Metadata-Version: 2.1
+Name: cohort-generator
+Version: 0.2.0
+Summary: Python wrapper for the OHDSI R packages
+Home-page: https://github.com/vantage6/python-ohdsi
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
+# python-ohdsi
+Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
+OMOP data sources in vantage6.
+
+# TODO
+Packages to be wrapped:
+- [ ] [Capr](https://github.com/OHDSI/Capr)
+- [X] [CirceR](https://github.com/OHDSI/CirceR)
+- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
+- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
+- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
+- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
+
+Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
```

### Comparing `cohort-generator-0.1.0/cohort_generator.egg-info/PKG-INFO` & `cohort-generator-0.2.0/cohort_generator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1
-Name: cohort-generator
-Version: 0.1.0
-Summary: Python wrapper for the OHDSI R packages
-Home-page: https://github.com/vantage6/python-ohdsi
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-# python-ohdsi
-Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
-OMOP data sources in vantage6.
-
-# TODO
-Packages to be wrapped:
-- [ ] [Capr](https://github.com/OHDSI/Capr)
-- [X] [CirceR](https://github.com/OHDSI/CirceR)
-- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
-- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
-- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
-- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
-
-Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
+Metadata-Version: 2.1
+Name: cohort-generator
+Version: 0.2.0
+Summary: Python wrapper for the OHDSI R packages
+Home-page: https://github.com/vantage6/python-ohdsi
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
+# python-ohdsi
+Python wrappers for (some) OHDSI tools. This project has been initiated for supporting
+OMOP data sources in vantage6.
+
+# TODO
+Packages to be wrapped:
+- [ ] [Capr](https://github.com/OHDSI/Capr)
+- [X] [CirceR](https://github.com/OHDSI/CirceR)
+- [X] [CohortGenerator](https://github.com/OHDSI/cohortgenerator)
+- [X] [SqlRender](https://github.com/OHDSI/SqlRender)
+- [X] [DatabaseConnector](https://github.com/OHDSI/DatabaseConnector)
+- [ ] [FeatureExtraction](https://github.com/OHDSI/FeatureExtraction)
+
+Release packages: `ohdsi-circe`, `ohdsi-capr`, `ohdsi-cohortgenerator`, `ohdsi-sqlrender`, `ohdsi-databaseconnector`, `ohdsi-featureextraction`
```

### Comparing `cohort-generator-0.1.0/ohdsi/cohort_generator/__init__.py` & `cohort-generator-0.2.0/ohdsi/cohort_generator/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from rpy2.robjects.methods import RS4
-from rpy2.robjects.vectors import ListVector, StrSexpVector
-from rpy2.robjects.packages import importr
-
-cohort_generator = importr('CohortGenerator')
-
-
-class CohortTables:
-
-    @staticmethod
-    def get_cohort_table_names(
-        cohort_table: str = "cohort",
-        cohort_inclusion_table: str | None = None,
-        cohort_inclusion_result_table: str | None = None,
-        cohort_inclusion_stats_table: str | None = None,
-        cohort_summary_stats_table: str | None = None,
-        cohort_censor_stats_table: str | None = None
-    ) -> ListVector:
-        """
-        Get the names of the cohort tables.
-        """
-        args = {
-            "cohortTable": cohort_table,
-            "cohortInclusionTable": cohort_inclusion_table,
-            "cohortInclusionResultTable": cohort_inclusion_result_table,
-            "cohortInclusionStatsTable": cohort_inclusion_stats_table,
-            "cohortSummaryStatsTable": cohort_summary_stats_table,
-            "cohortCensorStatsTable": cohort_censor_stats_table
-        }
-        # remove None values
-        args = {k: v for k, v in args.items() if v is not None}
-        return cohort_generator.getCohortTableNames(**args)
-
-    @staticmethod
-    def create_cohort_tables(
-        cohort_database_schema: str,
-        connection_details: ListVector | None = None,
-        connection: RS4 | None = None,
-        cohort_table_names: ListVector | None = None,
-        incremental: bool = False
-    ) -> RS4:
-        """
-        Create cohort tables.
-
-        Creates the cohort tables in the database.
-
-        Parameters
-        ----------
-        cohort_database_schema : str
-            The schema to create the cohort tables in
-        connection_details : ListVector, optional
-            The connection details, by default None
-        connection : RS4, optional
-            The connection, by default None
-        cohort_table_names : ListVector, optional
-            The names of the cohort tables, by default None
-        incremental : bool, optional
-            A boolean representing if the tables should be created
-            incrementally, by default False
-
-        Returns
-        -------
-        RS4
-            A wrapped cohort generation R object
-        """
-        if cohort_table_names is None:
-            cohort_table_names = CohortTables.get_cohort_table_names()
-
-        args = {
-            "cohortDatabaseSchema": cohort_database_schema,
-            "connectionDetails": connection_details,
-            "connection": connection,
-            "cohortTableNames": cohort_table_names,
-            "incremental": incremental
-        }
-        # remove None values
-        args = {k: v for k, v in args.items() if v is not None}
-        return cohort_generator.createCohortTables(**args)
+from rpy2.robjects.methods import RS4
+from rpy2.robjects.vectors import ListVector, StrSexpVector
+from rpy2.robjects.packages import importr
+
+cohort_generator = importr('CohortGenerator')
+
+
+class CohortTables:
+
+    @staticmethod
+    def get_cohort_table_names(
+        cohort_table: str = "cohort",
+        cohort_inclusion_table: str | None = None,
+        cohort_inclusion_result_table: str | None = None,
+        cohort_inclusion_stats_table: str | None = None,
+        cohort_summary_stats_table: str | None = None,
+        cohort_censor_stats_table: str | None = None
+    ) -> ListVector:
+        """
+        Get the names of the cohort tables.
+        """
+        args = {
+            "cohortTable": cohort_table,
+            "cohortInclusionTable": cohort_inclusion_table,
+            "cohortInclusionResultTable": cohort_inclusion_result_table,
+            "cohortInclusionStatsTable": cohort_inclusion_stats_table,
+            "cohortSummaryStatsTable": cohort_summary_stats_table,
+            "cohortCensorStatsTable": cohort_censor_stats_table
+        }
+        # remove None values
+        args = {k: v for k, v in args.items() if v is not None}
+        return cohort_generator.getCohortTableNames(**args)
+
+    @staticmethod
+    def create_cohort_tables(
+        cohort_database_schema: str,
+        connection_details: ListVector | None = None,
+        connection: RS4 | None = None,
+        cohort_table_names: ListVector | None = None,
+        incremental: bool = False
+    ) -> RS4:
+        """
+        Create cohort tables.
+
+        Creates the cohort tables in the database.
+
+        Parameters
+        ----------
+        cohort_database_schema : str
+            The schema to create the cohort tables in
+        connection_details : ListVector, optional
+            The connection details, by default None
+        connection : RS4, optional
+            The connection, by default None
+        cohort_table_names : ListVector, optional
+            The names of the cohort tables, by default None
+        incremental : bool, optional
+            A boolean representing if the tables should be created
+            incrementally, by default False
+
+        Returns
+        -------
+        RS4
+            A wrapped cohort generation R object
+        """
+        if cohort_table_names is None:
+            cohort_table_names = CohortTables.get_cohort_table_names()
+
+        args = {
+            "cohortDatabaseSchema": cohort_database_schema,
+            "connectionDetails": connection_details,
+            "connection": connection,
+            "cohortTableNames": cohort_table_names,
+            "incremental": incremental
+        }
+        # remove None values
+        args = {k: v for k, v in args.items() if v is not None}
+        return cohort_generator.createCohortTables(**args)
```

### Comparing `cohort-generator-0.1.0/ohdsi/cohort_generator/main.py` & `cohort-generator-0.2.0/ohdsi/cohort_generator/main.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from rpy2 import robjects
-from rpy2.robjects.packages import importr
-from importlib.resources import files
-
-from circe.cohort_expression import cohort_expression_from_json
-from circe.cohort_sql_builder import build_cohort_query
-
-
-cohort_json = files('circe.data').joinpath('simpleCohort.json').read_text()
-
-print("importing R cohort generator")
-ch = importr('CohortGenerator')
-
-cohort_to_create = ch.createEmptyCohortDefinitionSet()
-
-# circe
-cohort = cohort_expression_from_json(cohort_json)
-sql = build_cohort_query(cohort)
-##
-
-cohort_table_names = ch.getCohortTableNames(cohortTable = "my_cohort_table")
-
-print("importing R eunomia")
-eunomia = importr('Eunomia')
-eunomia.getEunomiaConnectionDetails()
-
-conectionDetails = eunomia.getEunomiaConnectionDetails()
-ch.createCohortTables(connectionDetails=conectionDetails, cohortDatabaseSchema = "main", cohortTableNames =cohort_table_names)
-
-
-
-
-rbase = importr('base')
-cohorts_to_create2 = rbase.rbind(
-    cohort_to_create,
-    robjects.r('data.frame')(cohortId=1, cohortName="SimpleCohort", sql=str(sql), stringAsFactors=False)
-)
-
-cohortGenerated = ch.generateCohortSet(
-    connectionDetails=conectionDetails,
-    cdmDatabaseSchema="main",
-    cohortDatabaseSchema="main",
-    cohortTableNames=cohort_table_names,
-    cohortDefinitionSet=cohorts_to_create2
-)
-
-
-counts = ch.getCohortCounts(
-    connectionDetails=conectionDetails,
-    cohortDatabaseSchema = "main",
-    cohortTable=cohort_table_names.rx2("cohortTable")
-)
-
-# from rpy2.robjects import pandas2ri
-# import rpy2.robjects as ro
-# import pandas as pd
-# with (ro.default_converter + pandas2ri.converter).context():
-#     pd_from_r_df = ro.conversion.get_conversion().rpy2py(cohortGenerated)
+from rpy2 import robjects
+from rpy2.robjects.packages import importr
+from importlib.resources import files
+
+from circe.cohort_expression import cohort_expression_from_json
+from circe.cohort_sql_builder import build_cohort_query
+
+
+cohort_json = files('circe.data').joinpath('simpleCohort.json').read_text()
+
+print("importing R cohort generator")
+ch = importr('CohortGenerator')
+
+cohort_to_create = ch.createEmptyCohortDefinitionSet()
+
+# circe
+cohort = cohort_expression_from_json(cohort_json)
+sql = build_cohort_query(cohort)
+##
+
+cohort_table_names = ch.getCohortTableNames(cohortTable = "my_cohort_table")
+
+print("importing R eunomia")
+eunomia = importr('Eunomia')
+eunomia.getEunomiaConnectionDetails()
+
+conectionDetails = eunomia.getEunomiaConnectionDetails()
+ch.createCohortTables(connectionDetails=conectionDetails, cohortDatabaseSchema = "main", cohortTableNames =cohort_table_names)
+
+
+
+
+rbase = importr('base')
+cohorts_to_create2 = rbase.rbind(
+    cohort_to_create,
+    robjects.r('data.frame')(cohortId=1, cohortName="SimpleCohort", sql=str(sql), stringAsFactors=False)
+)
+
+cohortGenerated = ch.generateCohortSet(
+    connectionDetails=conectionDetails,
+    cdmDatabaseSchema="main",
+    cohortDatabaseSchema="main",
+    cohortTableNames=cohort_table_names,
+    cohortDefinitionSet=cohorts_to_create2
+)
+
+
+counts = ch.getCohortCounts(
+    connectionDetails=conectionDetails,
+    cohortDatabaseSchema = "main",
+    cohortTable=cohort_table_names.rx2("cohortTable")
+)
+
+# from rpy2.robjects import pandas2ri
+# import rpy2.robjects as ro
+# import pandas as pd
+# with (ro.default_converter + pandas2ri.converter).context():
+#     pd_from_r_df = ro.conversion.get_conversion().rpy2py(cohortGenerated)
```

### Comparing `cohort-generator-0.1.0/setup.py` & `cohort-generator-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-import codecs
-
-from setuptools import setup, find_namespace_packages
-from pathlib import Path
-
-# get current directory
-here = Path(__file__).parent.absolute()
-parent_dir = here.parent.absolute()
-
-# get the long description from the README file
-with codecs.open(parent_dir / 'README.md', encoding='utf-8') as f:
-    long_description = f.read()
-
-# setup the package
-setup(
-    name='cohort-generator',
-    version='0.1.0',
-    description='Python wrapper for the OHDSI R packages',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/vantage6/python-ohdsi',
-    packages=find_namespace_packages(include=['ohdsi.*']),
-    python_requires='>=3.10',
-    install_requires=[
-        'rpy2==3.5.12',
-    ],
-    extras_require={
-        'dev': []
-    },
-    package_data={
-        'ohdsi.cohort_generator.data': [
-            'data/*'
-        ],
-    },
-    # entry_points={
-    #     'console_scripts': [
-    #         'vserver-local=vantage6.server.cli.server:cli_server'
-    #     ]
-    # }
-)
+import codecs
+
+from setuptools import setup, find_namespace_packages
+from pathlib import Path
+
+# get current directory
+here = Path(__file__).parent.absolute()
+parent_dir = here.parent.absolute()
+
+# get the long description from the README file
+with codecs.open(parent_dir / 'README.md', encoding='utf-8') as f:
+    long_description = f.read()
+
+# get the version from the parent dir
+with open(parent_dir / 'VERSION') as f:
+    version = f.read().strip()
+
+# setup the package
+setup(
+    name='cohort-generator',
+    version=version,
+    description='Python wrapper for the OHDSI R packages',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/vantage6/python-ohdsi',
+    packages=find_namespace_packages(include=['ohdsi.*']),
+    python_requires='>=3.10',
+    install_requires=[
+        'rpy2==3.5.12',
+    ],
+    extras_require={
+        'dev': []
+    },
+    package_data={
+        'ohdsi.cohort_generator.data': [
+            'data/*'
+        ],
+    },
+    # entry_points={
+    #     'console_scripts': [
+    #         'vserver-local=vantage6.server.cli.server:cli_server'
+    #     ]
+    # }
+)
```

