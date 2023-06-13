# Comparing `tmp/econbeautylib-0.0.6.tar.gz` & `tmp/econbeautylib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/econbeautylib-0.0.6.tar", last modified: Tue Jun 13 22:53:47 2023, max compression
+gzip compressed data, was "dist/econbeautylib-0.0.7.tar", last modified: Tue Jun 13 22:59:09 2023, max compression
```

## Comparing `econbeautylib-0.0.6.tar` & `econbeautylib-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 22:53:47.000000 econbeautylib-0.0.6/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       69 2023-06-11 21:36:53.000000 econbeautylib-0.0.6/MANIFEST.in
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 22:53:47.000000 econbeautylib-0.0.6/PKG-INFO
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.6/README.md
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 22:53:47.000000 econbeautylib-0.0.6/econbeautylib/
--rw-rw-rw-   0 dashka-z (1587325521) 593637566       28 2023-06-11 21:29:45.000000 econbeautylib-0.0.6/econbeautylib/__init__.py
--rw-r--r--   0 dashka-z (1587325521) 593637566      500 2023-06-13 22:52:10.000000 econbeautylib-0.0.6/econbeautylib/a.py
--rw-r--r--   0 dashka-z (1587325521) 593637566   171985 2023-06-13 22:51:19.000000 econbeautylib-0.0.6/econbeautylib/econstats.py
--rw-r--r--   0 dashka-z (1587325521) 593637566    35090 2023-06-13 22:01:13.000000 econbeautylib-0.0.6/econbeautylib/tasks.docx
--rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.6/econbeautylib/tasks_base.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.6/econbeautylib/upload_task_to_base.py
-drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 22:53:47.000000 econbeautylib-0.0.6/econbeautylib.egg-info/
--rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 22:53:47.000000 econbeautylib-0.0.6/econbeautylib.egg-info/PKG-INFO
--rw-r--r--   0 dashka-z (1587325521) 593637566      387 2023-06-13 22:53:47.000000 econbeautylib-0.0.6/econbeautylib.egg-info/SOURCES.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-13 22:53:47.000000 econbeautylib-0.0.6/econbeautylib.egg-info/dependency_links.txt
--rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.6/econbeautylib.egg-info/not-zip-safe
--rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-13 22:53:47.000000 econbeautylib-0.0.6/econbeautylib.egg-info/top_level.txt
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-13 22:53:47.000000 econbeautylib-0.0.6/setup.cfg
--rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-13 22:53:22.000000 econbeautylib-0.0.6/setup.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       69 2023-06-11 21:36:53.000000 econbeautylib-0.0.7/MANIFEST.in
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/PKG-INFO
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      887 2022-08-30 12:31:51.000000 econbeautylib-0.0.7/README.md
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib/
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566       28 2023-06-11 21:29:45.000000 econbeautylib-0.0.7/econbeautylib/__init__.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566      500 2023-06-13 22:52:10.000000 econbeautylib-0.0.7/econbeautylib/a.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566   171876 2023-06-13 22:58:57.000000 econbeautylib-0.0.7/econbeautylib/econstats.py
+-rw-r--r--   0 dashka-z (1587325521) 593637566    35090 2023-06-13 22:01:13.000000 econbeautylib-0.0.7/econbeautylib/tasks.docx
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566    34476 2023-06-11 21:05:32.000000 econbeautylib-0.0.7/econbeautylib/tasks_base.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566     2014 2023-06-11 21:25:49.000000 econbeautylib-0.0.7/econbeautylib/upload_task_to_base.py
+drwxr-xr-x   0 dashka-z (1587325521) 593637566        0 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/
+-rw-r--r--   0 dashka-z (1587325521) 593637566      209 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/PKG-INFO
+-rw-r--r--   0 dashka-z (1587325521) 593637566      387 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/SOURCES.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/dependency_links.txt
+-rw-r--r--   0 dashka-z (1587325521) 593637566        1 2023-06-11 21:25:58.000000 econbeautylib-0.0.7/econbeautylib.egg-info/not-zip-safe
+-rw-r--r--   0 dashka-z (1587325521) 593637566       14 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/econbeautylib.egg-info/top_level.txt
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      105 2023-06-13 22:59:09.000000 econbeautylib-0.0.7/setup.cfg
+-rw-rw-rw-   0 dashka-z (1587325521) 593637566      513 2023-06-13 22:59:05.000000 econbeautylib-0.0.7/setup.py
```

### Comparing `econbeautylib-0.0.6/README.md` & `econbeautylib-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.6/econbeautylib/econstats.py` & `econbeautylib-0.0.7/econbeautylib/econstats.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     all_tasks = DefaultDict(list)
     last_task_id = None
 
     for para in doc.paragraphs:
         if (para.style.name in  ('Heading 1', 'Heading 2')):
             last_task_id = para.text
         else:
-            print('w:br' in para._element.xml and 'type="page"' in para._element.xml)
+            # print('w:br' in para._element.xml and 'type="page"' in para._element.xml)
             all_tasks[last_task_id].append(para.text)
 
 
     tasks = []
 
     with open(pathlib.Path(pathlib.Path(os.path.dirname(os.path.abspath(__file__)), "tasks_base.txt")), encoding="UTF8") as f:
         for row in f:
@@ -2426,18 +2426,18 @@
 def get_task_by_id(id: int) -> Union[None, str]:
     all_tasks = load_all_tasks()
     for task in all_tasks:
         # if task.id == id:
         #     if (task.unit == 'a'):
         #         eval("task_"+str(id)+"()")
         #     else:
-                pdf = PdfFileReader(filehandle)
-                info = pdf.getDocumentInfo()
-                pages = pdf.getNumPages()
-                print("Количество страниц в документе: %i\n\n" % pages)
-                print("Мета-описание: ", info)
-                for i in range(pages):
-                    page = pdf.getPage(i)
-                    print("Стр.", i, " мета: ", page, "\n\nСодержание;\n")
-                    print(page.extractText().encode('latin').decode('windows-1251'))
+        filehandle =  pathlib.Path(pathlib.Path(os.path.dirname(os.path.abspath(__file__)), "tasks.pdf"))
+        pdf = PdfFileReader(filehandle)
+    
+        info = pdf.getDocumentInfo()
+        pages = pdf.getNumPages()
+        # print("Количество страниц в документе: %i\n\n" % pages)
+        # print("Мета-описание: ", info)
+        page = pdf.getPage(0)
 
-load_all_tasks()
+        fig = Image(filename=(page))
+        display(fig)
```

### Comparing `econbeautylib-0.0.6/econbeautylib/tasks.docx` & `econbeautylib-0.0.7/econbeautylib/tasks.docx`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.6/econbeautylib/tasks_base.txt` & `econbeautylib-0.0.7/econbeautylib/tasks_base.txt`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.6/econbeautylib/upload_task_to_base.py` & `econbeautylib-0.0.7/econbeautylib/upload_task_to_base.py`

 * *Files identical despite different names*

### Comparing `econbeautylib-0.0.6/setup.py` & `econbeautylib-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @author:
 Зайцева Дарья
 """
 
 from setuptools import setup, find_packages
 long_description = '''Library for the 5 semester'''
 setup(name='econbeautylib',
-      version='0.0.6',
+      version='0.0.7',
       url='https://github.com/dashkazaitseva',
       packages=['econbeautylib'],
       license='MIT',
       description='',
       zip_safe=False,
       package_data={'econbeautylib': ['*.txt', '*.docx']},
       include_package_data=True
```

