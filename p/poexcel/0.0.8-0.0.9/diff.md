# Comparing `tmp/poexcel-0.0.8.tar.gz` & `tmp/poexcel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poexcel-0.0.8.tar", last modified: Thu Mar 23 16:02:43 2023, max compression
+gzip compressed data, was "poexcel-0.0.9.tar", last modified: Fri Mar 24 14:26:03 2023, max compression
```

## Comparing `poexcel-0.0.8.tar` & `poexcel-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:43.390019 poexcel-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poexcel-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5265 2023-03-23 16:02:43.390019 poexcel-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4730 2023-03-22 12:35:51.000000 poexcel-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:43.341585 poexcel-0.0.8/poexcel/
--rw-rw-rw-   0        0        0       33 2022-09-17 07:20:49.000000 poexcel-0.0.8/poexcel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:43.363013 poexcel-0.0.8/poexcel/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poexcel-0.0.8/poexcel/api/__init__.py
--rw-rw-rw-   0        0        0     2071 2023-03-23 15:57:04.000000 poexcel-0.0.8/poexcel/api/excel.py
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:43.373010 poexcel-0.0.8/poexcel/core/
--rw-rw-rw-   0        0        0     6925 2023-03-22 12:49:01.000000 poexcel-0.0.8/poexcel/core/ExcelType.py
--rw-rw-rw-   0        0        0     2358 2023-03-23 16:02:40.000000 poexcel-0.0.8/poexcel/core/QueryExcel.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poexcel-0.0.8/poexcel/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:43.377016 poexcel-0.0.8/poexcel/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poexcel-0.0.8/poexcel/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:43.384025 poexcel-0.0.8/poexcel/lib/excel/
--rw-rw-rw-   0        0        0     3910 2022-09-17 07:45:13.000000 poexcel-0.0.8/poexcel/lib/excel/SplitExcel.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poexcel-0.0.8/poexcel/lib/excel/__init__.py
--rw-rw-rw-   0        0        0     1472 2022-09-01 13:34:44.000000 poexcel-0.0.8/poexcel/lib/pandas_mem.py
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:43.358585 poexcel-0.0.8/poexcel.egg-info/
--rw-rw-rw-   0        0        0     5265 2023-03-23 16:02:43.000000 poexcel-0.0.8/poexcel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2023-03-23 16:02:43.000000 poexcel-0.0.8/poexcel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 16:02:43.000000 poexcel-0.0.8/poexcel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 12:38:46.000000 poexcel-0.0.8/poexcel.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       66 2023-03-23 16:02:43.000000 poexcel-0.0.8/poexcel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-23 16:02:43.000000 poexcel-0.0.8/poexcel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      780 2023-03-23 16:02:43.391099 poexcel-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poexcel-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:43.388008 poexcel-0.0.8/tests/
--rw-rw-rw-   0        0        0      183 2022-09-17 07:20:49.000000 poexcel-0.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0     2563 2023-03-23 15:57:41.000000 poexcel-0.0.8/tests/test_excel.py
+drwxrwxrwx   0        0        0        0 2023-03-24 14:26:03.613825 poexcel-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poexcel-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5265 2023-03-24 14:26:03.613825 poexcel-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4730 2023-03-22 12:35:51.000000 poexcel-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-24 14:26:03.501365 poexcel-0.0.9/poexcel/
+-rw-rw-rw-   0        0        0       33 2022-09-17 07:20:49.000000 poexcel-0.0.9/poexcel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-24 14:26:03.550222 poexcel-0.0.9/poexcel/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poexcel-0.0.9/poexcel/api/__init__.py
+-rw-rw-rw-   0        0        0     2071 2023-03-23 15:57:04.000000 poexcel-0.0.9/poexcel/api/excel.py
+drwxrwxrwx   0        0        0        0 2023-03-24 14:26:03.569261 poexcel-0.0.9/poexcel/core/
+-rw-rw-rw-   0        0        0     6925 2023-03-22 12:49:01.000000 poexcel-0.0.9/poexcel/core/ExcelType.py
+-rw-rw-rw-   0        0        0     2468 2023-03-24 14:00:10.000000 poexcel-0.0.9/poexcel/core/QueryExcel.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poexcel-0.0.9/poexcel/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-24 14:26:03.583511 poexcel-0.0.9/poexcel/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poexcel-0.0.9/poexcel/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-24 14:26:03.598573 poexcel-0.0.9/poexcel/lib/excel/
+-rw-rw-rw-   0        0        0     3910 2022-09-17 07:45:13.000000 poexcel-0.0.9/poexcel/lib/excel/SplitExcel.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poexcel-0.0.9/poexcel/lib/excel/__init__.py
+-rw-rw-rw-   0        0        0     1472 2022-09-01 13:34:44.000000 poexcel-0.0.9/poexcel/lib/pandas_mem.py
+drwxrwxrwx   0        0        0        0 2023-03-24 14:26:03.537042 poexcel-0.0.9/poexcel.egg-info/
+-rw-rw-rw-   0        0        0     5265 2023-03-24 14:26:03.000000 poexcel-0.0.9/poexcel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2023-03-24 14:26:03.000000 poexcel-0.0.9/poexcel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-24 14:26:03.000000 poexcel-0.0.9/poexcel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-22 12:38:46.000000 poexcel-0.0.9/poexcel.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       66 2023-03-24 14:26:03.000000 poexcel-0.0.9/poexcel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-03-24 14:26:03.000000 poexcel-0.0.9/poexcel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      780 2023-03-24 14:26:03.616825 poexcel-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poexcel-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-24 14:26:03.610829 poexcel-0.0.9/tests/
+-rw-rw-rw-   0        0        0      183 2022-09-17 07:20:49.000000 poexcel-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     2587 2023-03-24 13:58:29.000000 poexcel-0.0.9/tests/test_excel.py
```

### Comparing `poexcel-0.0.8/LICENSE` & `poexcel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `poexcel-0.0.8/PKG-INFO` & `poexcel-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poexcel
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poexcel
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poexcel/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poexcel/blob/master/README.md
```

### Comparing `poexcel-0.0.8/README.md` & `poexcel-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `poexcel-0.0.8/poexcel/api/excel.py` & `poexcel-0.0.9/poexcel/api/excel.py`

 * *Files identical despite different names*

### Comparing `poexcel-0.0.8/poexcel/core/ExcelType.py` & `poexcel-0.0.9/poexcel/core/ExcelType.py`

 * *Files identical despite different names*

### Comparing `poexcel-0.0.8/poexcel/core/QueryExcel.py` & `poexcel-0.0.9/poexcel/core/QueryExcel.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,12 +44,14 @@
     for excel in simple_progress(waiting_query_excel_files, desc='正在搜索Excel中符合条件的数据：'):
         df = pd.read_excel(excel, sheet_name=None, header=None)
         for sheet in df.values():
             for i, current_row in enumerate(sheet.itertuples()):
                 # if i == 0:
                 #     print(sheet.iloc[i].to_dict())
                 if query_content in current_row:
-                    current_row_df = pd.DataFrame(sheet.iloc[i].to_dict(), index=[0])
+                    file_dict = {"文件位置":str(excel)}
+                    file_dict.update(sheet.iloc[i].to_dict())
+                    current_row_df = pd.DataFrame(file_dict, index=[0])
                     res_df = res_df.append(current_row_df)
                     # print()
     # print(res_df)
     res_df.to_excel(str(abs_output_path),index=False)
```

### Comparing `poexcel-0.0.8/poexcel/lib/excel/SplitExcel.py` & `poexcel-0.0.9/poexcel/lib/excel/SplitExcel.py`

 * *Files identical despite different names*

### Comparing `poexcel-0.0.8/poexcel/lib/pandas_mem.py` & `poexcel-0.0.9/poexcel/lib/pandas_mem.py`

 * *Files identical despite different names*

### Comparing `poexcel-0.0.8/poexcel.egg-info/PKG-INFO` & `poexcel-0.0.9/poexcel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poexcel
-Version: 0.0.8
+Version: 0.0.9
 Summary: pip install poexcel
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poexcel/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poexcel/blob/master/README.md
```

### Comparing `poexcel-0.0.8/poexcel.egg-info/SOURCES.txt` & `poexcel-0.0.9/poexcel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `poexcel-0.0.8/setup.cfg` & `poexcel-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f65 7863 656c 0d0a 7665 7273   = poexcel..vers
-00000020: 696f 6e20 3d20 302e 302e 380d 0a64 6573  ion = 0.0.8..des
+00000020: 696f 6e20 3d20 302e 302e 390d 0a64 6573  ion = 0.0.9..des
 00000030: 6372 6970 7469 6f6e 203d 2070 6970 2069  cription = pip i
 00000040: 6e73 7461 6c6c 2070 6f65 7863 656c 0d0a  nstall poexcel..
 00000050: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000060: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000070: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 00000080: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
 00000090: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
```

### Comparing `poexcel-0.0.8/tests/test_excel.py` & `poexcel-0.0.9/tests/test_excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         merge2excel(dir_path=r'../../contributors/bulabean', output_file='test_merge2excel.xlsx', )
 
     def test_find_excel_data(self):
         find_excel_data(search_key='刘家站垦殖场', target_dir=r'../../contributors/bulabean')
 
     def test_query4excel(self):
         # query4excel(query_content='程序员晚枫', query_path=r'D:\test\py310\excel_test')
-        query4excel(query_content='程序员晚枫', query_path=r'D:\test',output_path=r'D:\test\py310\excel_test\output_path',output_name='晚枫.xlsx')
+        query4excel(query_content='程序员晚枫', query_path=r'D:\test\py310\excel_test\course',output_path=r'D:\test\py310\excel_test\output_path',output_name='晚枫.xlsx')
 
     # def test_merge2sheet(self):
     #     """
     #     https://blog.csdn.net/xue_11/article/details/118424380
     #     https://www.jb51.net/article/214868.htm
     #     """
     #     dir_path = 'test_files/excel'
```

