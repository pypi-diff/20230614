# Comparing `tmp/FindJobsTW-1.0.5.tar.gz` & `tmp/FindJobsTW-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-1.0.5.tar", last modified: Tue Jun 13 13:46:33 2023, max compression
+gzip compressed data, was "FindJobsTW-1.0.7.tar", last modified: Wed Jun 14 01:33:40 2023, max compression
```

## Comparing `FindJobsTW-1.0.5.tar` & `FindJobsTW-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.297374 FindJobsTW-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.290397 FindJobsTW-1.0.5/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 13:46:33.000000 FindJobsTW-1.0.5/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 16:16:15.000000 FindJobsTW-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       72 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      591 2023-06-13 13:46:33.296377 FindJobsTW-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 16:16:15.000000 FindJobsTW-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.292390 FindJobsTW-1.0.5/findJobs/
--rw-rw-rw-   0        0        0    20125 2023-06-13 13:22:37.000000 FindJobsTW-1.0.5/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0      133 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/findJobs/__init__.py
--rw-rw-rw-   0        0        0     5368 2023-06-13 13:03:17.000000 FindJobsTW-1.0.5/findJobs/app.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.294384 FindJobsTW-1.0.5/findJobs/static/
--rw-rw-rw-   0        0        0  1245103 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/findJobs/static/drake.png
--rw-rw-rw-   0        0        0      382 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/findJobs/static/styles.css
-drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.295380 FindJobsTW-1.0.5/findJobs/static/temp/
--rw-rw-rw-   0        0        0        0 2023-06-13 13:43:36.000000 FindJobsTW-1.0.5/findJobs/static/temp/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-06-13 13:46:33.296377 FindJobsTW-1.0.5/findJobs/templates/
--rw-rw-rw-   0        0        0    29098 2023-06-13 11:41:35.000000 FindJobsTW-1.0.5/findJobs/templates/index.html
--rw-rw-rw-   0        0        0     5064 2023-06-13 13:34:51.000000 FindJobsTW-1.0.5/findJobs/url.py
--rw-rw-rw-   0        0        0       42 2023-06-13 13:46:33.297374 FindJobsTW-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-06-13 13:44:27.000000 FindJobsTW-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:40.116384 FindJobsTW-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:40.068382 FindJobsTW-1.0.7/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      763 2023-06-14 01:33:39.000000 FindJobsTW-1.0.7/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-06-14 01:33:39.000000 FindJobsTW-1.0.7/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 01:33:39.000000 FindJobsTW-1.0.7/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-14 01:33:39.000000 FindJobsTW-1.0.7/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 01:33:39.000000 FindJobsTW-1.0.7/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-06-12 09:32:38.000000 FindJobsTW-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      763 2023-06-14 01:33:40.108383 FindJobsTW-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-14 01:31:50.000000 FindJobsTW-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:40.084385 FindJobsTW-1.0.7/findJobs/
+-rw-rw-rw-   0        0        0    20368 2023-06-14 01:24:44.000000 FindJobsTW-1.0.7/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0     1288 2023-06-14 01:25:55.000000 FindJobsTW-1.0.7/findJobs/__init__.py
+-rw-rw-rw-   0        0        0     5368 2023-06-14 01:12:47.000000 FindJobsTW-1.0.7/findJobs/app.py
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:40.092387 FindJobsTW-1.0.7/findJobs/static/
+-rw-rw-rw-   0        0        0  1245103 2023-06-08 05:24:31.000000 FindJobsTW-1.0.7/findJobs/static/drake.png
+-rw-rw-rw-   0        0        0      382 2023-06-12 08:30:14.000000 FindJobsTW-1.0.7/findJobs/static/styles.css
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:40.100390 FindJobsTW-1.0.7/findJobs/static/temp/
+-rw-rw-rw-   0        0        0    32029 2023-06-14 01:27:44.000000 FindJobsTW-1.0.7/findJobs/static/temp/salary_boxplot.png
+-rw-rw-rw-   0        0        0    35422 2023-06-14 01:27:45.000000 FindJobsTW-1.0.7/findJobs/static/temp/salary_density.png
+drwxrwxrwx   0        0        0        0 2023-06-14 01:33:40.108383 FindJobsTW-1.0.7/findJobs/templates/
+-rw-rw-rw-   0        0        0    29098 2023-06-13 03:43:41.000000 FindJobsTW-1.0.7/findJobs/templates/index.html
+-rw-rw-rw-   0        0        0     5064 2023-06-14 01:12:47.000000 FindJobsTW-1.0.7/findJobs/url.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 01:33:40.116384 FindJobsTW-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-06-14 01:32:34.000000 FindJobsTW-1.0.7/setup.py
```

### Comparing `FindJobsTW-1.0.5/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-1.0.7/FindJobsTW.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.5
+Version: 1.0.7
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,7 +12,16 @@
 License-File: LICENSE
 
 # FindJobsTW
 A Python package to find jobs on 104.com.tw based on specific keywords.
 Co Author:
 
 祝您找到好工作!
+
+
+
+
+Co-Author:
+Dean  dannyfinselect@outlook.com
+Yuzhen kauyu520@gmail.com
+YangFC yangchia10@gmail.com
+Chen Tingen t.e.sfreiheit@gmail.com, github.com/chen-ting-en
```

### Comparing `FindJobsTW-1.0.5/LICENSE` & `FindJobsTW-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.5/PKG-INFO` & `FindJobsTW-1.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.5
+Version: 1.0.7
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,7 +12,16 @@
 License-File: LICENSE
 
 # FindJobsTW
 A Python package to find jobs on 104.com.tw based on specific keywords.
 Co Author:
 
 祝您找到好工作!
+
+
+
+
+Co-Author:
+Dean  dannyfinselect@outlook.com
+Yuzhen kauyu520@gmail.com
+YangFC yangchia10@gmail.com
+Chen Tingen t.e.sfreiheit@gmail.com, github.com/chen-ting-en
```

### Comparing `FindJobsTW-1.0.5/findJobs/FindJobs.py` & `FindJobsTW-1.0.7/findJobs/FindJobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,24 +376,30 @@
     def get_static_temp_path(self):
         # 獲取當前檔案的目錄
         current_dir = os.path.dirname(os.path.realpath(__file__))
 
         # 往上一層一層地搜尋，直到找到包含 'findJobs' 或 'FindJobsTW' 的路徑
         while current_dir != os.path.sep:
             if 'findJobs' in current_dir or 'FindJobsTW' in current_dir:
-                return os.path.relpath(os.path.join(current_dir, 'static/temp'))
+                target_dir = os.path.relpath(os.path.join(current_dir, 'static/temp'))
+                
+                # 檢查目標資料夾是否存在，若不存在則建立新的資料夾
+                if not os.path.exists(target_dir):
+                    os.makedirs(target_dir)
+
+                return target_dir
             current_dir = os.path.dirname(current_dir)
     
     def help(self):
         print("在瀏覽器中執行請參考下列代碼:")
         print()
         text1 = '''
             from threading import Timer
             import webbrowser
-            from findJobs import create_app, hlep
+            from findJobs import create_app
 
             def open_browser():
                 webbrowser.open_new('http://127.0.0.1:5000/')
 
             app = create_app()
 
             if __name__ == '__main__':
@@ -418,20 +424,20 @@
             #若要快速關閉視窗可按ctrl+w
             '''
         print(text2)
         print()
 
     
 if __name__ == "__main__":
-    a = Jobs("111")
-    a.help()
+    #a = Jobs("111")
+    #a.help()
     #print(os.path.relpath(a.get_static_temp_path()))
-''' keyword = "分析師"
+    keyword = "分析師"
     jobs = Jobs(keyword)
     jobs.search_links(max_pages = 1)#一頁是20個職缺
     jobs.find_jobs(max_jobs = 10)
     jobs.save_jobs()
     jobs.draw_box(show = False)
     jobs.draw_density(show = False)
     #jobs.show("all") #一次秀出全部
     jobs.show("職務類別")
-    #help()'''
+    #help()
```

### Comparing `FindJobsTW-1.0.5/findJobs/app.py` & `FindJobsTW-1.0.7/findJobs/app.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.5/findJobs/static/drake.png` & `FindJobsTW-1.0.7/findJobs/static/drake.png`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.5/findJobs/templates/index.html` & `FindJobsTW-1.0.7/findJobs/templates/index.html`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.5/findJobs/url.py` & `FindJobsTW-1.0.7/findJobs/url.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.5/setup.py` & `FindJobsTW-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='1.0.5',      
+    version='1.0.7',      
     packages=find_packages(),    
     install_requires=requirements,
     package_data={
         'findJobs': ['templates/*', 'static/*', 'static/temp/*']
     },  
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
```

