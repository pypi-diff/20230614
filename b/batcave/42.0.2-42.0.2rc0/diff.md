# Comparing `tmp/batcave-42.0.2.tar.gz` & `tmp/batcave-42.0.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batcave-42.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "batcave-42.0.2rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `batcave-42.0.2.tar` & `batcave-42.0.2rc0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     4792 2023-06-14 20:54:54.221057 batcave-42.0.2/.gitignore
--rw-r--r--   0        0        0     3569 2023-06-14 20:54:54.221057 batcave-42.0.2/.gitlab-ci.yml
--rw-r--r--   0        0        0       23 2023-06-14 20:54:54.221057 batcave-42.0.2/.p4cfg
--rw-r--r--   0        0        0     5043 2023-06-14 20:54:54.221057 batcave-42.0.2/.p4ignore
--rw-r--r--   0        0        0      158 2023-06-14 20:54:54.221057 batcave-42.0.2/.pypirc
--rw-r--r--   0        0        0       39 2023-06-14 20:54:54.221057 batcave-42.0.2/.readthedocs.yml
--rw-r--r--   0        0        0     4034 2023-06-14 20:54:54.221057 batcave-42.0.2/.vscode/.ropeproject/config.py
--rw-r--r--   0        0        0      592 2023-06-14 20:54:54.221057 batcave-42.0.2/.vscode/.ropeproject/objectdb
--rw-r--r--   0        0        0     5757 2023-06-14 20:54:54.221057 batcave-42.0.2/.vscode/launch.json
--rw-r--r--   0        0        0      468 2023-06-14 20:54:54.221057 batcave-42.0.2/.vscode/tasks.json
--rw-r--r--   0        0        0    38420 2023-06-14 20:54:54.222057 batcave-42.0.2/CHANGELOG.md
--rw-r--r--   0        0        0       86 2023-06-14 20:54:54.222057 batcave-42.0.2/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2023-06-14 20:54:54.222057 batcave-42.0.2/LICENSE
--rw-r--r--   0        0        0       93 2023-06-14 20:54:54.222057 batcave-42.0.2/MANIFEST.in
--rw-r--r--   0        0        0     1017 2023-06-14 20:54:54.222057 batcave-42.0.2/README.md
--rw-r--r--   0        0        0     1832 2023-06-14 20:55:21.730131 batcave-42.0.2/batcave/__init__.py
--rw-r--r--   0        0        0     5483 2023-06-14 20:54:54.222057 batcave-42.0.2/batcave/automation.py
--rw-r--r--   0        0        0    14410 2023-06-14 20:54:54.222057 batcave-42.0.2/batcave/cloudmgr.py
--rw-r--r--   0        0        0    74524 2023-06-14 20:54:54.222057 batcave-42.0.2/batcave/cms.py
--rw-r--r--   0        0        0     8590 2023-06-14 20:54:54.222057 batcave-42.0.2/batcave/commander.py
--rw-r--r--   0        0        0     9565 2023-06-14 20:54:54.222057 batcave-42.0.2/batcave/configmgr.py
--rw-r--r--   0        0        0    27694 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/data.py
--rw-r--r--   0        0        0    31760 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/expander.py
--rw-r--r--   0        0        0     8908 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/fileutil.py
--rw-r--r--   0        0        0    10747 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/gui.py
--rw-r--r--   0        0        0    28879 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/iispy.py
--rw-r--r--   0        0        0    17890 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/k8s.py
--rw-r--r--   0        0        0    10608 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/lang.py
--rw-r--r--   0        0        0     3140 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/menu.py
--rw-r--r--   0        0        0     2378 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/netutil.py
--rw-r--r--   0        0        0     3842 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/platarch.py
--rw-r--r--   0        0        0        0 2023-06-14 20:54:54.246057 batcave-42.0.2/batcave/py.typed
--rw-r--r--   0        0        0    13106 2023-06-14 20:54:54.223057 batcave-42.0.2/batcave/qbpy.py
--rw-r--r--   0        0        0    28247 2023-06-14 20:54:54.224057 batcave-42.0.2/batcave/reporter.py
--rw-r--r--   0        0        0    52861 2023-06-14 20:54:54.224057 batcave-42.0.2/batcave/servermgr.py
--rw-r--r--   0        0        0    11200 2023-06-14 20:54:54.224057 batcave-42.0.2/batcave/serverpath.py
--rw-r--r--   0        0        0     7801 2023-06-14 20:54:54.224057 batcave-42.0.2/batcave/statemachine.py
--rw-r--r--   0        0        0    23468 2023-06-14 20:54:54.224057 batcave-42.0.2/batcave/sysutil.py
--rw-r--r--   0        0        0     5429 2023-06-14 20:54:54.224057 batcave-42.0.2/batcave/tcpy.py
--rw-r--r--   0        0        0     3340 2023-06-14 20:54:54.224057 batcave-42.0.2/batcave/version.py
--rw-r--r--   0        0        0      634 2023-06-14 20:54:54.224057 batcave-42.0.2/docs/Makefile
--rw-r--r--   0        0        0     3747 2023-06-14 20:54:54.224057 batcave-42.0.2/docs/batcave.rst
--rw-r--r--   0        0        0     9167 2023-06-14 20:54:54.224057 batcave-42.0.2/docs/coding_standards.py
--rw-r--r--   0        0        0     2109 2023-06-14 20:54:54.224057 batcave-42.0.2/docs/conf.py
--rw-r--r--   0        0        0      469 2023-06-14 20:54:54.224057 batcave-42.0.2/docs/index.rst
--rw-r--r--   0        0        0      795 2023-06-14 20:54:54.224057 batcave-42.0.2/docs/make.bat
--rw-r--r--   0        0        0       65 2023-06-14 20:54:54.224057 batcave-42.0.2/docs/modules.rst
--rw-r--r--   0        0        0      229 2023-06-14 20:54:54.225057 batcave-42.0.2/docs/requirements.txt
--rw-r--r--   0        0        0     2794 2023-06-14 20:55:21.730131 batcave-42.0.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-14 20:54:54.225057 batcave-42.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1253 2023-06-14 20:54:54.225057 batcave-42.0.2/tests/test_lang.py
--rw-r--r--   0        0        0     2744 2023-06-14 20:54:54.225057 batcave-42.0.2/tests/test_statemachine.py
--rw-r--r--   0        0        0     3062 2023-06-14 20:54:54.225057 batcave-42.0.2/tests/test_sysutil.py
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 batcave-42.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4792 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.gitignore
+-rw-r--r--   0        0        0     3569 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.gitlab-ci.yml
+-rw-r--r--   0        0        0       23 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.p4cfg
+-rw-r--r--   0        0        0     5043 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.p4ignore
+-rw-r--r--   0        0        0      158 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.pypirc
+-rw-r--r--   0        0        0       39 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.readthedocs.yml
+-rw-r--r--   0        0        0     4034 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.vscode/.ropeproject/config.py
+-rw-r--r--   0        0        0      592 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.vscode/.ropeproject/objectdb
+-rw-r--r--   0        0        0     5757 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.vscode/launch.json
+-rw-r--r--   0        0        0      468 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/.vscode/tasks.json
+-rw-r--r--   0        0        0    38420 2023-06-14 20:48:50.617110 batcave-42.0.2rc0/CHANGELOG.md
+-rw-r--r--   0        0        0       86 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/LICENSE
+-rw-r--r--   0        0        0       93 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/MANIFEST.in
+-rw-r--r--   0        0        0     1017 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/README.md
+-rw-r--r--   0        0        0     1835 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/batcave/__init__.py
+-rw-r--r--   0        0        0     5483 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/batcave/automation.py
+-rw-r--r--   0        0        0    14410 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/batcave/cloudmgr.py
+-rw-r--r--   0        0        0    74524 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/batcave/cms.py
+-rw-r--r--   0        0        0     8590 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/batcave/commander.py
+-rw-r--r--   0        0        0     9565 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/batcave/configmgr.py
+-rw-r--r--   0        0        0    27694 2023-06-14 20:48:50.618110 batcave-42.0.2rc0/batcave/data.py
+-rw-r--r--   0        0        0    31760 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/expander.py
+-rw-r--r--   0        0        0     8908 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/fileutil.py
+-rw-r--r--   0        0        0    10747 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/gui.py
+-rw-r--r--   0        0        0    28879 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/iispy.py
+-rw-r--r--   0        0        0    17890 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/k8s.py
+-rw-r--r--   0        0        0    10608 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/lang.py
+-rw-r--r--   0        0        0     3140 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/menu.py
+-rw-r--r--   0        0        0     2378 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/netutil.py
+-rw-r--r--   0        0        0     3842 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/platarch.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:48:50.642110 batcave-42.0.2rc0/batcave/py.typed
+-rw-r--r--   0        0        0    13106 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/qbpy.py
+-rw-r--r--   0        0        0    28247 2023-06-14 20:48:50.619110 batcave-42.0.2rc0/batcave/reporter.py
+-rw-r--r--   0        0        0    52861 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/batcave/servermgr.py
+-rw-r--r--   0        0        0    11200 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/batcave/serverpath.py
+-rw-r--r--   0        0        0     7801 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/batcave/statemachine.py
+-rw-r--r--   0        0        0    23468 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/batcave/sysutil.py
+-rw-r--r--   0        0        0     5429 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/batcave/tcpy.py
+-rw-r--r--   0        0        0     3340 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/batcave/version.py
+-rw-r--r--   0        0        0      634 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/docs/Makefile
+-rw-r--r--   0        0        0     3747 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/docs/batcave.rst
+-rw-r--r--   0        0        0     9167 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/docs/coding_standards.py
+-rw-r--r--   0        0        0     2109 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/docs/conf.py
+-rw-r--r--   0        0        0      469 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/docs/make.bat
+-rw-r--r--   0        0        0       65 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/docs/modules.rst
+-rw-r--r--   0        0        0      229 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/docs/requirements.txt
+-rw-r--r--   0        0        0     2797 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-14 20:48:50.620110 batcave-42.0.2rc0/tests/__init__.py
+-rw-r--r--   0        0        0     1253 2023-06-14 20:48:50.621110 batcave-42.0.2rc0/tests/test_lang.py
+-rw-r--r--   0        0        0     2744 2023-06-14 20:48:50.621110 batcave-42.0.2rc0/tests/test_statemachine.py
+-rw-r--r--   0        0        0     3062 2023-06-14 20:48:50.621110 batcave-42.0.2rc0/tests/test_sysutil.py
+-rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 batcave-42.0.2rc0/PKG-INFO
```

### Comparing `batcave-42.0.2/.gitignore` & `batcave-42.0.2rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/.gitlab-ci.yml` & `batcave-42.0.2rc0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/.p4ignore` & `batcave-42.0.2rc0/.p4ignore`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/.vscode/.ropeproject/config.py` & `batcave-42.0.2rc0/.vscode/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/.vscode/.ropeproject/objectdb` & `batcave-42.0.2rc0/.vscode/.ropeproject/objectdb`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/.vscode/launch.json` & `batcave-42.0.2rc0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/CHANGELOG.md` & `batcave-42.0.2rc0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/LICENSE` & `batcave-42.0.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/README.md` & `batcave-42.0.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/__init__.py` & `batcave-42.0.2rc0/batcave/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
            '__author__', '__email__',
            '__license__', '__copyright__')
 
 __title__ = 'BatCave'
 __summary__ = 'Python Programming Toolkit'
 __uri__ = 'https://gitlab.com/arisilon/batcave/'
 
-__version__ = '42.0.2'
+__version__ = '42.0.2rc0'
 __build_name__ = '{var:build_name}'
 __build_date__ = '{var:build_date}'
 
 __author__ = 'Jeffery G. Smith'
 __email__ = 'web@pobox.com'
 
 __license__ = 'MIT'
```

### Comparing `batcave-42.0.2/batcave/automation.py` & `batcave-42.0.2rc0/batcave/automation.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/cloudmgr.py` & `batcave-42.0.2rc0/batcave/cloudmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/cms.py` & `batcave-42.0.2rc0/batcave/cms.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/commander.py` & `batcave-42.0.2rc0/batcave/commander.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/configmgr.py` & `batcave-42.0.2rc0/batcave/configmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/data.py` & `batcave-42.0.2rc0/batcave/data.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/expander.py` & `batcave-42.0.2rc0/batcave/expander.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/fileutil.py` & `batcave-42.0.2rc0/batcave/fileutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/gui.py` & `batcave-42.0.2rc0/batcave/gui.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/iispy.py` & `batcave-42.0.2rc0/batcave/iispy.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/k8s.py` & `batcave-42.0.2rc0/batcave/k8s.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/lang.py` & `batcave-42.0.2rc0/batcave/lang.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/menu.py` & `batcave-42.0.2rc0/batcave/menu.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/netutil.py` & `batcave-42.0.2rc0/batcave/netutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/platarch.py` & `batcave-42.0.2rc0/batcave/platarch.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/qbpy.py` & `batcave-42.0.2rc0/batcave/qbpy.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/reporter.py` & `batcave-42.0.2rc0/batcave/reporter.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/servermgr.py` & `batcave-42.0.2rc0/batcave/servermgr.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/serverpath.py` & `batcave-42.0.2rc0/batcave/serverpath.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/statemachine.py` & `batcave-42.0.2rc0/batcave/statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/sysutil.py` & `batcave-42.0.2rc0/batcave/sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/tcpy.py` & `batcave-42.0.2rc0/batcave/tcpy.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/batcave/version.py` & `batcave-42.0.2rc0/batcave/version.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/docs/Makefile` & `batcave-42.0.2rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/docs/batcave.rst` & `batcave-42.0.2rc0/docs/batcave.rst`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/docs/coding_standards.py` & `batcave-42.0.2rc0/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/docs/conf.py` & `batcave-42.0.2rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/docs/make.bat` & `batcave-42.0.2rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/pyproject.toml` & `batcave-42.0.2rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "wmi.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "42.0.2"
+current_version = "42.0.2rc0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip-ci]"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `batcave-42.0.2/tests/test_lang.py` & `batcave-42.0.2rc0/tests/test_lang.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/tests/test_statemachine.py` & `batcave-42.0.2rc0/tests/test_statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/tests/test_sysutil.py` & `batcave-42.0.2rc0/tests/test_sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-42.0.2/PKG-INFO` & `batcave-42.0.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batcave
-Version: 42.0.2
+Version: 42.0.2rc0
 Summary: BatCave Utilities module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

