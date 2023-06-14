# Comparing `tmp/robotframework-robotlog2db-1.3.6.tar.gz` & `tmp/robotframework-robotlog2db-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robotlog2db-1.3.6.tar", last modified: Thu Jun  8 14:02:12 2023, max compression
+gzip compressed data, was "robotframework-robotlog2db-1.3.7.tar", last modified: Wed Jun 14 08:58:32 2023, max compression
```

## Comparing `robotframework-robotlog2db-1.3.6.tar` & `robotframework-robotlog2db-1.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:12.724728 robotframework-robotlog2db-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-06-08 14:02:12.724728 robotframework-robotlog2db-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-06-08 13:59:44.000000 robotframework-robotlog2db-1.3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:12.724728 robotframework-robotlog2db-1.3.6/RobotLog2DB/
--rw-r--r--   0 runner    (1001) docker     (123)    42027 2023-06-08 13:59:44.000000 robotframework-robotlog2db-1.3.6/RobotLog2DB/CDataBase.py
--rw-r--r--   0 runner    (1001) docker     (123)   595182 2023-06-08 14:02:12.000000 robotframework-robotlog2db-1.3.6/RobotLog2DB/RobotLog2DB.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 13:59:44.000000 robotframework-robotlog2db-1.3.6/RobotLog2DB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-08 13:59:44.000000 robotframework-robotlog2db-1.3.6/RobotLog2DB/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43119 2023-06-08 13:59:44.000000 robotframework-robotlog2db-1.3.6/RobotLog2DB/robotlog2db.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-08 13:59:44.000000 robotframework-robotlog2db-1.3.6/RobotLog2DB/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:12.724728 robotframework-robotlog2db-1.3.6/RobotLog2DB/xsd/
--rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-06-08 13:59:44.000000 robotframework-robotlog2db-1.3.6/RobotLog2DB/xsd/robot.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:12.724728 robotframework-robotlog2db-1.3.6/robotframework_robotlog2db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-06-08 14:02:12.000000 robotframework-robotlog2db-1.3.6/robotframework_robotlog2db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-08 14:02:12.000000 robotframework-robotlog2db-1.3.6/robotframework_robotlog2db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:02:12.000000 robotframework-robotlog2db-1.3.6/robotframework_robotlog2db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 14:02:12.000000 robotframework-robotlog2db-1.3.6/robotframework_robotlog2db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 14:02:12.000000 robotframework-robotlog2db-1.3.6/robotframework_robotlog2db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 14:02:12.000000 robotframework-robotlog2db-1.3.6/robotframework_robotlog2db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:02:12.724728 robotframework-robotlog2db-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-08 13:59:44.000000 robotframework-robotlog2db-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:32.617748 robotframework-robotlog2db-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-14 08:58:32.617748 robotframework-robotlog2db-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:32.613748 robotframework-robotlog2db-1.3.7/RobotLog2DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    42027 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/CDataBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   595626 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/RobotLog2DB.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43119 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/robotlog2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:32.613748 robotframework-robotlog2db-1.3.7/RobotLog2DB/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/xsd/robot.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:32.617748 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:58:32.617748 robotframework-robotlog2db-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/setup.py
```

### Comparing `robotframework-robotlog2db-1.3.6/PKG-INFO` & `robotframework-robotlog2db-1.3.7/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,266 +1,309 @@
-Metadata-Version: 2.1
-Name: robotframework-robotlog2db
-Version: 1.3.6
-Summary: Imports robot result(s) to TestResultWebApp database
-Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
-Author: Tran Duy Ngoan
-Author-email: Ngoan.TranDuy@vn.bosch.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-
 RobotLog2DB
 ===========
 
 Table of Contents
 -----------------
 
--   [Getting Started](#getting-started)
-    -   [How to install](#how-to-install)
--   [Usage](#usage)
--   [Example](#example)
--   [Contribution](#contribution)
--   [Sourcecode Documentation](#sourcecode-documentation)
--   [Feedback](#feedback)
--   [About](#about)
-    -   [Maintainers](#maintainers)
-    -   [Contributors](#contributors)
-    -   [License](#license)
+-  `Getting Started <#getting-started>`__
 
+   -  `How to install <#how-to-install>`__
+-  `Usage <#usage>`__
+-  `Example <#example>`__
+-  `Contribution <#contribution>`__
+-  `Sourcecode Documentation <#sourcecode-documentation>`__
+-  `Feedback <#feedback>`__
+-  `About <#about>`__
+
+   -  `Maintainers <#maintainers>`__
+   -  `Contributors <#contributors>`__
+   -  `License <#license>`__
+   
 Getting Started
 ---------------
 
-[RobotLog2DB](https://github.com/test-fullautomation/robotframework-robotlog2db)
-is the tool that helps to import Robot Framework results (**\*.xml**
-format) to
-[TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)
-Dashboard.
+**RobotLog2DB** is a command-line tool that enables you to import `Robot 
+Framework XML result`_ files into TestResultWebApp_'s database for 
+presenting an overview about the whole test execution and detail of each test 
+result.
+
+**RobotLog2DB** tool is operating system independent and only works with 
+Python 3.
+
+How to install
+~~~~~~~~~~~~~~
+
+**RobotLog2DB** can be installed in two different ways.
+
+1. Installation via PyPi (recommended for users)
+
+   .. code::
+
+      pip install robotframework-robotlog2db
+
+   `RobotLog2DB in PyPi <https://pypi.org/project/robotframework-robotlog2db/>`_
+
+2. Installation via GitHub (recommended for developers)
+
+   * Clone the **robotframework-robotlog2db** repository to your machine.
+
+     .. code::
+
+        git clone https://github.com/test-fullautomation/robotframework-robotlog2db.git
 
-[RobotLog2DB](https://github.com/test-fullautomation/robotframework-robotlog2db)
-tool is operating system independent and only works with Python 3.
+     `RobotLog2DB in GitHub <https://github.com/test-fullautomation/robotframework-robotlog2db>`_
 
-### How to install
+   * Install dependencies
 
-RobotLog2DB is not available on [PyPI](https://pypi.org/) now.
+     **RobotLog2DB** requires some additional Python libraries. Before you install the cloned repository sources
+     you have to install the dependencies manually. The names of all related packages you can find in the file ``requirements.txt``
+     in the repository root folder. Use pip to install them:
 
-But you can install this package directly from Github repository as
-below:
+     .. code::
 
-    pip install git+https://github.com/test-fullautomation/robotframework-robotlog2db.git
+        pip install -r ./requirements.txt
 
-Or you can clone sourcecode to your local directory then install this
-package with below steps:
+     Additionally install **LaTeX** (recommended: TeX Live). This is used to render the documentation.
 
-    git clone https://github.com/test-fullautomation/robotframework-robotlog2db.git
-    cd robotframework-robotlog2db
-    python setup.py install
+   * Configure dependencies
 
-After succesful installation, the executable file **RobotLog2DB** will
-be available (under *Scripts* folder of Python on Windows and
-*\~/.local/bin/* folder on Linux).
+     The installation of **RobotLog2DB** includes to generate the documentation in PDF format. This is done by
+     an application called **GenPackageDoc**, that is part of the installation dependencies (see ``requirements.txt``).
 
-In case above location is added to **PATH** environment variable then
-you can run it directly as operation system\'s command.
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
+   * Use the following command to install **RobotLog2DB**:
+
+     .. code::
+
+        python setup.py install
+
+After succesful installation, the executable file **RobotLog2DB** 
+will be available (under *Scripts* folder of Python on Windows 
+and *~/.local/bin/* folder on Linux).
+
+In case above location is added to **PATH** environment variable 
+then you can run it directly as operation system's command.
 
 Usage
 -----
 
-[RobotLog2DB](https://github.com/test-fullautomation/robotframework-robotlog2db)
-requires the Robot Framework result file(s) which contains the output
-result in XML format (default name is `output.xml`) and
-[TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)\'s
-database information for importing.
+**RobotLog2DB** requires the Robot Framework result file(s) which contains the 
+output result in XML format (default name is ``output.xml``) and 
+TestResultWebApp_'s database information for importing.
+
+Use below command to get tools's usage
+
+::
 
-Use below command to get tools\'s usage
+   RobotLog2DB -h
 
-    RobotLog2DB -h
 
 The usage should be showed as below:
 
-    usage: RobotLog2DB (RobotXMLResult to TestResultWebApp importer) [-h] [-v] [--recursive] [--dryrun] [--append] [--UUID UUID] [--variant VARIANT] [--versions VERSIONS] [--config CONFIG]
-                                                                     resultxmlfile server user password database
+::
 
-    RobotLog2DB imports XML result files (default: output.xml) generated by the Robot Framework into a WebApp database.
+   usage: RobotLog2DB (RobotXMLResult to TestResultWebApp importer) [-h] [-v] [--recursive] [--dryrun] [--append] [--UUID UUID] [--variant VARIANT] [--versions VERSIONS] [--config CONFIG]
+                                                                    resultxmlfile server user password database
 
-    positional arguments:
-    resultxmlfile        absolute or relative path to the result file or directory of result files to be imported.
-    server               server which hosts the database (IP or URL).
-    user                 user for database login.
-    password             password for database login.
-    database             database schema for database login.
-
-    optional arguments:
-    -h, --help           show this help message and exit
-    -v, --version        version of the RobotLog2DB importer.
-    --recursive          if set, then the path is searched recursively for output files to be imported.
-    --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
-    --append             is used in combination with --UUID <UUID>.If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
-    --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided RobotLog2DB will generate an UUID for the whole import.
-    --variant VARIANT    variant name to be set for this import.
-    --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
-    --config CONFIG      configuration json file for component mapping information.
+   RobotLog2DB imports XML result files (default: output.xml) generated by the Robot Framework into a WebApp database.
 
-The below command is simple usage with all required arguments to import
-robot results into TestResultWebApp\'s database:
+   positional arguments:
+   resultxmlfile        absolute or relative path to the result file or directory of result files to be imported.
+   server               server which hosts the database (IP or URL).
+   user                 user for database login.
+   password             password for database login.
+   database             database schema for database login.
+
+   optional arguments:
+   -h, --help           show this help message and exit
+   -v, --version        version of the RobotLog2DB importer.
+   --recursive          if set, then the path is searched recursively for output files to be imported.
+   --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
+   --append             is used in combination with --UUID <UUID>.If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
+   --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided RobotLog2DB will generate an UUID for the whole import.
+   --variant VARIANT    variant name to be set for this import.
+   --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
+   --config CONFIG      configuration json file for component mapping information.
 
-    RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
+
+The below command is simple usage with all required arguments to import 
+Robot Framework results into TestResultWebApp's database:
+
+::
+
+   RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Besides the executable file, you can also run tool as a Python module
 
-    python -m RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
+::
+
+   python -m RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
+
 
 Example
 -------
 
-In order the import the robot result(s) to TestResultWebApp\'s database,
-we need the Robot Framework result file (`output.xml`).
+In order the import the Robot Framework result(s) to TestResultWebApp's database, 
+we need the Robot Framework result file (``output.xml``).
+
+So, firstly execute the Robot Framework testcase(s) to get the Robot Framework result file.
+
+Sample Robot Framework testcase which contains neccessary information for importing into 
+TestResultWebApp's database:
+
+::
+
+   *** Settings ***
+   # Test execution level
+   Metadata   project        ROBFW              # Project/Variant
+   Metadata   version_sw     SW_VERSION_0.1     # Software version
+   Metadata   version_hw     HW_VERSION_0.1     # Hardware version
+   Metadata   version_test   TEST_VERSION_0.1   # Test version
+
+   # File/Suite level
+   Documentation             This is description for Robot Framework test file
+   Metadata    author        Tran Duy Ngoan (RBVH/ECM1)
+   Metadata    component     Import_Tools
+   Metadata    testtool      Robot Framework 3.2rc2 (Python 3.9.0 on win32)
+   Metadata    machine       %{COMPUTERNAME}
+   Metadata    tester        %{USER}
+
+   *** Test Cases ***
+   Testcase 01
+      [Tags]   ISSUE-001   TCID-1001   FID-112   FID-111
+      Log   	This is Testcase 01
+
+   Testcase 02
+      [Tags]   ISSUE-RTC-003   TCID-1002   FID-113
+      Log   	This is Testcase 01
 
-So, firstly execute the robot testcase(s) to get the Robot Framework
-result file.
 
-Sample robot testcase which contains neccessary information for
-importing into TestResultWebApp\'s database:
+Notes:
+~~~~~~
 
-    *** Settings ***
-    # Test execution level
-    Metadata   project        ROBFW              # Project/Variant
-    Metadata   version_sw     SW_VERSION_0.1     # Software version
-    Metadata   version_hw     HW_VERSION_0.1     # Hardware version
-    Metadata   version_test   TEST_VERSION_0.1   # Test version
-
-    # File/Suite level
-    Documentation             This is description for robot test file
-    Metadata    author        Tran Duy Ngoan (RBVH/ECM1)
-    Metadata    component     Import_Tools
-    Metadata    testtool      Robot Framework 3.2rc2 (Python 3.9.0 on win32)
-    Metadata    machine       %{COMPUTERNAME}
-    Metadata    tester        %{USER}
-
-    *** Test Cases ***
-    Testcase 01
-       [Tags]   ISSUE-001   TCID-1001   FID-112   FID-111
-       Log       This is Testcase 01
-
-    Testcase 02
-       [Tags]   ISSUE-RTC-003   TCID-1002   FID-113
-       Log       This is Testcase 01
-
-### Notes:
-
-> In case you are using RobotFramework AIO, these below `Metadata`
-> definitions will be handled implicitly by [RobotFramework Testsuites
-> Management](https://github.com/test-fullautomation/robotframework-testsuitesmanagement)
-> library within Suite Setup.
->
-> -   project
-> -   version\_sw
-> -   version\_hw
-> -   version\_test
-> -   machine
-> -   tester
-> -   testtool
->
-> So that you do not need to define them in your Robot testcase(s).
->
-> However, if these `Metadata` definitions are already missing in the
-> RobotFramework output result file, you can specific them when
-> executing the RobotLog2DB tool with the optional arguments:
->
-> -   `--variant VARIANT`: Project definitions
-> -   `--versions VERSIONS`: Versions (Software;Hardware;Test)
->     definitions.
-> -   `--config CONFIG`: Project, versions or component mapping
->     definitions.
->
-> Please refer to [RobotLog2DB tool's
-> Documentation](https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/RobotLog2DB/RobotLog2DB.pdf)
-> for more detail about these optional arguments.
-
-After getting Robot Framwork result file (`output.xml`), use below
-sample command to import that result into TestResultWebApp\'s database
-which is hosted at *localhost* as below sample command
+   In case you are using RobotFramework AIO, these below ``Metadata`` 
+   definitions will be handled implicitly by `RobotFramework Testsuites 
+   Management`_ library within Suite Setup. 
 
-    RobotLog2DB output.xml localhost test_user test_pw test_db
+   * project
+   * version_sw
+   * version_hw
+   * version_test
+   * machine
+   * tester
+   * testtool
 
-Then, open TestResultWebApp with your favourite browser and you will see
-how wonderful the execution result is displayed as below figures:
+   So that you do not need to define them in your Robot Framework testcase(s).
+
+   However, if these ``Metadata`` definitions are already missing in the 
+   Robot Framework output result file, you can specific them when executing the
+   **RobotLog2DB** tool with the optional arguments:
+
+   * ``--variant VARIANT``: Project definitions
+   * ``--versions VERSIONS``: Versions (Software;Hardware;Test) definitions.
+   * ``--config CONFIG``: Project, versions or component mapping definitions.
+
+   Please refer to `RobotLog2DB tool’s Documentation`_ for more detail about
+   these optional arguments.
+
+After getting Robot Framework result file (``output.xml``), use below sample 
+command to  import that result into TestResultWebApp's database which is hosted 
+at *localhost* as below sample command
+
+::
+
+   RobotLog2DB output.xml localhost test_user test_pw test_db
+
+Then, open TestResultWebApp with your favourite browser and you will see how 
+wonderful the execution result is displayed as below figures:
 
 Dashboard view:
 
-![Dashboard view](packagedoc/additional_docs/pictures/Dashboard.png)
+.. image:: https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/packagedoc/additional_docs/pictures/Dashboard.png?raw=true
+   :alt: Dashboard view
 
 Datatable view:
 
-![Datatable view](packagedoc/additional_docs/pictures/Datatable.png)
+.. image:: https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/packagedoc/additional_docs/pictures/Datatable.png?raw=true
+   :alt: Datatable view
 
 Contribution
 ------------
-
-We are always searching support and you are cordially invited to help to
-improve
-[RobotLog2DB](https://github.com/test-fullautomation/robotframework-robotlog2db)
-tool.
+We are always searching support and you are cordially invited to help to improve 
+**RobotLog2DB** tool.
 
 Sourcecode Documentation
 ------------------------
-
-To understand more detail about the tool\'s features, parameters and how
-Robot testcase information will be displayed on TestResultWebApp, please
-refer to [RobotLog2DB tool's
-Documentation](https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/RobotLog2DB/RobotLog2DB.pdf).
+To understand more detail about the tool's features, parameters and how Robot Framework
+testcase information will be displayed on TestResultWebApp, please refer to 
+`RobotLog2DB tool’s Documentation`_.
 
 Feedback
 --------
-
 Please feel free to give any feedback to us via
 
-Email to: [Robot Framework Support
-Group](mailto:RobotFrameworkSupportGroup@bcn.bosch.com)
+Email to: `Thomas Pollerspöck`_
 
-Issue tracking: [RobotLog2DB
-Issues](https://github.com/test-fullautomation/robotframework-robotlog2db/issues)
+Issue tracking: `RobotLog2DB Issues`_
 
 About
 -----
 
-### Maintainers
-
-[Thomas Pollerspöck](mailto:Thomas.Pollerspoeck@de.bosch.com)
+Maintainers
+~~~~~~~~~~~
+`Thomas Pollerspöck`_
 
-[Tran Duy Ngoan](mailto:Ngoan.TranDuy@vn.bosch.com)
+`Tran Duy Ngoan`_
 
-### Contributors
+Contributors
+~~~~~~~~~~~~
 
-[Nguyen Huynh Tri Cuong](mailto:Cuong.NguyenHuynhTri@vn.bosch.com)
+`Nguyen Huynh Tri Cuong`_
 
-[Mai Dinh Nam Son](mailto:Son.MaiDinhNam@vn.bosch.com)
+`Mai Dinh Nam Son`_
 
-[Tran Hoang Nguyen](mailto:Nguyen.TranHoang@vn.bosch.com)
+`Tran Hoang Nguyen`_
 
-[Holger Queckenstedt](mailto:Holger.Queckenstedt@de.bosch.com)
+`Holger Queckenstedt`_
 
-### License
+License
+~~~~~~~
 
 Copyright 2020-2022 Robert Bosch GmbH
 
-Licensed under the Apache License, Version 2.0 (the \"License\"); you
-may not use this file except in compliance with the License. You may
-obtain a copy of the License at
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
 
-> [![License: Apache
-> v2](https://img.shields.io/pypi/l/robotframework.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
+    |License: Apache v2|
 
 Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an \"AS IS\" BASIS,
+distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 
+.. |License: Apache v2| image:: https://img.shields.io/pypi/l/robotframework.svg
+   :target: http://www.apache.org/licenses/LICENSE-2.0.html
+.. _RobotLog2DB: https://github.com/test-fullautomation/robotframework-robotlog2db
+.. _TestResultWebApp: https://github.com/test-fullautomation/TestResultWebApp
+.. _Thomas Pollerspöck: mailto:Thomas.Pollerspoeck@de.bosch.com
+.. _Tran Duy Ngoan: mailto:Ngoan.TranDuy@vn.bosch.com
+.. _Nguyen Huynh Tri Cuong: mailto:Cuong.NguyenHuynhTri@vn.bosch.com
+.. _Mai Dinh Nam Son: mailto:Son.MaiDinhNam@vn.bosch.com
+.. _Tran Hoang Nguyen: mailto:Nguyen.TranHoang@vn.bosch.com
+.. _Holger Queckenstedt: mailto:Holger.Queckenstedt@de.bosch.com
+.. _RobotLog2DB tool’s Documentation: https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/RobotLog2DB/RobotLog2DB.pdf
+.. _RobotLog2DB Issues: https://github.com/test-fullautomation/robotframework-robotlog2db/issues
+.. _RobotFramework Testsuites Management: https://github.com/test-fullautomation/robotframework-testsuitesmanagement
+.. _Robot Framework XML result: https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#output-file
```

### Comparing `robotframework-robotlog2db-1.3.6/RobotLog2DB/CDataBase.py` & `robotframework-robotlog2db-1.3.7/RobotLog2DB/CDataBase.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.6/RobotLog2DB/RobotLog2DB.pdf` & `robotframework-robotlog2db-1.3.7/RobotLog2DB/RobotLog2DB.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 7% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 RobotLog2DB
-v. 1.3.6
+v. 1.3.7
 Tran Duy Ngoan
-05.04.2023
+14.06.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -2115,19 +2115,19 @@
 
 Name
 
 RobotLog2DB
 
 Version
 
-1.3.6
+1.3.7
 
 Date
 
-05.04.2023
+14.06.2023
 
 Description
 
 Imports robot result(s) to TestResultWebApp database
 
 Package URL
 
@@ -2241,19 +2241,24 @@
 Support 4 byte characters for importing to db
 1.3.6
 
 05.04.2023
 
 - Enhance console log with test case counter and component statistics
 - Add try/except for database access
+1.3.7
+
+14.06.2023
+
+Update README with new instruction for installation and image’s links
 
 32
 
 CHAPTER 6. HISTORY
 
 RobotLog2DB.pdf
-Created at 08.06.2023 - 14:02:07
+Created at 14.06.2023 - 08:58:27
 by GenPackageDoc v. 0.40.3
 
 33
```

### Comparing `robotframework-robotlog2db-1.3.6/RobotLog2DB/__init__.py` & `robotframework-robotlog2db-1.3.7/RobotLog2DB/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.6/RobotLog2DB/__main__.py` & `robotframework-robotlog2db-1.3.7/RobotLog2DB/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.6/RobotLog2DB/robotlog2db.py` & `robotframework-robotlog2db-1.3.7/RobotLog2DB/robotlog2db.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.6/RobotLog2DB/xsd/robot.xsd` & `robotframework-robotlog2db-1.3.7/RobotLog2DB/xsd/robot.xsd`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.6/robotframework_robotlog2db.egg-info/PKG-INFO` & `robotframework-robotlog2db-1.3.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2db
-Version: 1.3.6
+Version: 1.3.7
 Summary: Imports robot result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -33,52 +33,106 @@
     -   [Maintainers](#maintainers)
     -   [Contributors](#contributors)
     -   [License](#license)
 
 Getting Started
 ---------------
 
-[RobotLog2DB](https://github.com/test-fullautomation/robotframework-robotlog2db)
-is the tool that helps to import Robot Framework results (**\*.xml**
-format) to
-[TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)
-Dashboard.
+**RobotLog2DB** is a command-line tool that enables you to import [Robot
+Framework XML
+result](https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#output-file)
+files into
+[TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)\'s
+database for presenting an overview about the whole test execution and
+detail of each test result.
 
-[RobotLog2DB](https://github.com/test-fullautomation/robotframework-robotlog2db)
-tool is operating system independent and only works with Python 3.
+**RobotLog2DB** tool is operating system independent and only works with
+Python 3.
 
 ### How to install
 
-RobotLog2DB is not available on [PyPI](https://pypi.org/) now.
+**RobotLog2DB** can be installed in two different ways.
+
+1.  Installation via PyPi (recommended for users)
+
+    ``` {.}
+    pip install robotframework-robotlog2db
+    ```
+
+    [RobotLog2DB in
+    PyPi](https://pypi.org/project/robotframework-robotlog2db/)
+
+2.  Installation via GitHub (recommended for developers)
+
+    -   Clone the **robotframework-robotlog2db** repository to your
+        machine.
+
+        ``` {.}
+        git clone https://github.com/test-fullautomation/robotframework-robotlog2db.git
+        ```
+
+        [RobotLog2DB in
+        GitHub](https://github.com/test-fullautomation/robotframework-robotlog2db)
+
+    -   Install dependencies
+
+        **RobotLog2DB** requires some additional Python libraries.
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
+        The installation of **RobotLog2DB** includes to generate the
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
 
-    pip install git+https://github.com/test-fullautomation/robotframework-robotlog2db.git
+        -   `GENDOC_LATEXPATH` : path to `pdflatex` executable
 
-Or you can clone sourcecode to your local directory then install this
-package with below steps:
+    -   Use the following command to install **RobotLog2DB**:
 
-    git clone https://github.com/test-fullautomation/robotframework-robotlog2db.git
-    cd robotframework-robotlog2db
-    python setup.py install
+        ``` {.}
+        python setup.py install
+        ```
 
 After succesful installation, the executable file **RobotLog2DB** will
 be available (under *Scripts* folder of Python on Windows and
 *\~/.local/bin/* folder on Linux).
 
 In case above location is added to **PATH** environment variable then
 you can run it directly as operation system\'s command.
 
 Usage
 -----
 
-[RobotLog2DB](https://github.com/test-fullautomation/robotframework-robotlog2db)
-requires the Robot Framework result file(s) which contains the output
-result in XML format (default name is `output.xml`) and
+**RobotLog2DB** requires the Robot Framework result file(s) which
+contains the output result in XML format (default name is `output.xml`)
+and
 [TestResultWebApp](https://github.com/test-fullautomation/TestResultWebApp)\'s
 database information for importing.
 
 Use below command to get tools\'s usage
 
     RobotLog2DB -h
 
@@ -104,43 +158,43 @@
     --append             is used in combination with --UUID <UUID>.If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
     --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided RobotLog2DB will generate an UUID for the whole import.
     --variant VARIANT    variant name to be set for this import.
     --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
     --config CONFIG      configuration json file for component mapping information.
 
 The below command is simple usage with all required arguments to import
-robot results into TestResultWebApp\'s database:
+Robot Framework results into TestResultWebApp\'s database:
 
     RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Besides the executable file, you can also run tool as a Python module
 
     python -m RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Example
 -------
 
-In order the import the robot result(s) to TestResultWebApp\'s database,
-we need the Robot Framework result file (`output.xml`).
+In order the import the Robot Framework result(s) to TestResultWebApp\'s
+database, we need the Robot Framework result file (`output.xml`).
 
-So, firstly execute the robot testcase(s) to get the Robot Framework
-result file.
+So, firstly execute the Robot Framework testcase(s) to get the Robot
+Framework result file.
 
-Sample robot testcase which contains neccessary information for
-importing into TestResultWebApp\'s database:
+Sample Robot Framework testcase which contains neccessary information
+for importing into TestResultWebApp\'s database:
 
     *** Settings ***
     # Test execution level
     Metadata   project        ROBFW              # Project/Variant
     Metadata   version_sw     SW_VERSION_0.1     # Software version
     Metadata   version_hw     HW_VERSION_0.1     # Hardware version
     Metadata   version_test   TEST_VERSION_0.1   # Test version
 
     # File/Suite level
-    Documentation             This is description for robot test file
+    Documentation             This is description for Robot Framework test file
     Metadata    author        Tran Duy Ngoan (RBVH/ECM1)
     Metadata    component     Import_Tools
     Metadata    testtool      Robot Framework 3.2rc2 (Python 3.9.0 on win32)
     Metadata    machine       %{COMPUTERNAME}
     Metadata    tester        %{USER}
 
     *** Test Cases ***
@@ -163,70 +217,68 @@
 > -   version\_sw
 > -   version\_hw
 > -   version\_test
 > -   machine
 > -   tester
 > -   testtool
 >
-> So that you do not need to define them in your Robot testcase(s).
+> So that you do not need to define them in your Robot Framework
+> testcase(s).
 >
 > However, if these `Metadata` definitions are already missing in the
-> RobotFramework output result file, you can specific them when
-> executing the RobotLog2DB tool with the optional arguments:
+> Robot Framework output result file, you can specific them when
+> executing the **RobotLog2DB** tool with the optional arguments:
 >
 > -   `--variant VARIANT`: Project definitions
 > -   `--versions VERSIONS`: Versions (Software;Hardware;Test)
 >     definitions.
 > -   `--config CONFIG`: Project, versions or component mapping
 >     definitions.
 >
 > Please refer to [RobotLog2DB tool's
 > Documentation](https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/RobotLog2DB/RobotLog2DB.pdf)
 > for more detail about these optional arguments.
 
-After getting Robot Framwork result file (`output.xml`), use below
+After getting Robot Framework result file (`output.xml`), use below
 sample command to import that result into TestResultWebApp\'s database
 which is hosted at *localhost* as below sample command
 
     RobotLog2DB output.xml localhost test_user test_pw test_db
 
 Then, open TestResultWebApp with your favourite browser and you will see
 how wonderful the execution result is displayed as below figures:
 
 Dashboard view:
 
-![Dashboard view](packagedoc/additional_docs/pictures/Dashboard.png)
+![Dashboard view](https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/packagedoc/additional_docs/pictures/Dashboard.png?raw=true)
 
 Datatable view:
 
-![Datatable view](packagedoc/additional_docs/pictures/Datatable.png)
+![Datatable view](https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/packagedoc/additional_docs/pictures/Datatable.png?raw=true)
 
 Contribution
 ------------
 
 We are always searching support and you are cordially invited to help to
-improve
-[RobotLog2DB](https://github.com/test-fullautomation/robotframework-robotlog2db)
-tool.
+improve **RobotLog2DB** tool.
 
 Sourcecode Documentation
 ------------------------
 
 To understand more detail about the tool\'s features, parameters and how
-Robot testcase information will be displayed on TestResultWebApp, please
-refer to [RobotLog2DB tool's
+Robot Framework testcase information will be displayed on
+TestResultWebApp, please refer to [RobotLog2DB tool's
 Documentation](https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/RobotLog2DB/RobotLog2DB.pdf).
 
 Feedback
 --------
 
 Please feel free to give any feedback to us via
 
-Email to: [Robot Framework Support
-Group](mailto:RobotFrameworkSupportGroup@bcn.bosch.com)
+Email to: [Thomas Pollerspöck](mailto:Thomas.Pollerspoeck@de.bosch.com)
 
 Issue tracking: [RobotLog2DB
 Issues](https://github.com/test-fullautomation/robotframework-robotlog2db/issues)
 
 About
 -----
```

### Comparing `robotframework-robotlog2db-1.3.6/setup.py` & `robotframework-robotlog2db-1.3.7/setup.py`

 * *Files identical despite different names*

