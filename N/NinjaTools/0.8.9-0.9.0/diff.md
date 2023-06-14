# Comparing `tmp/NinjaTools-0.8.9.tar.gz` & `tmp/NinjaTools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NinjaTools-0.8.9.tar", last modified: Tue Oct 11 12:50:24 2022, max compression
+gzip compressed data, was "NinjaTools-0.9.0.tar", last modified: Thu Nov  3 02:43:39 2022, max compression
```

## Comparing `NinjaTools-0.8.9.tar` & `NinjaTools-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-10-11 12:50:24.447614 NinjaTools-0.8.9/
-drwxrwxrwx   0        0        0        0 2022-10-11 12:50:24.439614 NinjaTools-0.8.9/NinjaTools.egg-info/
--rw-rw-rw-   0        0        0      621 2022-10-11 12:50:24.000000 NinjaTools-0.8.9/NinjaTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2022-10-11 12:50:24.000000 NinjaTools-0.8.9/NinjaTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-11 12:50:24.000000 NinjaTools-0.8.9/NinjaTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      286 2022-10-11 12:50:24.000000 NinjaTools-0.8.9/NinjaTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-10-11 12:50:24.000000 NinjaTools-0.8.9/NinjaTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      621 2022-10-11 12:50:24.446615 NinjaTools-0.8.9/PKG-INFO
--rw-rw-rw-   0        0        0       11 2022-03-10 21:15:41.000000 NinjaTools-0.8.9/README.md
-drwxrwxrwx   0        0        0        0 2022-10-11 12:50:24.446615 NinjaTools-0.8.9/ninja_tools/
--rw-rw-rw-   0        0        0        0 2022-03-10 21:19:30.000000 NinjaTools-0.8.9/ninja_tools/__init__.py
--rw-rw-rw-   0        0        0      545 2022-03-08 20:04:20.000000 NinjaTools-0.8.9/ninja_tools/bbox.py
--rw-rw-rw-   0        0        0     5943 2022-10-11 12:50:07.000000 NinjaTools-0.8.9/ninja_tools/excel.py
--rw-rw-rw-   0        0        0     2425 2022-03-23 15:11:16.000000 NinjaTools-0.8.9/ninja_tools/find_image.py
--rw-rw-rw-   0        0        0     2406 2022-03-23 15:11:16.000000 NinjaTools-0.8.9/ninja_tools/image_cropper.py
--rw-rw-rw-   0        0        0     1346 2022-03-23 15:04:13.000000 NinjaTools-0.8.9/ninja_tools/image_functions.py
--rw-rw-rw-   0        0        0    15394 2022-03-23 15:04:18.000000 NinjaTools-0.8.9/ninja_tools/image_processor.py
--rw-rw-rw-   0        0        0    10295 2022-07-14 12:48:58.000000 NinjaTools-0.8.9/ninja_tools/keyboard.py
--rw-rw-rw-   0        0        0     2590 2022-04-04 09:23:36.000000 NinjaTools-0.8.9/ninja_tools/memory.py
--rw-rw-rw-   0        0        0     3337 2022-07-14 12:51:21.000000 NinjaTools-0.8.9/ninja_tools/mouse.py
--rw-rw-rw-   0        0        0     1971 2022-03-10 19:45:07.000000 NinjaTools-0.8.9/ninja_tools/processing.py
--rw-rw-rw-   0        0        0     2270 2022-03-23 14:47:13.000000 NinjaTools-0.8.9/ninja_tools/screen_capture.py
--rw-rw-rw-   0        0        0     6596 2022-04-08 02:42:11.000000 NinjaTools-0.8.9/ninja_tools/utils.py
--rw-rw-rw-   0        0        0       42 2022-10-11 12:50:24.447614 NinjaTools-0.8.9/setup.cfg
--rw-rw-rw-   0        0        0     1410 2022-10-11 12:50:19.000000 NinjaTools-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-03 02:43:39.659712 NinjaTools-0.9.0/
+drwxrwxrwx   0        0        0        0 2022-11-03 02:43:39.518986 NinjaTools-0.9.0/NinjaTools.egg-info/
+-rw-rw-rw-   0        0        0      621 2022-11-03 02:43:39.000000 NinjaTools-0.9.0/NinjaTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2022-11-03 02:43:39.000000 NinjaTools-0.9.0/NinjaTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-03 02:43:39.000000 NinjaTools-0.9.0/NinjaTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      294 2022-11-03 02:43:39.000000 NinjaTools-0.9.0/NinjaTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-11-03 02:43:39.000000 NinjaTools-0.9.0/NinjaTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      621 2022-11-03 02:43:39.659712 NinjaTools-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2022-03-10 21:15:41.000000 NinjaTools-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-11-03 02:43:39.647133 NinjaTools-0.9.0/ninja_tools/
+-rw-rw-rw-   0        0        0        0 2022-03-10 21:19:30.000000 NinjaTools-0.9.0/ninja_tools/__init__.py
+-rw-rw-rw-   0        0        0      545 2022-03-08 20:04:20.000000 NinjaTools-0.9.0/ninja_tools/bbox.py
+-rw-rw-rw-   0        0        0     6094 2022-10-13 05:07:34.000000 NinjaTools-0.9.0/ninja_tools/excel.py
+-rw-rw-rw-   0        0        0     2425 2022-03-23 15:11:16.000000 NinjaTools-0.9.0/ninja_tools/find_image.py
+-rw-rw-rw-   0        0        0     2406 2022-03-23 15:11:16.000000 NinjaTools-0.9.0/ninja_tools/image_cropper.py
+-rw-rw-rw-   0        0        0     1346 2022-03-23 15:04:13.000000 NinjaTools-0.9.0/ninja_tools/image_functions.py
+-rw-rw-rw-   0        0        0    15394 2022-03-23 15:04:18.000000 NinjaTools-0.9.0/ninja_tools/image_processor.py
+-rw-rw-rw-   0        0        0     2101 2022-10-29 18:43:07.000000 NinjaTools-0.9.0/ninja_tools/json_db.py
+-rw-rw-rw-   0        0        0    10295 2022-07-14 12:48:58.000000 NinjaTools-0.9.0/ninja_tools/keyboard.py
+-rw-rw-rw-   0        0        0     2590 2022-04-04 09:23:36.000000 NinjaTools-0.9.0/ninja_tools/memory.py
+-rw-rw-rw-   0        0        0     3337 2022-07-14 12:51:21.000000 NinjaTools-0.9.0/ninja_tools/mouse.py
+-rw-rw-rw-   0        0        0     1971 2022-03-10 19:45:07.000000 NinjaTools-0.9.0/ninja_tools/processing.py
+-rw-rw-rw-   0        0        0     2270 2022-03-23 14:47:13.000000 NinjaTools-0.9.0/ninja_tools/screen_capture.py
+-rw-rw-rw-   0        0        0     6596 2022-04-08 02:42:11.000000 NinjaTools-0.9.0/ninja_tools/utils.py
+-rw-rw-rw-   0        0        0       42 2022-11-03 02:43:39.659712 NinjaTools-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1397 2022-11-03 02:43:35.000000 NinjaTools-0.9.0/setup.py
```

### Comparing `NinjaTools-0.8.9/NinjaTools.egg-info/PKG-INFO` & `NinjaTools-0.9.0/NinjaTools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: NinjaTools
-Version: 0.8.9
+Version: 0.9.0
 Summary: Bunch of useful tools
 Home-page: https://github.com/nikkoxgonzales/ninja-tools
 Author: Nikko Gonzales
 Author-email: nikkoxgonzales@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: image
 Provides-Extra: memory
 Provides-Extra: excel
 Provides-Extra: all
 
 Ninja Tools
```

### Comparing `NinjaTools-0.8.9/NinjaTools.egg-info/SOURCES.txt` & `NinjaTools-0.9.0/NinjaTools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 ninja_tools/__init__.py
 ninja_tools/bbox.py
 ninja_tools/excel.py
 ninja_tools/find_image.py
 ninja_tools/image_cropper.py
 ninja_tools/image_functions.py
 ninja_tools/image_processor.py
+ninja_tools/json_db.py
 ninja_tools/keyboard.py
 ninja_tools/memory.py
 ninja_tools/mouse.py
 ninja_tools/processing.py
 ninja_tools/screen_capture.py
 ninja_tools/utils.py
```

### Comparing `NinjaTools-0.8.9/PKG-INFO` & `NinjaTools-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: NinjaTools
-Version: 0.8.9
+Version: 0.9.0
 Summary: Bunch of useful tools
 Home-page: https://github.com/nikkoxgonzales/ninja-tools
 Author: Nikko Gonzales
 Author-email: nikkoxgonzales@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: image
 Provides-Extra: memory
 Provides-Extra: excel
 Provides-Extra: all
 
 Ninja Tools
```

### Comparing `NinjaTools-0.8.9/ninja_tools/bbox.py` & `NinjaTools-0.9.0/ninja_tools/bbox.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/excel.py` & `NinjaTools-0.9.0/ninja_tools/excel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import re
 import warnings
 
 try:
     import openpyxl
-    import xlrd
     import webcolors
     from openpyxl.utils.cell import coordinate_from_string, column_index_from_string
 except ImportError:
     raise 'pip install ninjatools[excel] or ninjatools[all] to use excel functions!'
 
 # Remove warnings
 warnings.filterwarnings('ignore', category=UserWarning, module='openpyxl')
@@ -22,15 +20,14 @@
     def __repr__(self):
         str_color = ', '.join(str(_) for _ in self.rgb)
         return f'Closest Color: {self.name} | RGB: ({str_color})'
 
 
 class Excel:
     def __init__(self, workbook_path):
-        self.wb_xlrd = xlrd.open_workbook(workbook_path)
         self.wb = openpyxl.load_workbook(workbook_path, data_only=True)
         self.sheet_name = None
 
     def get_sheets(self) -> list:
         """
         Returns a list of sheet names
         :return:
@@ -41,17 +38,26 @@
     def cell(self, cell, sheet_name=None):
         """
         Returns the value of a cell
         :param cell:
         :param sheet_name:
         :return:
         """
+
+        if isinstance(cell, str):
+            cell = self.get_cell(cell)
+        elif not isinstance(cell, tuple) and not isinstance(cell, list):
+            raise TypeError('cell must be a tuple or string')
+
         sheet_name = sheet_name if sheet_name else self.sheet_name
         ws = self.wb[sheet_name]
-        return ws[cell].value
+        value = ws.cell(cell[0], cell[1]).value
+        value = '' if value is None else value
+        value = str(value).strip().replace('\xa0', ' ')
+        return value
 
     def get_color(self, cell) -> ColorObject:
         """
         Returns the color of a cell
         :param cell:
         :return:
         """
@@ -60,39 +66,54 @@
         hex_color = f'#{hex_color[2:]}'
         rgb_color = webcolors.hex_to_rgb(hex_color)
         rgb_color = (rgb_color.red, rgb_color.green, rgb_color.blue)
         color_name = self.closest_color(rgb_color)
 
         return ColorObject(hex_color, rgb_color, color_name)
 
-    def read_range(self, cell_1, cell_2, sheet_name=None) -> list:
+    def read_range(self, start, end, sheet_name=None, remove_empty=False) -> list:
         """
         Reads a range of cells
-        :param cell_1:
-        :param cell_2:
+        :param start:
+        :param end:
         :param sheet_name:
+        :param remove_empty:
         :return:
         """
-        sheet_name = sheet_name if sheet_name else self.sheet_name
+        data = []
 
-        var = self.get_cell(cell_1)
-        var2 = self.get_cell(cell_2)
+        sheet_name = sheet_name if sheet_name else self.sheet_name
 
-        ws = self.wb[sheet_name]
+        rc_start = self.get_cell(start)
+        rc_end = self.get_cell(end)
 
-        data = []
-        for _ in range(var[0], var2[0] + 1):
+        for row in range(rc_start[0], rc_end[0] + 1):
             temp = []
-            for __ in range(var[1], var2[1] + 1):
-                temp.append(ws.cell(_, __).value)
+            for col in range(rc_start[1], rc_end[1] + 1):
+                temp.append(self.cell((row, col), sheet_name))
 
-            data.append(temp)
+            if remove_empty:
+                if not all([not _ for _ in temp]):
+                    data.append(temp)
+            else:
+                data.append(temp)
 
         return data
 
+    def read_all(self, sheet_name=None, remove_empty=False) -> list:
+        """
+        Reads all cells in a sheet
+        :param sheet_name:
+        :param remove_empty:
+        :return:
+        """
+        sheet_name = sheet_name if sheet_name else self.sheet_name
+        return self.read_range('A1', self.get_last(), sheet_name, remove_empty)
+
+    # Still buggy
     def read_indefinitely(self, start_cell: str, num_of_columns: int, num_of_rows=None, steps: int = 1) -> list:
         """
         Reads a range of cells indefinitely
         :param start_cell:
         :param num_of_columns:
         :param num_of_rows:
         :param steps:
@@ -134,38 +155,15 @@
         Returns the cell coordinates
         :param cell:
         :return:
         """
         xy = coordinate_from_string(cell)
         col = column_index_from_string(xy[0])
         row = xy[1]
-        return col, row
-    #
-    # @staticmethod
-    # def get_cell(cell) -> tuple:
-    #     """
-    #     Returns a tuple of the cell
-    #     :param cell:
-    #     :return:
-    #     """
-    #     r = re.compile("([a-zA-Z]+)([0-9]+)")
-    #     m = r.match(cell)
-    #     col = m.group(1).upper()
-    #     number_row = int(m.group(2)) - 1
-    #
-    #     abc = ["A", "B", "C", "D", "E", "F", "G", "H", "I",
-    #            "J", "K", "L", "M", "N", "O", "P", "Q", "R",
-    #            "S", "T", "U", "V", "W", "X", "Y", "Z"]
-    #
-    #     number_col = 0
-    #
-    #     for char in col:
-    #         number_col += abc.index(char)
-    #
-    #     return number_row, number_col
+        return row, col
 
     @staticmethod
     def get_cell_name(row, column) -> str:
         """
         Returns the cell name
         :param row:
         :param column:
```

### Comparing `NinjaTools-0.8.9/ninja_tools/find_image.py` & `NinjaTools-0.9.0/ninja_tools/find_image.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/image_cropper.py` & `NinjaTools-0.9.0/ninja_tools/image_cropper.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/image_functions.py` & `NinjaTools-0.9.0/ninja_tools/image_functions.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/image_processor.py` & `NinjaTools-0.9.0/ninja_tools/image_processor.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/keyboard.py` & `NinjaTools-0.9.0/ninja_tools/keyboard.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/memory.py` & `NinjaTools-0.9.0/ninja_tools/memory.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/mouse.py` & `NinjaTools-0.9.0/ninja_tools/mouse.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/processing.py` & `NinjaTools-0.9.0/ninja_tools/processing.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/screen_capture.py` & `NinjaTools-0.9.0/ninja_tools/screen_capture.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/ninja_tools/utils.py` & `NinjaTools-0.9.0/ninja_tools/utils.py`

 * *Files identical despite different names*

### Comparing `NinjaTools-0.8.9/setup.py` & `NinjaTools-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="NinjaTools",
-    version="0.8.9",
+    version="0.9.0",
     author="Nikko Gonzales",
     author_email="nikkoxgonzales@gmail.com",
     description="Bunch of useful tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nikkoxgonzales/ninja-tools",
-    install_requires=[
-        'pywin32>=303',
-        'pyperclip>=1.8.2',
-        'psutil>=5.9.0',
-    ],
     extras_require={
         'image': [
             'opencv-python==4.5.5.62',
             'scikit-image>=0.19.2',
             'numpy>=1.22.3',
         ],
 
         'memory': [
             'Pymem>=1.8.5',
             'regex'
         ],
 
         'excel': [
-            'xlrd==1.2.0',
             'openpyxl==3.0.10',
             'webcolors>=1.12'
         ],
 
         'all': [
             'opencv-python==4.5.5.62',
             'scikit-image>=0.19.2',
-            'xlrd==1.2.0',
+            'openpyxl==3.0.10',
+            'webcolors>=1.12'
             'numpy>=1.22.3',
             'Pymem>=1.8.5',
+            'pywin32>=303',
+            'pyperclip>=1.8.2',
+            'psutil>=5.9.0'
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows",
     ],
     packages=setuptools.find_packages(),
-    python_requires='>=3.9'
+    python_requires='>=3.7'
 )
```

