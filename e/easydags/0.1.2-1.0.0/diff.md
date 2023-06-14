# Comparing `tmp/easydags-0.1.2.tar.gz` & `tmp/easydags-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydags-0.1.2.tar", last modified: Wed Jun 14 06:53:53 2023, max compression
+gzip compressed data, was "easydags-1.0.0.tar", last modified: Wed Jun 14 07:00:09 2023, max compression
```

## Comparing `easydags-0.1.2.tar` & `easydags-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-14 06:53:53.552911 easydags-0.1.2/
--rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.1.2/LICENSE
--rw-r--r--   0 mateograciano   (501) staff       (20)    21551 2023-06-14 06:53:53.552779 easydags-0.1.2/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)    21356 2023-06-12 08:11:31.000000 easydags-0.1.2/README.md
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-14 06:53:53.551903 easydags-0.1.2/easydags/
--rw-rw-r--   0 mateograciano   (501) staff       (20)      406 2023-06-12 22:44:01.000000 easydags-0.1.2/easydags/__init__.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.1.2/easydags/config.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    23257 2023-06-14 06:51:13.000000 easydags-0.1.2/easydags/dag.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.1.2/easydags/errors.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    12545 2023-06-12 22:43:20.000000 easydags-0.1.2/easydags/node.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)     3829 2023-06-12 07:21:06.000000 easydags-0.1.2/easydags/ops.py
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-14 06:53:53.552605 easydags-0.1.2/easydags.egg-info/
--rw-r--r--   0 mateograciano   (501) staff       (20)    21551 2023-06-14 06:53:53.000000 easydags-0.1.2/easydags.egg-info/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-14 06:53:53.000000 easydags-0.1.2/easydags.egg-info/SOURCES.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-14 06:53:53.000000 easydags-0.1.2/easydags.egg-info/dependency_links.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-14 06:53:53.000000 easydags-0.1.2/easydags.egg-info/requires.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-14 06:53:53.000000 easydags-0.1.2/easydags.egg-info/top_level.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.1.2/pyproject.toml
--rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-14 06:53:53.552947 easydags-0.1.2/setup.cfg
--rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-14 06:53:34.000000 easydags-0.1.2/setup.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-14 07:00:09.641820 easydags-1.0.0/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-1.0.0/LICENSE
+-rw-r--r--   0 mateograciano   (501) staff       (20)    21861 2023-06-14 07:00:09.641672 easydags-1.0.0/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)    21666 2023-06-14 06:59:21.000000 easydags-1.0.0/README.md
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-14 07:00:09.640777 easydags-1.0.0/easydags/
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      406 2023-06-12 22:44:01.000000 easydags-1.0.0/easydags/__init__.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-1.0.0/easydags/config.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    23257 2023-06-14 06:51:13.000000 easydags-1.0.0/easydags/dag.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-1.0.0/easydags/errors.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    12545 2023-06-12 22:43:20.000000 easydags-1.0.0/easydags/node.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)     3829 2023-06-12 07:21:06.000000 easydags-1.0.0/easydags/ops.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-14 07:00:09.641501 easydags-1.0.0/easydags.egg-info/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    21861 2023-06-14 07:00:09.000000 easydags-1.0.0/easydags.egg-info/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-14 07:00:09.000000 easydags-1.0.0/easydags.egg-info/SOURCES.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-14 07:00:09.000000 easydags-1.0.0/easydags.egg-info/dependency_links.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-14 07:00:09.000000 easydags-1.0.0/easydags.egg-info/requires.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-14 07:00:09.000000 easydags-1.0.0/easydags.egg-info/top_level.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-1.0.0/pyproject.toml
+-rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-14 07:00:09.641911 easydags-1.0.0/setup.cfg
+-rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-14 06:59:55.000000 easydags-1.0.0/setup.py
```

### Comparing `easydags-0.1.2/LICENSE` & `easydags-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easydags-0.1.2/PKG-INFO` & `easydags-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: easydags
-Version: 0.1.2
-Summary: Dags made easy
-Author: Mateo Graciano
-Author-email: magralo@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Easydags: DAGs made easy
 
 This library heavily inspired this package: https://github.com/mindee/tawazi, and a little bit by Airflow.
 
 
 ## Easy install using pypi
 You can easily install this in a separate conda envioronment with the following:
@@ -19,14 +10,22 @@
 conda create -n easydags python=3.10 -y
 conda activate easydags
 pip install easydags
 ```
 
 Now you can run your DAG's on your local envioronment
 
+## Easy learning with some easy tutorials
+
+- Tutorial_ETL_with_doft_dependencies.ipnyb (Data Engineering + soft dependencies)
+- Tutorial_imbalance_gs.ipnyb (Machine learning + hard dependencies)
+- Tutorial_ML toy.ipnyb (Machine learning + hard dependencies)
+
+# Easy understanding of easydags and its features
+
 ## Define a DAG
 
 Maybe all of you already know what a Directed Acyclic Graph (DAG) is..., but please think about this definition when using this library:
 
 
 A DAG represents a collection of tasks you want to run; this is also organized to show relationships between tasks.
 
@@ -854,8 +853,8 @@
 Basically the idea here is that you can create a different conda envioronment for each dag (or just one... do what you need here) and create bash script that:
 
 1. Activate the conda envioronment
 2. Run a python script with your dag
 
 After that you can use cronjobs to schedule your dags (please read how to use crontab -e on linux)
 
-You will need to to make the bash and python script executables with chmod +x {file}
+You will need to to make the bash and python script executables with chmod +x {file}
```

### Comparing `easydags-0.1.2/README.md` & `easydags-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: easydags
+Version: 1.0.0
+Summary: Dags made easy
+Author: Mateo Graciano
+Author-email: magralo@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Easydags: DAGs made easy
 
 This library heavily inspired this package: https://github.com/mindee/tawazi, and a little bit by Airflow.
 
 
 ## Easy install using pypi
 You can easily install this in a separate conda envioronment with the following:
@@ -10,14 +19,22 @@
 conda create -n easydags python=3.10 -y
 conda activate easydags
 pip install easydags
 ```
 
 Now you can run your DAG's on your local envioronment
 
+## Easy learning with some easy tutorials
+
+- Tutorial_ETL_with_doft_dependencies.ipnyb (Data Engineering + soft dependencies)
+- Tutorial_imbalance_gs.ipnyb (Machine learning + hard dependencies)
+- Tutorial_ML toy.ipnyb (Machine learning + hard dependencies)
+
+# Easy understanding of easydags and its features
+
 ## Define a DAG
 
 Maybe all of you already know what a Directed Acyclic Graph (DAG) is..., but please think about this definition when using this library:
 
 
 A DAG represents a collection of tasks you want to run; this is also organized to show relationships between tasks.
 
@@ -845,8 +862,8 @@
 Basically the idea here is that you can create a different conda envioronment for each dag (or just one... do what you need here) and create bash script that:
 
 1. Activate the conda envioronment
 2. Run a python script with your dag
 
 After that you can use cronjobs to schedule your dags (please read how to use crontab -e on linux)
 
-You will need to to make the bash and python script executables with chmod +x {file}
+You will need to to make the bash and python script executables with chmod +x {file}
```

### Comparing `easydags-0.1.2/easydags/dag.py` & `easydags-1.0.0/easydags/dag.py`

 * *Files identical despite different names*

### Comparing `easydags-0.1.2/easydags/node.py` & `easydags-1.0.0/easydags/node.py`

 * *Files identical despite different names*

### Comparing `easydags-0.1.2/easydags/ops.py` & `easydags-1.0.0/easydags/ops.py`

 * *Files identical despite different names*

### Comparing `easydags-0.1.2/easydags.egg-info/PKG-INFO` & `easydags-1.0.0/easydags.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydags
-Version: 0.1.2
+Version: 1.0.0
 Summary: Dags made easy
 Author: Mateo Graciano
 Author-email: magralo@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easydags: DAGs made easy
@@ -19,14 +19,22 @@
 conda create -n easydags python=3.10 -y
 conda activate easydags
 pip install easydags
 ```
 
 Now you can run your DAG's on your local envioronment
 
+## Easy learning with some easy tutorials
+
+- Tutorial_ETL_with_doft_dependencies.ipnyb (Data Engineering + soft dependencies)
+- Tutorial_imbalance_gs.ipnyb (Machine learning + hard dependencies)
+- Tutorial_ML toy.ipnyb (Machine learning + hard dependencies)
+
+# Easy understanding of easydags and its features
+
 ## Define a DAG
 
 Maybe all of you already know what a Directed Acyclic Graph (DAG) is..., but please think about this definition when using this library:
 
 
 A DAG represents a collection of tasks you want to run; this is also organized to show relationships between tasks.
```

### Comparing `easydags-0.1.2/setup.py` & `easydags-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'easydags',         # How you named your package folder (MyLib)
   packages = ['easydags'],   # Chose the same as "name"
-  version = '0.1.2',      # Start with a small number and increase it with every change you make
+  version = '1.0.0',      # Start with a small number and increase it with every change you make
   description = 'Dags made easy',   # Give a short description about your library
   author = 'Mateo Graciano',                   # Type in your name
   author_email = 'magralo@gmail.com',      # Type in your E-Mail
   install_requires=[            # I get to this in a second
           'networkx==2.6.3',
           'pydantic==1.10',
           'loguru==0.6.0',
```

