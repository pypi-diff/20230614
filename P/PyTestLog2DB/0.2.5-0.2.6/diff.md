# Comparing `tmp/PyTestLog2DB-0.2.5.tar.gz` & `tmp/PyTestLog2DB-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTestLog2DB-0.2.5.tar", last modified: Thu May  4 13:03:47 2023, max compression
+gzip compressed data, was "PyTestLog2DB-0.2.6.tar", last modified: Wed Jun  7 13:56:27 2023, max compression
```

## Comparing `PyTestLog2DB-0.2.5.tar` & `PyTestLog2DB-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/PyTestLog2DB/
--rw-r--r--   0 runner    (1001) docker     (123)    42027 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/CDataBase.py
--rw-r--r--   0 runner    (1001) docker     (123)   532667 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/PyTestLog2DB.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43619 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/pytestlog2db.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/PyTestLog2DB/xsd/
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/PyTestLog2DB/xsd/junit.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 13:03:47.000000 PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:03:47.893103 PyTestLog2DB-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-04 13:01:15.000000 PyTestLog2DB-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:56:27.970648 PyTestLog2DB-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 13:54:16.000000 PyTestLog2DB-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-06-07 13:56:27.970648 PyTestLog2DB-0.2.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:56:27.970648 PyTestLog2DB-0.2.6/PyTestLog2DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    42027 2023-06-07 13:54:16.000000 PyTestLog2DB-0.2.6/PyTestLog2DB/CDataBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   533533 2023-06-07 13:56:27.000000 PyTestLog2DB-0.2.6/PyTestLog2DB/PyTestLog2DB.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-07 13:54:16.000000 PyTestLog2DB-0.2.6/PyTestLog2DB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-07 13:54:16.000000 PyTestLog2DB-0.2.6/PyTestLog2DB/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43619 2023-06-07 13:54:16.000000 PyTestLog2DB-0.2.6/PyTestLog2DB/pytestlog2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-07 13:54:16.000000 PyTestLog2DB-0.2.6/PyTestLog2DB/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:56:27.970648 PyTestLog2DB-0.2.6/PyTestLog2DB/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-07 13:54:16.000000 PyTestLog2DB-0.2.6/PyTestLog2DB/xsd/junit.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:56:27.970648 PyTestLog2DB-0.2.6/PyTestLog2DB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-06-07 13:56:27.000000 PyTestLog2DB-0.2.6/PyTestLog2DB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-07 13:56:27.000000 PyTestLog2DB-0.2.6/PyTestLog2DB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:56:27.000000 PyTestLog2DB-0.2.6/PyTestLog2DB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 13:56:27.000000 PyTestLog2DB-0.2.6/PyTestLog2DB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 13:56:27.000000 PyTestLog2DB-0.2.6/PyTestLog2DB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-06-07 13:54:16.000000 PyTestLog2DB-0.2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:56:27.970648 PyTestLog2DB-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-07 13:54:16.000000 PyTestLog2DB-0.2.6/setup.py
```

### Comparing `PyTestLog2DB-0.2.5/LICENSE` & `PyTestLog2DB-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.5/PKG-INFO` & `PyTestLog2DB-0.2.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTestLog2DB
-Version: 0.2.5
+Version: 0.2.6
 Summary: Imports pytest result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/python-pytestlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -34,55 +34,101 @@
     -   [Maintainers](#maintainers)
     -   [Contributors](#contributors)
     -   [License](#license)
 
 Getting Started
 ---------------
 
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-is the tool that helps to import [PyTest](https://docs.pytest.org)
-results file(s) (as [JUnit XML](https://llg.cubic.org/docs/junit)
-format) to
-[TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)
-Dashboard.
+**PyTestLog2DB** is a command-line tool that enables you to import
+[pytest](https://docs.pytest.org) XML result files into
+[TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)\'s
+database for presenting an overview about the whole test execution and
+detail of each test result.
 
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-tool is operating system independent and only works with Python 3.
+**PyTestLog2DB** tool is operating system independent and only works
+with Python 3.
 
 ### How to install
 
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-is not available on [PyPI](https://pypi.org/) now.
+**PyTestLog2DB** can be installed in two different ways.
+
+1.  Installation via PyPi (recommended for users)
+
+    ``` {.}
+    pip install PyTestLog2DB
+    ```
+
+    [PyTestLog2DB in PyPi](https://pypi.org/project/PyTestLog2DB/)
+
+2.  Installation via GitHub (recommended for developers)
+
+    -   Clone the **python-pytestlog2db** repository to your machine.
+
+        ``` {.}
+        git clone https://github.com/test-fullautomation/python-pytestlog2db.git
+        ```
+
+        [PyTestLog2DB in
+        GitHub](https://github.com/test-fullautomation/python-pytestlog2db)
+
+    -   Install dependencies
+
+        **PyTestLog2DB** requires some additional Python libraries.
+        Before you install the cloned repository sources you have to
+        install the dependencies manually. The names of all related
+        packages you can find in the file `requirements.txt` in the
+        repository root folder. Use pip to install them:
+
+        ``` {.}
+        pip install -r ./requirements.txt
+        ```
+
+        Additionally install **LaTeX** (recommended: TeX Live). This is
+        used to render the documentation.
+
+    -   Configure dependencies
+
+        The installation of **PyTestLog2DB** includes to generate the
+        documentation in PDF format. This is done by an application
+        called **GenPackageDoc**, that is part of the installation
+        dependencies (see `requirements.txt`).
+
+        **GenPackageDoc** uses **LaTeX** to generate the documentation
+        in PDF format. Therefore **GenPackageDoc** needs to know where
+        to find **LaTeX**. This is defined in the **GenPackageDoc**
+        configuration file
+
+        ``` {.}
+        packagedoc\packagedoc_config.json
+        ```
 
-But you can install this package directly from Github repository as
-below:
+        Before you start the installation you have to introduce the
+        following environment variable, that is used in
+        `packagedoc_config.json`:
 
-    pip install git+https://github.com/test-fullautomation/python-pytestlog2db.git
+        -   `GENDOC_LATEXPATH` : path to `pdflatex` executable
 
-Or you can clone sourcecode to your local directory then install this
-package with below steps:
+    -   Use the following command to install **PyTestLog2DB**:
 
-    git clone https://github.com/test-fullautomation/python-pytestlog2db.git
-    cd python-pytestlog2db
-    python setup.py install
+        ``` {.}
+        python setup.py install
+        ```
 
 After succesful installation, the executable file **PyTestLog2DB** will
 be available (under *Scripts* folder of Python on Windows and
 *\~/.local/bin/* folder on Linux).
 
 In case above location is added to **PATH** environment variable then
 you can run it directly as operation system\'s command.
 
 Usage
 -----
 
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-requires the [PyTest](https://docs.pytest.org) result file(s) which
-contains the test result in [JUnit
-XML](https://llg.cubic.org/docs/junit) format and
+**PyTestLog2DB** requires the [pytest](https://docs.pytest.org) result
+file(s) which contains the test result in *JUnit XML* format and
 [TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)\'s
 database information for importing.
 
 Use below command to get tools\'s usage
 
     PyTestLog2DB -h
 
@@ -98,47 +144,47 @@
     server               server which hosts the database (IP or URL).
     user                 user for database login.
     password             password for database login.
     database             database schema for database login.
 
     optional arguments:
     -h, --help           show this help message and exit
-    -v                   Version of the PyTestLog2DB importer.
+    -v, --version        version of the PyTestLog2DB importer.
     --recursive          if set, then the path is searched recursively for output files to be imported.
     --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
-    --append             is used in combination with --UUID <UUID>. If set, allow to append new result(s) to existing execution result UUID in -UUID argument.
+    --append             is used in combination with --UUID <UUID>. If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
     --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided PyTestLog2DB will generate an UUID for the whole import.
     --variant VARIANT    variant name to be set for this import.
     --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
     --config CONFIG      configuration json file for component mapping information.
 
 The below command is simple usage with all required arguments to import
-[PyTest](https://docs.pytest.org) results into TestResultWebApp\'s
+[pytest](https://docs.pytest.org) results into TestResultWebApp\'s
 database:
 
     PyTestLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Besides the executable file, you can also run tool as a Python module
 
     python -m PyTestLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Example
 -------
 
 In order the import the robot result(s) to TestResultWebApp\'s database,
-we need the [PyTest](https://docs.pytest.org) result file in [JUnit
-XML](https://llg.cubic.org/docs/junit) format.
+we need the [pytest](https://docs.pytest.org) result file in *JUnit XML*
+format.
 
-So, firstly execute the [PyTest](https://docs.pytest.org) testcase(s) to
+So, firstly execute the [pytest](https://docs.pytest.org) testcase(s) to
 get the result file(s). But the **\*.xml** result file is not generated
 by default.
 
 We need to specify the argument *\--junit-xml=\<path\>* when executing
-[PyTest](https://docs.pytest.org) to get the generated [JUnit
-XML](https://llg.cubic.org/docs/junit) report file at given path.
+[pytest](https://docs.pytest.org) to get the generated *JUnit XML*
+report file at given path.
 
 E.g: :
 
     pytest --junit-xml=path/to/result.xml pytest/folder
 
 After that, the **\*.xml** result file will be available at
 **path/to/result.xml** and can be used for importing to
@@ -148,31 +194,30 @@
     PyTestLog2DB path/to/result.xml localhost test_user test_pw test_db
 
 Then, open TestResultWebApp with your favourite browser and you will see
 how wonderful the execution result is displayed as below figures:
 
 Dashboard view:
 
-![Dashboard view](packagedoc/additional_docs/pictures/Dashboard.png)
+![Dashboard view](https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/packagedoc/additional_docs/pictures/Dashboard.png?raw=true)
 
 Datatable view:
 
-![Datatable view](packagedoc/additional_docs/pictures/Datatable.png)
+![Datatable view](https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/packagedoc/additional_docs/pictures/Datatable.png?raw=true)
 
 ### Notes:
 
-> The **\*.xml** report file generated by PyTest contains only the
+> The **\*.xml** report file generated by pytest contains only the
 > testcase result(s) and less metadata information about the test
 > execution such as *project/variant*, *software version*, *tester* ,
 > *component*, \... which are required by
 > [TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp).
 >
-> So that,
-> [PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-> will handle those information with the default values.
+> So that, **PyTestLog2DB** will handle those information with the
+> default values.
 >
 > But you can use the optional argument *\--config CONFIG* to specify
 > those information when importing to
 > [TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)\'s
 > database.
 >
 > Sample configuration file:
@@ -195,23 +240,21 @@
 > Documentation](https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/PyTestLog2DB/PyTestLog2DB.pdf)
 > for more detail about default values and the configuration json file.
 
 Contribution
 ------------
 
 We are always searching support and you are cordially invited to help to
-improve
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-tool.
+improve **PyTestLog2DB** tool.
 
 Sourcecode Documentation
 ------------------------
 
 To understand more detail about the tool\'s features, parameters and how
-PyTest result(s) will be displayed on TestResultWebApp, please refer to
+pytest result(s) will be displayed on TestResultWebApp, please refer to
 [PyTestLog2DB tool's
 Documentation](https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/PyTestLog2DB/PyTestLog2DB.pdf).
 
 Feedback
 --------
 
 Please feel free to give any feedback to us via
```

### Comparing `PyTestLog2DB-0.2.5/PyTestLog2DB/CDataBase.py` & `PyTestLog2DB-0.2.6/PyTestLog2DB/CDataBase.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.5/PyTestLog2DB/PyTestLog2DB.pdf` & `PyTestLog2DB-0.2.6/PyTestLog2DB/PyTestLog2DB.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 PyTestLog2DB
-v. 0.2.5
+v. 0.2.6
 Tran Duy Ngoan
-04.05.2023
+08.05.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -1850,19 +1850,19 @@
 
 Name
 
 PyTestLog2DB
 
 Version
 
-0.2.5
+0.2.6
 
 Date
 
-04.05.2023
+08.05.2023
 
 Description
 
 Imports pytest result(s) to TestResultWebApp database
 
 Package URL
 
@@ -1958,15 +1958,20 @@
 Support 4 byte characters for importing to db
 0.1.9
 
 20.04.2023
 
 - Enhance console log with test case counter and component statistics
 - Add try/except for database access
+0.2.6
+
+08.05.2023
+
+Update README for publishing package to PyPI
 
 PyTestLog2DB.pdf
-Created at 04.05.2023 - 13:03:43
-by GenPackageDoc v. 0.39.2
+Created at 07.06.2023 - 13:56:23
+by GenPackageDoc v. 0.39.3
 
 29
```

### Comparing `PyTestLog2DB-0.2.5/PyTestLog2DB/__init__.py` & `PyTestLog2DB-0.2.6/PyTestLog2DB/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.5/PyTestLog2DB/__main__.py` & `PyTestLog2DB-0.2.6/PyTestLog2DB/__main__.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.5/PyTestLog2DB/pytestlog2db.py` & `PyTestLog2DB-0.2.6/PyTestLog2DB/pytestlog2db.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.5/PyTestLog2DB/version.py` & `PyTestLog2DB-0.2.6/PyTestLog2DB/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of PyTestLog2DB
 #
-VERSION      = "0.2.5"
-VERSION_DATE = "04.05.2023"
+VERSION      = "0.2.6"
+VERSION_DATE = "08.05.2023"
```

### Comparing `PyTestLog2DB-0.2.5/PyTestLog2DB/xsd/junit.xsd` & `PyTestLog2DB-0.2.6/PyTestLog2DB/xsd/junit.xsd`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.5/PyTestLog2DB.egg-info/PKG-INFO` & `PyTestLog2DB-0.2.6/PyTestLog2DB.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTestLog2DB
-Version: 0.2.5
+Version: 0.2.6
 Summary: Imports pytest result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/python-pytestlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -34,55 +34,101 @@
     -   [Maintainers](#maintainers)
     -   [Contributors](#contributors)
     -   [License](#license)
 
 Getting Started
 ---------------
 
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-is the tool that helps to import [PyTest](https://docs.pytest.org)
-results file(s) (as [JUnit XML](https://llg.cubic.org/docs/junit)
-format) to
-[TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)
-Dashboard.
+**PyTestLog2DB** is a command-line tool that enables you to import
+[pytest](https://docs.pytest.org) XML result files into
+[TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)\'s
+database for presenting an overview about the whole test execution and
+detail of each test result.
 
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-tool is operating system independent and only works with Python 3.
+**PyTestLog2DB** tool is operating system independent and only works
+with Python 3.
 
 ### How to install
 
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-is not available on [PyPI](https://pypi.org/) now.
+**PyTestLog2DB** can be installed in two different ways.
+
+1.  Installation via PyPi (recommended for users)
+
+    ``` {.}
+    pip install PyTestLog2DB
+    ```
+
+    [PyTestLog2DB in PyPi](https://pypi.org/project/PyTestLog2DB/)
+
+2.  Installation via GitHub (recommended for developers)
+
+    -   Clone the **python-pytestlog2db** repository to your machine.
+
+        ``` {.}
+        git clone https://github.com/test-fullautomation/python-pytestlog2db.git
+        ```
+
+        [PyTestLog2DB in
+        GitHub](https://github.com/test-fullautomation/python-pytestlog2db)
+
+    -   Install dependencies
+
+        **PyTestLog2DB** requires some additional Python libraries.
+        Before you install the cloned repository sources you have to
+        install the dependencies manually. The names of all related
+        packages you can find in the file `requirements.txt` in the
+        repository root folder. Use pip to install them:
+
+        ``` {.}
+        pip install -r ./requirements.txt
+        ```
+
+        Additionally install **LaTeX** (recommended: TeX Live). This is
+        used to render the documentation.
+
+    -   Configure dependencies
+
+        The installation of **PyTestLog2DB** includes to generate the
+        documentation in PDF format. This is done by an application
+        called **GenPackageDoc**, that is part of the installation
+        dependencies (see `requirements.txt`).
+
+        **GenPackageDoc** uses **LaTeX** to generate the documentation
+        in PDF format. Therefore **GenPackageDoc** needs to know where
+        to find **LaTeX**. This is defined in the **GenPackageDoc**
+        configuration file
+
+        ``` {.}
+        packagedoc\packagedoc_config.json
+        ```
 
-But you can install this package directly from Github repository as
-below:
+        Before you start the installation you have to introduce the
+        following environment variable, that is used in
+        `packagedoc_config.json`:
 
-    pip install git+https://github.com/test-fullautomation/python-pytestlog2db.git
+        -   `GENDOC_LATEXPATH` : path to `pdflatex` executable
 
-Or you can clone sourcecode to your local directory then install this
-package with below steps:
+    -   Use the following command to install **PyTestLog2DB**:
 
-    git clone https://github.com/test-fullautomation/python-pytestlog2db.git
-    cd python-pytestlog2db
-    python setup.py install
+        ``` {.}
+        python setup.py install
+        ```
 
 After succesful installation, the executable file **PyTestLog2DB** will
 be available (under *Scripts* folder of Python on Windows and
 *\~/.local/bin/* folder on Linux).
 
 In case above location is added to **PATH** environment variable then
 you can run it directly as operation system\'s command.
 
 Usage
 -----
 
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-requires the [PyTest](https://docs.pytest.org) result file(s) which
-contains the test result in [JUnit
-XML](https://llg.cubic.org/docs/junit) format and
+**PyTestLog2DB** requires the [pytest](https://docs.pytest.org) result
+file(s) which contains the test result in *JUnit XML* format and
 [TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)\'s
 database information for importing.
 
 Use below command to get tools\'s usage
 
     PyTestLog2DB -h
 
@@ -98,47 +144,47 @@
     server               server which hosts the database (IP or URL).
     user                 user for database login.
     password             password for database login.
     database             database schema for database login.
 
     optional arguments:
     -h, --help           show this help message and exit
-    -v                   Version of the PyTestLog2DB importer.
+    -v, --version        version of the PyTestLog2DB importer.
     --recursive          if set, then the path is searched recursively for output files to be imported.
     --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
-    --append             is used in combination with --UUID <UUID>. If set, allow to append new result(s) to existing execution result UUID in -UUID argument.
+    --append             is used in combination with --UUID <UUID>. If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
     --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided PyTestLog2DB will generate an UUID for the whole import.
     --variant VARIANT    variant name to be set for this import.
     --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
     --config CONFIG      configuration json file for component mapping information.
 
 The below command is simple usage with all required arguments to import
-[PyTest](https://docs.pytest.org) results into TestResultWebApp\'s
+[pytest](https://docs.pytest.org) results into TestResultWebApp\'s
 database:
 
     PyTestLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Besides the executable file, you can also run tool as a Python module
 
     python -m PyTestLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Example
 -------
 
 In order the import the robot result(s) to TestResultWebApp\'s database,
-we need the [PyTest](https://docs.pytest.org) result file in [JUnit
-XML](https://llg.cubic.org/docs/junit) format.
+we need the [pytest](https://docs.pytest.org) result file in *JUnit XML*
+format.
 
-So, firstly execute the [PyTest](https://docs.pytest.org) testcase(s) to
+So, firstly execute the [pytest](https://docs.pytest.org) testcase(s) to
 get the result file(s). But the **\*.xml** result file is not generated
 by default.
 
 We need to specify the argument *\--junit-xml=\<path\>* when executing
-[PyTest](https://docs.pytest.org) to get the generated [JUnit
-XML](https://llg.cubic.org/docs/junit) report file at given path.
+[pytest](https://docs.pytest.org) to get the generated *JUnit XML*
+report file at given path.
 
 E.g: :
 
     pytest --junit-xml=path/to/result.xml pytest/folder
 
 After that, the **\*.xml** result file will be available at
 **path/to/result.xml** and can be used for importing to
@@ -148,31 +194,30 @@
     PyTestLog2DB path/to/result.xml localhost test_user test_pw test_db
 
 Then, open TestResultWebApp with your favourite browser and you will see
 how wonderful the execution result is displayed as below figures:
 
 Dashboard view:
 
-![Dashboard view](packagedoc/additional_docs/pictures/Dashboard.png)
+![Dashboard view](https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/packagedoc/additional_docs/pictures/Dashboard.png?raw=true)
 
 Datatable view:
 
-![Datatable view](packagedoc/additional_docs/pictures/Datatable.png)
+![Datatable view](https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/packagedoc/additional_docs/pictures/Datatable.png?raw=true)
 
 ### Notes:
 
-> The **\*.xml** report file generated by PyTest contains only the
+> The **\*.xml** report file generated by pytest contains only the
 > testcase result(s) and less metadata information about the test
 > execution such as *project/variant*, *software version*, *tester* ,
 > *component*, \... which are required by
 > [TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp).
 >
-> So that,
-> [PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-> will handle those information with the default values.
+> So that, **PyTestLog2DB** will handle those information with the
+> default values.
 >
 > But you can use the optional argument *\--config CONFIG* to specify
 > those information when importing to
 > [TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)\'s
 > database.
 >
 > Sample configuration file:
@@ -195,23 +240,21 @@
 > Documentation](https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/PyTestLog2DB/PyTestLog2DB.pdf)
 > for more detail about default values and the configuration json file.
 
 Contribution
 ------------
 
 We are always searching support and you are cordially invited to help to
-improve
-[PyTestLog2DB](https://github.com/test-fullautomation/python-pytestlog2db)
-tool.
+improve **PyTestLog2DB** tool.
 
 Sourcecode Documentation
 ------------------------
 
 To understand more detail about the tool\'s features, parameters and how
-PyTest result(s) will be displayed on TestResultWebApp, please refer to
+pytest result(s) will be displayed on TestResultWebApp, please refer to
 [PyTestLog2DB tool's
 Documentation](https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/PyTestLog2DB/PyTestLog2DB.pdf).
 
 Feedback
 --------
 
 Please feel free to give any feedback to us via
```

### Comparing `PyTestLog2DB-0.2.5/README.rst` & `PyTestLog2DB-0.2.6/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -17,52 +17,91 @@
    -  `Maintainers <#maintainers>`__
    -  `Contributors <#contributors>`__
    -  `License <#license>`__
    
 Getting Started
 ---------------
 
-PyTestLog2DB_ is the tool that helps to import PyTest_ results file(s)
-(as `JUnit XML`_ format) to TestResultWebApp_ Dashboard.
+**PyTestLog2DB** is a command-line tool that enables you to import pytest_ XML 
+result files into TestResultWebApp_'s database for presenting an overview about 
+the whole test execution and detail of each test result.
 
-PyTestLog2DB_ tool is operating system independent and only works with 
+**PyTestLog2DB** tool is operating system independent and only works with 
 Python 3.
 
 How to install
 ~~~~~~~~~~~~~~
 
-PyTestLog2DB_ is not available on PyPI_ now.
+**PyTestLog2DB** can be installed in two different ways.
 
-But you can install this package directly from Github repository as below:
+1. Installation via PyPi (recommended for users)
 
-::
+   .. code::
 
-   pip install git+https://github.com/test-fullautomation/python-pytestlog2db.git
+      pip install PyTestLog2DB
 
-Or you can clone sourcecode to your local directory then install this package 
-with below steps:
+   `PyTestLog2DB in PyPi <https://pypi.org/project/PyTestLog2DB/>`_
 
-::
+2. Installation via GitHub (recommended for developers)
+
+   * Clone the **python-pytestlog2db** repository to your machine.
+
+     .. code::
+
+        git clone https://github.com/test-fullautomation/python-pytestlog2db.git
+
+     `PyTestLog2DB in GitHub <https://github.com/test-fullautomation/python-pytestlog2db>`_
+
+   * Install dependencies
+
+     **PyTestLog2DB** requires some additional Python libraries. Before you install the cloned repository sources
+     you have to install the dependencies manually. The names of all related packages you can find in the file ``requirements.txt``
+     in the repository root folder. Use pip to install them:
+
+     .. code::
+
+        pip install -r ./requirements.txt
+
+     Additionally install **LaTeX** (recommended: TeX Live). This is used to render the documentation.
+
+   * Configure dependencies
+
+     The installation of **PyTestLog2DB** includes to generate the documentation in PDF format. This is done by
+     an application called **GenPackageDoc**, that is part of the installation dependencies (see ``requirements.txt``).
+
+     **GenPackageDoc** uses **LaTeX** to generate the documentation in PDF format. Therefore **GenPackageDoc** needs to know where to find
+     **LaTeX**. This is defined in the **GenPackageDoc** configuration file
+
+     .. code::
+
+        packagedoc\packagedoc_config.json
+
+     Before you start the installation you have to introduce the following environment variable, that is used in ``packagedoc_config.json``:
+
+     - ``GENDOC_LATEXPATH`` : path to ``pdflatex`` executable
+
+   * Use the following command to install **PyTestLog2DB**:
+
+     .. code::
 
-   git clone https://github.com/test-fullautomation/python-pytestlog2db.git
-   cd python-pytestlog2db
-   python setup.py install
+        python setup.py install
 
-After succesful installation, the executable file **PyTestLog2DB** 
-will be available (under *Scripts* folder of Python on Windows 
-and *~/.local/bin/* folder on Linux).
+After succesful installation, the executable file **PyTestLog2DB** will be 
+available (under *Scripts* folder of Python on Windows and *~/.local/bin/* 
+folder on Linux).
 
-In case above location is added to **PATH** environment variable 
-then you can run it directly as operation system's command.
+In case above location is added to **PATH** environment variable then you can 
+run it directly as operation system's command.
 
 Usage
 -----
 
-PyTestLog2DB_ requires the PyTest_ result file(s) which contains the test
-result in `JUnit XML`_ format and TestResultWebApp_'s database information for importing.
+**PyTestLog2DB** requires the pytest_ result file(s) which contains the test
+result in *JUnit XML* format and TestResultWebApp_'s database information for 
+importing.
 
 Use below command to get tools's usage
 
 ::
 
    PyTestLog2DB -h
 
@@ -81,26 +120,26 @@
    server               server which hosts the database (IP or URL).
    user                 user for database login.
    password             password for database login.
    database             database schema for database login.
 
    optional arguments:
    -h, --help           show this help message and exit
-   -v                   Version of the PyTestLog2DB importer.
+   -v, --version        version of the PyTestLog2DB importer.
    --recursive          if set, then the path is searched recursively for output files to be imported.
    --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
-   --append             is used in combination with --UUID <UUID>. If set, allow to append new result(s) to existing execution result UUID in -UUID argument.
+   --append             is used in combination with --UUID <UUID>. If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
    --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided PyTestLog2DB will generate an UUID for the whole import.
    --variant VARIANT    variant name to be set for this import.
    --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
    --config CONFIG      configuration json file for component mapping information.
 
 
 The below command is simple usage with all required arguments to import 
-PyTest_ results into TestResultWebApp's database:
+pytest_ results into TestResultWebApp's database:
 
 ::
 
    PyTestLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Besides the executable file, you can also run tool as a Python module
 
@@ -108,21 +147,21 @@
 
    python -m PyTestLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Example
 -------
 
 In order the import the robot result(s) to TestResultWebApp's database, 
-we need the PyTest_ result file in `JUnit XML`_ format.
+we need the pytest_ result file in *JUnit XML* format.
 
-So, firstly execute the PyTest_ testcase(s) to get the result file(s). But the 
+So, firstly execute the pytest_ testcase(s) to get the result file(s). But the 
 ***.xml** result file is not generated by default.
 
-We need to specify the argument *--junit-xml=<path>* when executing PyTest_ 
-to get the generated `JUnit XML`_ report file at given path.
+We need to specify the argument *--junit-xml=<path>* when executing pytest_ 
+to get the generated *JUnit XML* report file at given path.
 
 E.g:
 ::
 
    pytest --junit-xml=path/to/result.xml pytest/folder
 
 After that, the ***.xml** result file will be available at **path/to/result.xml**
@@ -133,31 +172,31 @@
    PyTestLog2DB path/to/result.xml localhost test_user test_pw test_db
 
 Then, open TestResultWebApp with your favourite browser and you will see how 
 wonderful the execution result is displayed as below figures:
 
 Dashboard view:
 
-.. image:: packagedoc/additional_docs/pictures/Dashboard.png
+.. image:: https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/packagedoc/additional_docs/pictures/Dashboard.png?raw=true
    :alt: Dashboard view
 
 Datatable view:
 
-.. image:: packagedoc/additional_docs/pictures/Datatable.png
+.. image:: https://github.com/test-fullautomation/python-pytestlog2db/blob/develop/packagedoc/additional_docs/pictures/Datatable.png?raw=true
    :alt: Datatable view
 
 Notes:
 ~~~~~~
 
-   The ***.xml** report file generated by PyTest contains only the testcase 
+   The ***.xml** report file generated by pytest contains only the testcase 
    result(s) and less metadata information about the test execution such as 
    *project/variant*, *software version*, *tester* , *component*, ... 
    which are required by TestResultWebApp_.
 
-   So that, PyTestLog2DB_ will handle those information with the default values.
+   So that, **PyTestLog2DB** will handle those information with the default values.
 
    But you can use the optional argument *--config CONFIG* to specify those
    information when importing to TestResultWebApp_'s database.
 
    Sample configuration file:
 
    ::
@@ -178,19 +217,19 @@
 
    Please refer `PyTestLog2DB tool’s Documentation`_ for more detail about default
    values and the configuration json file.
 
 Contribution
 ------------
 We are always searching support and you are cordially invited to help to improve 
-PyTestLog2DB_ tool.
+**PyTestLog2DB** tool.
 
 Sourcecode Documentation
 ------------------------
-To understand more detail about the tool's features, parameters and how PyTest
+To understand more detail about the tool's features, parameters and how pytest
 result(s) will be displayed on TestResultWebApp, please refer to 
 `PyTestLog2DB tool’s Documentation`_.
 
 Feedback
 --------
 Please feel free to give any feedback to us via
 
@@ -234,15 +273,15 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 
 .. |License: Apache v2| image:: https://img.shields.io/pypi/l/robotframework.svg
    :target: http://www.apache.org/licenses/LICENSE-2.0.html
-.. _PyTest: https://docs.pytest.org
+.. _pytest: https://docs.pytest.org
 .. _JUnit XML: https://llg.cubic.org/docs/junit
 .. _PyTestLog2DB: https://github.com/test-fullautomation/python-pytestlog2db
 .. _TestResultWebApp: https://github.com/test-fullautomation/TestResultWebApp
 .. _PyPI: https://pypi.org/
 .. _Thomas Pollerspöck: mailto:Thomas.Pollerspoeck@de.bosch.com
 .. _Tran Duy Ngoan: mailto:Ngoan.TranDuy@vn.bosch.com
 .. _Nguyen Huynh Tri Cuong: mailto:Cuong.NguyenHuynhTri@vn.bosch.com
```

### Comparing `PyTestLog2DB-0.2.5/setup.py` & `PyTestLog2DB-0.2.6/setup.py`

 * *Files identical despite different names*

