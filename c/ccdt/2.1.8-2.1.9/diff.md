# Comparing `tmp/ccdt-2.1.8.tar.gz` & `tmp/ccdt-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.1.8.tar", last modified: Tue Jun  6 03:09:34 2023, max compression
+gzip compressed data, was "ccdt-2.1.9.tar", last modified: Tue Jun  6 06:37:12 2023, max compression
```

## Comparing `ccdt-2.1.8.tar` & `ccdt-2.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.171066 ccdt-2.1.8/
--rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.8/LICENSE
--rw-rw-rw-   0        0        0     4309 2023-06-06 03:09:34.169071 ccdt-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3785 2023-05-23 02:44:28.000000 ccdt-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.032437 ccdt-2.1.8/ccdt/
--rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.8/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.051386 ccdt-2.1.8/ccdt/dataset/
--rw-rw-rw-   0        0        0      216 2023-05-17 01:52:32.000000 ccdt-2.1.8/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.079310 ccdt-2.1.8/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.8/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    22572 2023-05-25 05:57:25.000000 ccdt-2.1.8/ccdt/dataset/base_coco/base_coco.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.102249 ccdt-2.1.8/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.8/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0     7523 2023-06-06 03:07:09.000000 ccdt-2.1.8/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0    63537 2023-06-06 03:07:09.000000 ccdt-2.1.8/ccdt/dataset/base_labelme/base_labelme.py
--rw-rw-rw-   0        0        0    14420 2023-05-25 03:24:49.000000 ccdt-2.1.8/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.110255 ccdt-2.1.8/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      221 2023-05-17 01:56:42.000000 ccdt-2.1.8/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.8/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    17029 2023-05-25 06:27:22.000000 ccdt-2.1.8/ccdt/dataset/utils/labelme_load.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.154133 ccdt-2.1.8/ccdt/video_tool/
--rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.8/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-05-25 06:23:23.000000 ccdt-2.1.8/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     4845 2023-05-25 06:30:32.000000 ccdt-2.1.8/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.046398 ccdt-2.1.8/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4309 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-06-06 03:09:34.000000 ccdt-2.1.8/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-06 03:09:33.000000 ccdt-2.1.8/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 03:09:34.171066 ccdt-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2401 2023-06-06 03:07:09.000000 ccdt-2.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 03:09:34.166078 ccdt-2.1.8/test/
--rw-rw-rw-   0        0        0     8106 2023-06-05 05:36:13.000000 ccdt-2.1.8/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:12.144636 ccdt-2.1.9/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.9/LICENSE
+-rw-rw-rw-   0        0        0     4309 2023-06-06 06:37:12.142867 ccdt-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-05-23 02:44:28.000000 ccdt-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:12.089011 ccdt-2.1.9/ccdt/
+-rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.9/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:12.109956 ccdt-2.1.9/ccdt/dataset/
+-rw-rw-rw-   0        0        0      216 2023-05-17 01:52:32.000000 ccdt-2.1.9/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:12.114942 ccdt-2.1.9/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.9/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    22572 2023-05-25 05:57:25.000000 ccdt-2.1.9/ccdt/dataset/base_coco/base_coco.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:12.122921 ccdt-2.1.9/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.9/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0     7523 2023-06-06 03:07:09.000000 ccdt-2.1.9/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0    64027 2023-06-06 06:30:23.000000 ccdt-2.1.9/ccdt/dataset/base_labelme/base_labelme.py
+-rw-rw-rw-   0        0        0    14600 2023-06-06 06:21:07.000000 ccdt-2.1.9/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:12.130899 ccdt-2.1.9/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      221 2023-05-17 01:56:42.000000 ccdt-2.1.9/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.9/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    17029 2023-05-25 06:27:22.000000 ccdt-2.1.9/ccdt/dataset/utils/labelme_load.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:12.138878 ccdt-2.1.9/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.9/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-05-25 06:23:23.000000 ccdt-2.1.9/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     4845 2023-05-25 06:30:32.000000 ccdt-2.1.9/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:12.103971 ccdt-2.1.9/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4309 2023-06-06 06:37:12.000000 ccdt-2.1.9/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-06 06:37:12.000000 ccdt-2.1.9/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 06:37:12.000000 ccdt-2.1.9/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-06 06:37:12.000000 ccdt-2.1.9/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-06-06 06:37:12.000000 ccdt-2.1.9/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-06 06:37:12.000000 ccdt-2.1.9/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 06:37:12.144636 ccdt-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2401 2023-06-06 06:36:46.000000 ccdt-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 06:37:12.140872 ccdt-2.1.9/test/
+-rw-rw-rw-   0        0        0     8106 2023-06-05 05:36:13.000000 ccdt-2.1.9/test/test.py
```

### Comparing `ccdt-2.1.8/LICENSE` & `ccdt-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.8/PKG-INFO` & `ccdt-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.8
+Version: 2.1.9
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.8/README.md` & `ccdt-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.8/ccdt/dataset/base_coco/base_coco.py` & `ccdt-2.1.9/ccdt/dataset/base_coco/base_coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.8/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.1.9/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.8/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.1.9/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files 0% similar despite different names*

```diff
@@ -753,14 +753,21 @@
             f'去重前文件数量有{len(self.datasets)}，去重后文件数量有{len(self.datasets) - del_num}，删除重复的文件有{del_num}')
 
     def check_group_labelme(self, parameter):
         """
         labelme数据集检查功能实现，包含标注多边形点数错误、标注分组错误、标注越界错误、标注flags属性错误、
         :param parameter:
         """
+        if parameter.judging_label == 'plate':
+            for dataset in tqdm(self.datasets):
+                if dataset.get('background') is True:
+                    for shape in dataset.get('labelme_info').get('shapes'):
+                        if shape.get('shape_type') == 'polygon':  # 车牌标注都是多边形的，只要group_id为空就追加
+                            if shape.get('group_id') is None:
+                                self.error_dataset_handle(dataset)
         if isinstance(parameter.judging_polygon, int):  # 检查多边形点是否超出5个点
             print(f'多边形标注的点是否超出预期数量，预期为4个点，超出则人工矫正')
             for dataset in tqdm(self.datasets):
                 if dataset.get('background') is True:
                     for shape in dataset.get('labelme_info').get('shapes'):
                         if shape.get('shape_type') == 'polygon':
                             if len(shape.get('points')) != parameter.judging_polygon:
@@ -773,15 +780,14 @@
                     for shape in dataset.get('labelme_info').get('shapes'):
                         group_id_list[shape['group_id']].append(shape)
                     # 判断分组标注元素数量，是否符合预测判断条件预期
                     for group_shape_key, group_shape_value in group_id_list.items():
                         if len(group_shape_value) != parameter.judging_group:
                             # 如果同一张图像分组出现多次错误，只追加一次dataset
                             self.error_dataset_handle(dataset)
-
         if isinstance(parameter.judging_flags, dict):
             print(f'对标注flags属性进行检查，比如检查车牌颜色、单双层字符，是否，漏勾选。complete被勾选后，车牌号是否录入')
             for dataset in tqdm(self.datasets):
                 file_path = dataset.get('full_path')
                 if dataset.get('background') is True:
                     for shape in dataset.get('labelme_info').get('shapes'):
                         if shape.get('flags'):
```

### Comparing `ccdt-2.1.8/ccdt/dataset/main.py` & `ccdt-2.1.9/ccdt/dataset/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     parser.add_argument('--http-url', type=str,
                         help="minio文件对象存储中，网络文件统一资源定位器，http://192.168.1.235:9393/chipeak-dataset")
     parser.add_argument('--min-pixel', type=int, default=512,
                         help='最小像素截图设置，默认512像素。即大于512像素的矩形框才进行截图')
     parser.add_argument('--judging-group', type=int, help='默认值为2个shape元素为一组，用于判断分组元素的数量')
     # parser.add_argument('--judging-flags', type=json.loads, help="检查flags默认标注属性，是否符合标注准则")
     parser.add_argument('--judging-flags', type=ast.literal_eval, help="检查flags默认标注属性，是否符合标注准则")
+    parser.add_argument('--judging-label', type=str, help="检查车牌默认分组属性，是否符合标注准则，车牌一定要打组，如果没有打组就筛选出来")
     parser.add_argument('--judging-polygon', type=int,
                         help='检查多边形标注的点是否超出预期数量，比如4个点的多边形，不能出现5个')
     parser.add_argument('--judging-cross-the-border', type=str, help="检查标注形状是否超越原始图像边界")
     parser.add_argument('--point-number', type=int,
                         help='点标注的数量，用于标注点排序时，追加标注点到列表中然后判断，是否满足标注规则')
     parser.add_argument('--automatic-correction', action="store_true",
                         help="默认False，是否自动矫正标注形状超越图像边界情况。是为True，否为False")
```

### Comparing `ccdt-2.1.8/ccdt/dataset/utils/encoder.py` & `ccdt-2.1.9/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.8/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.1.9/ccdt/dataset/utils/labelme_load.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.8/ccdt/video_tool/split.py` & `ccdt-2.1.9/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.8/ccdt/video_tool/video_main.py` & `ccdt-2.1.9/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.8/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.9/ccdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.8
+Version: 2.1.9
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.8/ccdt.egg-info/SOURCES.txt` & `ccdt-2.1.9/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.8/setup.py` & `ccdt-2.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.1.8',
+    version='2.1.9',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ccdt-2.1.8/test/test.py` & `ccdt-2.1.9/test/test.py`

 * *Files identical despite different names*

