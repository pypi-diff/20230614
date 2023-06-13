# Comparing `tmp/econbeautylib-0.0.7.tar.gz` & `tmp/econbeautylib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/econbeautylib-0.0.7.tar", last modified: Tue Jun 13 22:59:09 2023, max compression
+gzip compressed data, was "dist/econbeautylib-0.0.8.tar", last modified: Tue Jun 13 23:30:58 2023, max compression
```

## Comparing `econbeautylib-0.0.7.tar` & `econbeautylib-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       69 2023-06-11 21:36:53.000000 econbeautylib-0.0.7/MANIFEST.in
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/PKG-INFO
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.7/README.md
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       28 2023-06-11 21:29:45.000000 econbeautylib-0.0.7/econbeautylib/__init__.py
--rw-r--r--   0 dashka-z (1587325521) 593637566      500 2023-06-13 22:52:10.000000 econbeautylib-0.0.7/econbeautylib/a.py
--rw-r--r--   0 dashka-z (1587325521) 593637566   171876 2023-06-13 22:58:57.000000 econbeautylib-0.0.7/econbeautylib/econstats.py
--rw-r--r--   0 dashka-z (1587325521) 593637566    35090 2023-06-13 22:01:13.000000 econbeautylib-0.0.7/econbeautylib/tasks.docx
--rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.7/econbeautylib/tasks_base.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.7/econbeautylib/upload_task_to_base.py
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/PKG-INFO
--rw-r--r--   0 dashka-z (1587325521) 593637566      387 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/SOURCES.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/dependency_links.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.7/econbeautylib.egg-info/not-zip-safe
--rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/top_level.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/setup.cfg
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-13 22:59:05.000000 econbeautylib-0.0.7/setup.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       69 2023-06-11 21:36:53.000000 econbeautylib-0.0.8/MANIFEST.in
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/PKG-INFO
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.8/README.md
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       28 2023-06-11 21:29:45.000000 econbeautylib-0.0.8/econbeautylib/__init__.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566      500 2023-06-13 22:52:10.000000 econbeautylib-0.0.8/econbeautylib/a.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566   171802 2023-06-13 23:30:29.000000 econbeautylib-0.0.8/econbeautylib/econstats.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566    35090 2023-06-13 22:01:13.000000 econbeautylib-0.0.8/econbeautylib/tasks.docx
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.8/econbeautylib/tasks_base.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.8/econbeautylib/upload_task_to_base.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/PKG-INFO
+-rw-r--r--   0 dashka-z (1587325521) 593637566      387 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/SOURCES.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/dependency_links.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/not-zip-safe
+-rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/econbeautylib.egg-info/top_level.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-13 23:30:58.000000 econbeautylib-0.0.8/setup.cfg
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-13 23:30:56.000000 econbeautylib-0.0.8/setup.py
```

### Comparing `econbeautylib-0.0.7/README.md` & `econbeautylib-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.7/econbeautylib/econstats.py` & `econbeautylib-0.0.8/econbeautylib/econstats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from docx import Document
 import os
 from typing import DefaultDict, List, Optional, Union, Dict, Any
 import string
 import pathlib
 import json
 from PyPDF2 import PdfFileReader
+from IPython.display import IFrame
+import PyPDF2
 from IPython.display import Image
 from IPython.display import display, Markdown
+import fitz
 
 class Task:
     class Fields:
         ID = "id"
         UNIT = "unit"
         TASK_TEXT = "task_text"
         TASK_SOLUTION = "TASK_SOLUTION"
@@ -38,21 +41,23 @@
     print("""https://colab.research.google.com/drive/1-pgJ6hiDrEZxT0J3xTqw53SZmpt0tpD5?ouid=0&usp=drive_open#scrollTo=h4-0bfwhGYBX colab для практики, будьте аккуратны""")
 
 def load_all_tasks():
     path = pathlib.Path(pathlib.Path(os.path.dirname(os.path.abspath(__file__)), "tasks.docx"))
     doc = Document(path)
     all_tasks = DefaultDict(list)
     last_task_id = None
+    cnt = 0
 
     for para in doc.paragraphs:
         if (para.style.name in  ('Heading 1', 'Heading 2')):
             last_task_id = para.text
+            cnt += 1
         else:
-            # print('w:br' in para._element.xml and 'type="page"' in para._element.xml)
-            all_tasks[last_task_id].append(para.text)
+            all_tasks[last_task_id] = cnt
+            
 
 
     tasks = []
 
     with open(pathlib.Path(pathlib.Path(os.path.dirname(os.path.abspath(__file__)), "tasks_base.txt")), encoding="UTF8") as f:
         for row in f:
             tasks.append(Task.deserialize(json.loads(row)))
@@ -2422,22 +2427,20 @@
 
     """))
 
 
 def get_task_by_id(id: int) -> Union[None, str]:
     all_tasks = load_all_tasks()
     for task in all_tasks:
-        # if task.id == id:
-        #     if (task.unit == 'a'):
-        #         eval("task_"+str(id)+"()")
-        #     else:
-        filehandle =  pathlib.Path(pathlib.Path(os.path.dirname(os.path.abspath(__file__)), "tasks.pdf"))
-        pdf = PdfFileReader(filehandle)
-    
-        info = pdf.getDocumentInfo()
-        pages = pdf.getNumPages()
-        # print("Количество страниц в документе: %i\n\n" % pages)
-        # print("Мета-описание: ", info)
-        page = pdf.getPage(0)
+        if task.id == id:
+            if (task.unit == 'a'):
+                eval("task_"+str(id)+"()")
+            else:
+                filehandle=pathlib.Path(pathlib.Path(os.path.dirname(os.path.abspath(__file__)), "tasks.docx"))
+                doc = fitz.open(filehandle)
+                page = doc.load_page(task.task_solution)
+                pix = page.get_pixmap()
+                output = "outfile.png"
+                pix.save(output)
+                doc.close()
+                Image(output)
 
-        fig = Image(filename=(page))
-        display(fig)
```

### Comparing `econbeautylib-0.0.7/econbeautylib/tasks.docx` & `econbeautylib-0.0.8/econbeautylib/tasks.docx`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.7/econbeautylib/tasks_base.txt` & `econbeautylib-0.0.8/econbeautylib/tasks_base.txt`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.7/econbeautylib/upload_task_to_base.py` & `econbeautylib-0.0.8/econbeautylib/upload_task_to_base.py`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.7/setup.py` & `econbeautylib-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @author:
 Зайцева Дарья
 """
 
 from setuptools import setup, find_packages
 long_description = '''Library for the 5 semester'''
 setup(name='econbeautylib',
-      version='0.0.7',
+      version='0.0.8',
       url='https://github.com/dashkazaitseva',
       packages=['econbeautylib'],
       license='MIT',
       description='',
       zip_safe=False,
       package_data={'econbeautylib': ['*.txt', '*.docx']},
       include_package_data=True
```

