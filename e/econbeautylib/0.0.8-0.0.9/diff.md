# Comparing `tmp/econbeautylib-0.0.8.tar.gz` & `tmp/econbeautylib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/econbeautylib-0.0.8.tar", last modified: Tue Jun 13 23:30:58 2023, max compression
+gzip compressed data, was "dist/econbeautylib-0.0.9.tar", last modified: Tue Jun 13 23:37:09 2023, max compression
```

## Comparing `econbeautylib-0.0.8.tar` & `econbeautylib-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       69 2023-06-11 21:36:53.000000 econbeautylib-0.0.8/MANIFEST.in
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/PKG-INFO
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.8/README.md
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       28 2023-06-11 21:29:45.000000 econbeautylib-0.0.8/econbeautylib/__init__.py
--rw-r--r--   0 dashka-z (1587325521) 593637566      500 2023-06-13 22:52:10.000000 econbeautylib-0.0.8/econbeautylib/a.py
--rw-r--r--   0 dashka-z (1587325521) 593637566   171802 2023-06-13 23:30:29.000000 econbeautylib-0.0.8/econbeautylib/econstats.py
--rw-r--r--   0 dashka-z (1587325521) 593637566    35090 2023-06-13 22:01:13.000000 econbeautylib-0.0.8/econbeautylib/tasks.docx
--rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.8/econbeautylib/tasks_base.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.8/econbeautylib/upload_task_to_base.py
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/PKG-INFO
--rw-r--r--   0 dashka-z (1587325521) 593637566      387 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/SOURCES.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/dependency_links.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/not-zip-safe
--rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/top_level.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/setup.cfg
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-13 23:30:56.000000 econbeautylib-0.0.8/setup.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 23:37:09.000000 econbeautylib-0.0.9/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       69 2023-06-11 21:36:53.000000 econbeautylib-0.0.9/MANIFEST.in
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 23:37:09.000000 econbeautylib-0.0.9/PKG-INFO
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.9/README.md
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 23:37:09.000000 econbeautylib-0.0.9/econbeautylib/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       28 2023-06-11 21:29:45.000000 econbeautylib-0.0.9/econbeautylib/__init__.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566      500 2023-06-13 22:52:10.000000 econbeautylib-0.0.9/econbeautylib/a.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566   171801 2023-06-13 23:36:51.000000 econbeautylib-0.0.9/econbeautylib/econstats.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566    35090 2023-06-13 22:01:13.000000 econbeautylib-0.0.9/econbeautylib/tasks.docx
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.9/econbeautylib/tasks_base.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.9/econbeautylib/upload_task_to_base.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 23:37:09.000000 econbeautylib-0.0.9/econbeautylib.egg-info/
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 23:37:09.000000 econbeautylib-0.0.9/econbeautylib.egg-info/PKG-INFO
+-rw-r--r--   0 dashka-z (1587325521) 593637566      387 2023-06-13 23:37:09.000000 econbeautylib-0.0.9/econbeautylib.egg-info/SOURCES.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-13 23:37:09.000000 econbeautylib-0.0.9/econbeautylib.egg-info/dependency_links.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.9/econbeautylib.egg-info/not-zip-safe
+-rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-13 23:37:09.000000 econbeautylib-0.0.9/econbeautylib.egg-info/top_level.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-13 23:37:09.000000 econbeautylib-0.0.9/setup.cfg
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-13 23:37:07.000000 econbeautylib-0.0.9/setup.py
```

### Comparing `econbeautylib-0.0.8/README.md` & `econbeautylib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.8/econbeautylib/econstats.py` & `econbeautylib-0.0.9/econbeautylib/econstats.py`

 * *Files 0% similar despite different names*

```diff
@@ -2431,15 +2431,15 @@
 def get_task_by_id(id: int) -> Union[None, str]:
     all_tasks = load_all_tasks()
     for task in all_tasks:
         if task.id == id:
             if (task.unit == 'a'):
                 eval("task_"+str(id)+"()")
             else:
-                filehandle=pathlib.Path(pathlib.Path(os.path.dirname(os.path.abspath(__file__)), "tasks.docx"))
+                filehandle=pathlib.Path(pathlib.Path(os.path.dirname(os.path.abspath(__file__)), "tasks.pdf"))
                 doc = fitz.open(filehandle)
                 page = doc.load_page(task.task_solution)
                 pix = page.get_pixmap()
                 output = "outfile.png"
                 pix.save(output)
                 doc.close()
                 Image(output)
```

### Comparing `econbeautylib-0.0.8/econbeautylib/tasks.docx` & `econbeautylib-0.0.9/econbeautylib/tasks.docx`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.8/econbeautylib/tasks_base.txt` & `econbeautylib-0.0.9/econbeautylib/tasks_base.txt`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.8/econbeautylib/upload_task_to_base.py` & `econbeautylib-0.0.9/econbeautylib/upload_task_to_base.py`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.8/setup.py` & `econbeautylib-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @author:
 Зайцева Дарья
 """
 
 from setuptools import setup, find_packages
 long_description = '''Library for the 5 semester'''
 setup(name='econbeautylib',
-      version='0.0.8',
+      version='0.0.9',
       url='https://github.com/dashkazaitseva',
       packages=['econbeautylib'],
       license='MIT',
       description='',
       zip_safe=False,
       package_data={'econbeautylib': ['*.txt', '*.docx']},
       include_package_data=True
```

