# Comparing `tmp/robotframework-robotlog2rqm-1.2.0.tar.gz` & `tmp/robotframework-robotlog2rqm-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robotlog2rqm-1.2.0.tar", last modified: Thu Jun  8 14:02:49 2023, max compression
+gzip compressed data, was "robotframework-robotlog2rqm-1.2.1.tar", last modified: Wed Jun 14 09:10:51 2023, max compression
```

## Comparing `robotframework-robotlog2rqm-1.2.0.tar` & `robotframework-robotlog2rqm-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:49.653113 robotframework-robotlog2rqm-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-08 14:02:49.653113 robotframework-robotlog2rqm-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:49.649113 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/
--rw-r--r--   0 runner    (1001) docker     (123)    54873 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/CRQM.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:49.653113 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/buildrecord.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/configuration.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/executionresult.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/executionworkitem.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/suiteexecutionrecord.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/testcase.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/testsuitelog.xml
--rw-r--r--   0 runner    (1001) docker     (123)   227483 2023-06-08 14:02:49.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RobotLog2RQM.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/robotlog2rqm.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:49.653113 robotframework-robotlog2rqm-1.2.0/robotframework_robotlog2rqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-08 14:02:49.000000 robotframework-robotlog2rqm-1.2.0/robotframework_robotlog2rqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-08 14:02:49.000000 robotframework-robotlog2rqm-1.2.0/robotframework_robotlog2rqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:02:49.000000 robotframework-robotlog2rqm-1.2.0/robotframework_robotlog2rqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 14:02:49.000000 robotframework-robotlog2rqm-1.2.0/robotframework_robotlog2rqm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:02:49.000000 robotframework-robotlog2rqm-1.2.0/robotframework_robotlog2rqm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 14:02:49.000000 robotframework-robotlog2rqm-1.2.0/robotframework_robotlog2rqm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:02:49.653113 robotframework-robotlog2rqm-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-08 13:59:58.000000 robotframework-robotlog2rqm-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/
+-rw-r--r--   0 runner    (1001) docker     (123)    54873 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/CRQM.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/buildrecord.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/configuration.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/executionresult.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/executionworkitem.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/suiteexecutionrecord.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/testcase.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/testsuitelog.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   227725 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RobotLog2RQM.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/robotlog2rqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 09:10:51.000000 robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:10:51.524300 robotframework-robotlog2rqm-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-14 09:08:03.000000 robotframework-robotlog2rqm-1.2.1/setup.py
```

### Comparing `robotframework-robotlog2rqm-1.2.0/LICENSE` & `robotframework-robotlog2rqm-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/PKG-INFO` & `robotframework-robotlog2rqm-1.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2rqm
-Version: 1.2.0
+Version: 1.2.1
 Summary: Imports robot result(s) to IBM Rational Quality Manager (RQM)
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2rqm
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -45,32 +45,71 @@
 
 1.  Installation via PyPi (recommended for users)
 
     ``` {.}
     pip install RobotLog2RQM
     ```
 
-    [RobotLog2RQM in PyPi](https://pypi.org/project/RobotLog2RQM/)
+    [RobotLog2RQM in
+    PyPi](https://pypi.org/project/robotframework-robotlog2rqm/)
 
 2.  Installation via GitHub (recommended for developers)
 
-    Clone the **python-robotlog2rqm** repository to your machine.
+    -   Clone the **robotframework-robotlog2rqm** repository to your
+        machine.
 
-    ``` {.}
-    git clone https://github.com/test-fullautomation/python-robotlog2rqm.git
-    ```
+        ``` {.}
+        git clone https://github.com/test-fullautomation/robotframework-robotlog2rqm.git
+        ```
 
-    [RobotLog2RQM in
-    GitHub](https://github.com/test-fullautomation/python-robotlog2rqm)
+        [RobotLog2RQM in
+        GitHub](https://github.com/test-fullautomation/robotframework-robotlog2rqm)
 
-    Use the following command to install **RobotLog2RQM**:
+    -   Install dependencies
 
-    ``` {.}
-    setup.py install
-    ```
+        **RobotLog2RQM** requires some additional Python libraries.
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
+        The installation of **RobotLog2RQM** includes to generate the
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
+
+        Before you start the installation you have to introduce the
+        following environment variable, that is used in
+        `packagedoc_config.json`:
+
+        -   `GENDOC_LATEXPATH` : path to `pdflatex` executable
+
+    -   Use the following command to install **RobotLog2RQM**:
+
+        ``` {.}
+        python setup.py install
+        ```
 
 After succesful installation, the executable file **RobotLog2RQM** will
 be available (under *Scripts* folder of Python on Windows and
 *\~/.local/bin/* folder on Linux).
 
 In case above location is added to **PATH** environment variable then
 you can run it directly as operation system\'s command.
```

### Comparing `robotframework-robotlog2rqm-1.2.0/README.rst` & `robotframework-robotlog2rqm-1.2.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -37,31 +37,59 @@
 
 1. Installation via PyPi (recommended for users)
 
    .. code::
 
       pip install RobotLog2RQM
 
-   `RobotLog2RQM in PyPi <https://pypi.org/project/RobotLog2RQM/>`_
+   `RobotLog2RQM in PyPi <https://pypi.org/project/robotframework-robotlog2rqm/>`_
 
 2. Installation via GitHub (recommended for developers)
 
-   Clone the **python-robotlog2rqm** repository to your machine.
+   * Clone the **robotframework-robotlog2rqm** repository to your machine.
 
-   .. code::
+     .. code::
 
-      git clone https://github.com/test-fullautomation/python-robotlog2rqm.git
+        git clone https://github.com/test-fullautomation/robotframework-robotlog2rqm.git
 
-   `RobotLog2RQM in GitHub <https://github.com/test-fullautomation/python-robotlog2rqm>`_
+     `RobotLog2RQM in GitHub <https://github.com/test-fullautomation/robotframework-robotlog2rqm>`_
 
-   Use the following command to install **RobotLog2RQM**:
+   * Install dependencies
 
-   .. code::
+     **RobotLog2RQM** requires some additional Python libraries. Before you install the cloned repository sources
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
+     The installation of **RobotLog2RQM** includes to generate the documentation in PDF format. This is done by
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
+   * Use the following command to install **RobotLog2RQM**:
+
+     .. code::
 
-      setup.py install
+        python setup.py install
 
 After succesful installation, the executable file **RobotLog2RQM** 
 will be available (under *Scripts* folder of Python on Windows 
 and *~/.local/bin/* folder on Linux).
 
 In case above location is added to **PATH** environment variable 
 then you can run it directly as operation system's command.
```

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/CRQM.py` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/CRQM.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/buildrecord.xml` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/buildrecord.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/configuration.xml` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/configuration.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/executionresult.xml` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/executionresult.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/executionworkitem.xml` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/executionworkitem.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/suiteexecutionrecord.xml` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/suiteexecutionrecord.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/testcase.xml` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/testcase.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RQM_templates/testsuitelog.xml` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RQM_templates/testsuitelog.xml`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/RobotLog2RQM.pdf` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/RobotLog2RQM.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 10% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 RobotLog2RQM
-v. 1.2.0
+v. 1.2.1
 Tran Duy Ngoan
-09.01.2023
+14.06.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -1873,19 +1873,19 @@
 
 Name
 
 RobotLog2RQM
 
 Version
 
-1.2.0
+1.2.1
 
 Date
 
-09.01.2023
+14.06.2023
 
 Description
 
 Imports robot result(s) to IBM Rational Quality Manager (RQM)
 
 Package URL
 
@@ -1963,15 +1963,20 @@
 Rename package to RobotLog2RQM
 1.2.0
 
 09.01.2023
 
 - Rework optional arguments and improve logging messages
 - Update README and document for publishing pypi
+1.2.1
+
+14.06.2022
+
+Update README: fix links issue and update installation section
 
 RobotLog2RQM.pdf
-Created at 08.06.2023 - 14:02:45
+Created at 14.06.2023 - 09:10:48
 by GenPackageDoc v. 0.40.3
 
 27
```

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/__init__.py` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/__main__.py` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/robotlog2rqm.py` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/robotlog2rqm.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/RobotLog2RQM/version.py` & `robotframework-robotlog2rqm-1.2.1/RobotLog2RQM/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of RobotLog2RQM
 #
-VERSION      = "1.2.0"
-VERSION_DATE = "09.01.2023"
+VERSION      = "1.2.1"
+VERSION_DATE = "14.06.2023"
```

### Comparing `robotframework-robotlog2rqm-1.2.0/robotframework_robotlog2rqm.egg-info/PKG-INFO` & `robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2rqm
-Version: 1.2.0
+Version: 1.2.1
 Summary: Imports robot result(s) to IBM Rational Quality Manager (RQM)
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2rqm
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -45,32 +45,71 @@
 
 1.  Installation via PyPi (recommended for users)
 
     ``` {.}
     pip install RobotLog2RQM
     ```
 
-    [RobotLog2RQM in PyPi](https://pypi.org/project/RobotLog2RQM/)
+    [RobotLog2RQM in
+    PyPi](https://pypi.org/project/robotframework-robotlog2rqm/)
 
 2.  Installation via GitHub (recommended for developers)
 
-    Clone the **python-robotlog2rqm** repository to your machine.
+    -   Clone the **robotframework-robotlog2rqm** repository to your
+        machine.
 
-    ``` {.}
-    git clone https://github.com/test-fullautomation/python-robotlog2rqm.git
-    ```
+        ``` {.}
+        git clone https://github.com/test-fullautomation/robotframework-robotlog2rqm.git
+        ```
 
-    [RobotLog2RQM in
-    GitHub](https://github.com/test-fullautomation/python-robotlog2rqm)
+        [RobotLog2RQM in
+        GitHub](https://github.com/test-fullautomation/robotframework-robotlog2rqm)
 
-    Use the following command to install **RobotLog2RQM**:
+    -   Install dependencies
 
-    ``` {.}
-    setup.py install
-    ```
+        **RobotLog2RQM** requires some additional Python libraries.
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
+        The installation of **RobotLog2RQM** includes to generate the
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
+
+        Before you start the installation you have to introduce the
+        following environment variable, that is used in
+        `packagedoc_config.json`:
+
+        -   `GENDOC_LATEXPATH` : path to `pdflatex` executable
+
+    -   Use the following command to install **RobotLog2RQM**:
+
+        ``` {.}
+        python setup.py install
+        ```
 
 After succesful installation, the executable file **RobotLog2RQM** will
 be available (under *Scripts* folder of Python on Windows and
 *\~/.local/bin/* folder on Linux).
 
 In case above location is added to **PATH** environment variable then
 you can run it directly as operation system\'s command.
```

### Comparing `robotframework-robotlog2rqm-1.2.0/robotframework_robotlog2rqm.egg-info/SOURCES.txt` & `robotframework-robotlog2rqm-1.2.1/robotframework_robotlog2rqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2rqm-1.2.0/setup.py` & `robotframework-robotlog2rqm-1.2.1/setup.py`

 * *Files identical despite different names*

