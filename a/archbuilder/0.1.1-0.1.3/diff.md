# Comparing `tmp/archbuilder-0.1.1.tar.gz` & `tmp/archbuilder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archbuilder-0.1.1.tar", last modified: Tue Jun 13 17:18:09 2023, max compression
+gzip compressed data, was "archbuilder-0.1.3.tar", last modified: Wed Jun 14 11:26:53 2023, max compression
```

## Comparing `archbuilder-0.1.1.tar` & `archbuilder-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.535076 archbuilder-0.1.1/
--rw-rw-rw-   0        0        0       29 2023-05-31 23:56:47.000000 archbuilder-0.1.1/.coveragerc
--rw-rw-rw-   0        0        0       80 2023-06-12 15:29:27.000000 archbuilder-0.1.1/.flake8
--rw-rw-rw-   0        0        0      295 2023-06-10 13:44:10.000000 archbuilder-0.1.1/.gitignore
--rw-rw-rw-   0        0        0        8 2023-06-10 13:45:01.000000 archbuilder-0.1.1/.python-version
--rw-rw-rw-   0        0        0     1497 2023-06-13 17:18:09.533078 archbuilder-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-12 17:46:00.000000 archbuilder-0.1.1/Pipfile
--rw-rw-rw-   0        0        0    33014 2023-06-12 17:47:23.000000 archbuilder-0.1.1/Pipfile.lock
--rw-rw-rw-   0        0        0     1195 2023-06-13 17:12:25.000000 archbuilder-0.1.1/README.md
--rw-rw-rw-   0        0        0      493 2023-06-13 17:17:09.000000 archbuilder-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      154 2023-05-31 23:59:03.000000 archbuilder-0.1.1/pytest.ini
--rw-rw-rw-   0        0        0       42 2023-06-13 17:18:09.535076 archbuilder-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.415073 archbuilder-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.479076 archbuilder-0.1.1/src/archbuilder/
--rw-rw-rw-   0        0        0      700 2023-06-13 17:06:49.000000 archbuilder-0.1.1/src/archbuilder/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.497083 archbuilder-0.1.1/src/archbuilder.egg-info/
--rw-rw-rw-   0        0        0     1497 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-13 17:18:09.000000 archbuilder-0.1.1/src/archbuilder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.506081 archbuilder-0.1.1/src/builder/
--rw-rw-rw-   0        0        0       30 2023-06-12 16:35:52.000000 archbuilder-0.1.1/src/builder/__init__.py
--rw-rw-rw-   0        0        0      736 2023-06-13 17:16:18.000000 archbuilder-0.1.1/src/builder/builder.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.518077 archbuilder-0.1.1/src/template/
--rw-rw-rw-   0        0        0       32 2023-06-12 16:42:50.000000 archbuilder-0.1.1/src/template/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-06-10 12:46:22.000000 archbuilder-0.1.1/src/template/template.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.419080 archbuilder-0.1.1/tests/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:18:09.528077 archbuilder-0.1.1/tests/unit/
--rw-rw-rw-   0        0        0      390 2023-06-12 15:12:19.000000 archbuilder-0.1.1/tests/unit/test_builder.py
--rw-rw-rw-   0        0        0      608 2023-06-13 17:16:18.000000 archbuilder-0.1.1/tests/unit/test_template.py
--rw-rw-rw-   0        0        0      782 2023-06-10 17:45:09.000000 archbuilder-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.168307 archbuilder-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.160307 archbuilder-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.164307 archbuilder-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.github/workflows/testpypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 11:26:37.000000 archbuilder-0.1.3/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-14 11:26:53.168307 archbuilder-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 11:26:37.000000 archbuilder-0.1.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    33014 2023-06-14 11:26:37.000000 archbuilder-0.1.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-14 11:26:37.000000 archbuilder-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 11:26:37.000000 archbuilder-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 11:26:37.000000 archbuilder-0.1.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:26:53.168307 archbuilder-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.160307 archbuilder-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.164307 archbuilder-0.1.3/src/archbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/archbuilder/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.164307 archbuilder-0.1.3/src/archbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 11:26:53.000000 archbuilder-0.1.3/src/archbuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.164307 archbuilder-0.1.3/src/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.168307 archbuilder-0.1.3/src/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-14 11:26:37.000000 archbuilder-0.1.3/src/template/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.160307 archbuilder-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:26:53.168307 archbuilder-0.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-14 11:26:37.000000 archbuilder-0.1.3/tests/unit/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 11:26:37.000000 archbuilder-0.1.3/tests/unit/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 11:26:37.000000 archbuilder-0.1.3/tox.ini
```

### Comparing `archbuilder-0.1.1/PKG-INFO` & `archbuilder-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-Metadata-Version: 2.1
-Name: archbuilder
-Version: 0.1.1
-Summary: A tool to enable developers set up their projects quickly
-Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-
-# Archbuilder
-
-Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
-```bash
-  pip install archbuilder
-```
-    
-## Usage
-
-##### 1. By using a python script
-```python
-# Import archbuilder
-from builder import Builder
-from template import Template
-
-# Create a template from a json file
-template = Template('sass.json')
-
-# Create the project tree from the template
-project = Builder('sass', template)
-project.build()
-```
-
-##### 2. By using the command-line
-Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
-```bash
-archbuilder sass sass.json
-```
-
-## Contributing
-
-Contributions are always welcome!
-
-For major changes, please open an issue first
-to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-## License
-
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: archbuilder
+Version: 0.1.3
+Summary: A tool to enable developers set up their projects quickly
+Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+
+# Archbuilder
+
+Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
+```bash
+  pip install archbuilder
+```
+    
+## Usage
+
+##### 1. By using a python script
+```python
+# Import archbuilder
+from builder import Builder
+from template import Template
+
+# Create a template from a json file
+template = Template('sass.json')
+
+# Create the project tree from the template
+project = Builder('sass', template)
+project.build()
+```
+
+##### 2. By using the command-line
+Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
+```bash
+archbuilder sass sass.json
+```
+
+## Contributing
+
+Contributions are always welcome!
+
+For major changes, please open an issue first
+to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+## License
+
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
```

### Comparing `archbuilder-0.1.1/Pipfile.lock` & `archbuilder-0.1.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `archbuilder-0.1.1/README.md` & `archbuilder-0.1.3/src/archbuilder.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,54 @@
-
-# Archbuilder
-
-Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
-```bash
-  pip install archbuilder
-```
-    
-## Usage
-
-##### 1. By using a python script
-```python
-# Import archbuilder
-from builder import Builder
-from template import Template
-
-# Create a template from a json file
-template = Template('sass.json')
-
-# Create the project tree from the template
-project = Builder('sass', template)
-project.build()
-```
-
-##### 2. By using the command-line
-Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
-```bash
-archbuilder sass sass.json
-```
-
-## Contributing
-
-Contributions are always welcome!
-
-For major changes, please open an issue first
-to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-## License
-
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1
+Name: archbuilder
+Version: 0.1.3
+Summary: A tool to enable developers set up their projects quickly
+Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+
+# Archbuilder
+
+Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
+```bash
+  pip install archbuilder
+```
+    
+## Usage
+
+##### 1. By using a python script
+```python
+# Import archbuilder
+from builder import Builder
+from template import Template
+
+# Create a template from a json file
+template = Template('sass.json')
+
+# Create the project tree from the template
+project = Builder('sass', template)
+project.build()
+```
+
+##### 2. By using the command-line
+Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
+```bash
+archbuilder sass sass.json
+```
+
+## Contributing
+
+Contributions are always welcome!
+
+For major changes, please open an issue first
+to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+## License
+
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
```

### Comparing `archbuilder-0.1.1/src/archbuilder.egg-info/PKG-INFO` & `archbuilder-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-Metadata-Version: 2.1
-Name: archbuilder
-Version: 0.1.1
-Summary: A tool to enable developers set up their projects quickly
-Author-email: "Coleman A. Matey" <colemanmatey@icloud.com>
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-
-# Archbuilder
-
-Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
-```bash
-  pip install archbuilder
-```
-    
-## Usage
-
-##### 1. By using a python script
-```python
-# Import archbuilder
-from builder import Builder
-from template import Template
-
-# Create a template from a json file
-template = Template('sass.json')
-
-# Create the project tree from the template
-project = Builder('sass', template)
-project.build()
-```
-
-##### 2. By using the command-line
-Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
-```bash
-archbuilder sass sass.json
-```
-
-## Contributing
-
-Contributions are always welcome!
-
-For major changes, please open an issue first
-to discuss what you would like to change.
-
-Please make sure to update tests as appropriate.
-## License
-
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
+
+# Archbuilder
+
+Archbuilder is a tool that aims to speed up the setting up of projects by creating the project directories and files from user-defined templates.
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Archbuilder.
+```bash
+  pip install archbuilder
+```
+    
+## Usage
+
+##### 1. By using a python script
+```python
+# Import archbuilder
+from builder import Builder
+from template import Template
+
+# Create a template from a json file
+template = Template('sass.json')
+
+# Create the project tree from the template
+project = Builder('sass', template)
+project.build()
+```
+
+##### 2. By using the command-line
+Invoke archbuilder to create your project. Pass the name of the project as the first argument and the path to the json file as the second argument
+```bash
+archbuilder sass sass.json
+```
+
+## Contributing
+
+Contributions are always welcome!
+
+For major changes, please open an issue first
+to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+## License
+
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
```

### Comparing `archbuilder-0.1.1/src/builder/builder.py` & `archbuilder-0.1.3/src/builder/builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-"""
-"""
-from pathlib import Path
-
-
-class Builder:
-    """"""
-
-    def __init__(self, project, template, output="build", root=Path.cwd()):
-        """"""
-        self.project = project
-        self.template = template
-        self.output = output
-        self.root = root
-
-    def build(self):
-        """"""
-        for path in self.paths():
-            if not path.exists():
-                path.parent.mkdir(parents=True, exist_ok=True)
-                path.touch(exist_ok=True)
-
-    def paths(self):
-        """"""
-        paths = list()
-        for tail in self.template.tails():
-            path = Path(self.root / self.output / self.project / tail)
-            paths.append(path)
-        return paths
+"""
+"""
+
+from pathlib import Path
+
+
+class Builder:
+    """"""
+
+    def __init__(self, project, template, output="build", root=Path.cwd()):
+        """"""
+        self.project = project
+        self.template = template
+        self.output = output
+        self.root = root
+
+    def build(self):
+        """"""
+        for path in self.paths():
+            if not path.exists():
+                path.parent.mkdir(parents=True, exist_ok=True)
+                path.touch(exist_ok=True)
+
+    def paths(self):
+        """"""
+        paths = list()
+        for tail in self.template.tails():
+            path = Path(self.root / self.output / self.project / tail)
+            paths.append(path)
+        return paths
```

