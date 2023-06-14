# Comparing `tmp/ftrack-ams-2.0.8.tar.gz` & `tmp/ftrack-ams-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack-ams-2.0.8.tar", max compression
+gzip compressed data, was "ftrack-ams-2.0.9.tar", max compression
```

## Comparing `ftrack-ams-2.0.8.tar` & `ftrack-ams-2.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1235 2022-02-02 11:31:25.293484 ftrack-ams-2.0.8/LICENSE
--rw-r--r--   0        0        0      848 2023-02-01 15:15:32.879006 ftrack-ams-2.0.8/pyproject.toml
--rw-r--r--   0        0        0       23 2022-02-08 11:55:16.998285 ftrack-ams-2.0.8/src/ftrack_ams/__init__.py
--rw-r--r--   0        0        0    10213 2023-02-01 15:15:26.720625 ftrack-ams-2.0.8/src/ftrack_ams/add.py
--rw-r--r--   0        0        0     1152 2022-04-06 08:15:13.140610 ftrack-ams-2.0.8/src/ftrack_ams/console.py
--rw-r--r--   0        0        0     2623 2022-08-04 12:42:20.387536 ftrack-ams-2.0.8/src/ftrack_ams/fileserver.py
--rw-r--r--   0        0        0     1600 2023-02-01 14:58:01.596861 ftrack-ams-2.0.8/src/ftrack_ams/functions.py
--rw-r--r--   0        0        0    14006 2023-01-30 10:31:47.148109 ftrack-ams-2.0.8/src/ftrack_ams/main.py
--rw-r--r--   0        0        0      138 2023-01-12 08:52:14.614652 ftrack-ams-2.0.8/src/ftrack_ams/test.py
--rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 ftrack-ams-2.0.8/setup.py
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 ftrack-ams-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1235 2022-02-02 11:31:25.293484 ftrack-ams-2.0.9/LICENSE
+-rw-r--r--   0        0        0      848 2023-02-01 15:18:14.355304 ftrack-ams-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:55:16.998285 ftrack-ams-2.0.9/src/ftrack_ams/__init__.py
+-rw-r--r--   0        0        0    10224 2023-02-01 15:17:58.889770 ftrack-ams-2.0.9/src/ftrack_ams/add.py
+-rw-r--r--   0        0        0     1152 2022-04-06 08:15:13.140610 ftrack-ams-2.0.9/src/ftrack_ams/console.py
+-rw-r--r--   0        0        0     2623 2022-08-04 12:42:20.387536 ftrack-ams-2.0.9/src/ftrack_ams/fileserver.py
+-rw-r--r--   0        0        0     1600 2023-02-01 14:58:01.596861 ftrack-ams-2.0.9/src/ftrack_ams/functions.py
+-rw-r--r--   0        0        0    14006 2023-01-30 10:31:47.148109 ftrack-ams-2.0.9/src/ftrack_ams/main.py
+-rw-r--r--   0        0        0      138 2023-01-12 08:52:14.614652 ftrack-ams-2.0.9/src/ftrack_ams/test.py
+-rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 ftrack-ams-2.0.9/setup.py
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 ftrack-ams-2.0.9/PKG-INFO
```

### Comparing `ftrack-ams-2.0.8/LICENSE` & `ftrack-ams-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ftrack-ams-2.0.8/pyproject.toml` & `ftrack-ams-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-ams"
-version = "2.0.8"
+version = "2.0.9"
 description = ""
 authors = ["Lucas Selfslagh <lucas@animotions.be>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
 click = "^8.0.3"
 pick = "^1.2.0"
```

### Comparing `ftrack-ams-2.0.8/src/ftrack_ams/add.py` & `ftrack-ams-2.0.9/src/ftrack_ams/add.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,15 @@
         if interior_shots is not None and len(interior_shots) > 0:
             int_folder = interior_shots[0]
             num_exist_int = len(int_folder["children"])
             print(f'{existing_project["name"]} already has {num_exist_int} INT images')
 
         while True:
             try:
-                additional_ints = int(
-                    input(f"Enter amount of additional INT images: "))
+                additional_ints = int(input("Enter amount of additional INT images: "))
             except ValueError:
                 print("Sorry, I didn't understand that? Did you type a number?")
                 continue
             else:
                 print(f"Number of addtional INT:{additional_ints}")
                 break
 
@@ -78,14 +77,15 @@
                     f"{existing_project['name']} has no INT images, let's create a folder for them!")
                 int_folder = session.create(
                     "Folder",
                     {
                         "name": f"{projnumber}_INT",
                         "parent": existing_project
                     })
+                session.commit()
 
         exterior_shots = [i for i in existing_project['children'] if "EXT" in i["name"]]
         num_existing_ext = 0
         ext_folder = None
         if exterior_shots is not None and len(exterior_shots) > 0:
             ext_folder = exterior_shots[0]
             num_existing_ext = len(ext_folder["children"])
```

### Comparing `ftrack-ams-2.0.8/src/ftrack_ams/console.py` & `ftrack-ams-2.0.9/src/ftrack_ams/console.py`

 * *Files identical despite different names*

### Comparing `ftrack-ams-2.0.8/src/ftrack_ams/fileserver.py` & `ftrack-ams-2.0.9/src/ftrack_ams/fileserver.py`

 * *Files identical despite different names*

### Comparing `ftrack-ams-2.0.8/src/ftrack_ams/functions.py` & `ftrack-ams-2.0.9/src/ftrack_ams/functions.py`

 * *Files identical despite different names*

### Comparing `ftrack-ams-2.0.8/src/ftrack_ams/main.py` & `ftrack-ams-2.0.9/src/ftrack_ams/main.py`

 * *Files identical despite different names*

### Comparing `ftrack-ams-2.0.8/setup.py` & `ftrack-ams-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['click>=8.0.3,<9.0.0', 'ftrack-python-api>=2.3.1,<3.0.0', 'pick>=1.2.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ftrack-ams = ftrack_ams.console:main']}
 
 setup_kwargs = {
     'name': 'ftrack-ams',
-    'version': '2.0.8',
+    'version': '2.0.9',
     'description': '',
     'long_description': 'None',
     'author': 'Lucas Selfslagh',
     'author_email': 'lucas@animotions.be',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

