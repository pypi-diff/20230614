# Comparing `tmp/HawaData-0.6.3.tar.gz` & `tmp/HawaData-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.6.3.tar", last modified: Tue Jun 13 09:39:12 2023, max compression
+gzip compressed data, was "HawaData-0.6.4.tar", last modified: Wed Jun 14 03:28:05 2023, max compression
```

## Comparing `HawaData-0.6.3.tar` & `HawaData-0.6.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.738807 HawaData-0.6.3/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.733116 HawaData-0.6.3/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2870 2023-06-13 09:39:12.000000 HawaData-0.6.3/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-13 09:39:12.000000 HawaData-0.6.3/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-13 09:39:12.000000 HawaData-0.6.3/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-13 09:39:12.000000 HawaData-0.6.3/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2870 2023-06-13 09:39:12.738566 HawaData-0.6.3/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.6.3/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.733551 HawaData-0.6.3/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.6.3/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.734772 HawaData-0.6.3/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.6.3/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.6.3/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.6.3/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.6.3/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.6.3/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.735834 HawaData-0.6.3/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.6.3/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9450 2023-06-13 03:35:19.000000 HawaData-0.6.3/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5630 2023-06-13 03:42:10.000000 HawaData-0.6.3/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3065 2023-06-01 01:31:26.000000 HawaData-0.6.3/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.6.3/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.737204 HawaData-0.6.3/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.6.3/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.6.3/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.6.3/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.6.3/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-08 13:01:01.000000 HawaData-0.6.3/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.6.3/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.738016 HawaData-0.6.3/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.6.3/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28118 2023-06-13 09:39:06.000000 HawaData-0.6.3/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.6.3/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-13 09:39:12.738875 HawaData-0.6.3/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.6.3/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-13 09:39:12.738256 HawaData-0.6.3/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.6.3/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-14 03:28:05.252678 HawaData-0.6.4/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-14 03:28:05.238978 HawaData-0.6.4/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2899 2023-06-14 03:28:05.000000 HawaData-0.6.4/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-14 03:28:05.000000 HawaData-0.6.4/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-14 03:28:05.000000 HawaData-0.6.4/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-14 03:28:05.000000 HawaData-0.6.4/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2899 2023-06-14 03:28:05.252376 HawaData-0.6.4/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.6.4/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-14 03:28:05.239507 HawaData-0.6.4/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.6.4/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-14 03:28:05.242669 HawaData-0.6.4/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.6.4/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.6.4/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.6.4/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.6.4/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.6.4/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-14 03:28:05.244940 HawaData-0.6.4/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.6.4/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    10803 2023-06-14 03:26:20.000000 HawaData-0.6.4/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5630 2023-06-13 03:42:10.000000 HawaData-0.6.4/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3065 2023-06-01 01:31:26.000000 HawaData-0.6.4/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.6.4/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-14 03:28:05.249076 HawaData-0.6.4/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.6.4/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.6.4/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.6.4/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.6.4/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-08 13:01:01.000000 HawaData-0.6.4/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.6.4/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-14 03:28:05.251048 HawaData-0.6.4/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.6.4/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28120 2023-06-14 02:44:03.000000 HawaData-0.6.4/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.6.4/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-14 03:28:05.252766 HawaData-0.6.4/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.6.4/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-14 03:28:05.251677 HawaData-0.6.4/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.6.4/test/test_query.py
```

### Comparing `HawaData-0.6.3/HawaData.egg-info/PKG-INFO` & `HawaData-0.6.4/HawaData.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.6.3
+Version: 0.6.4
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -99,7 +99,8 @@
 - 0.5.11 remove text
 - 0.5.12 get grade focus
 - 0.5.13 count grade class scores
 - 0.6.0 add student health api data
 - 0.6.1 count dim field scores
 - 0.6.2 count dim field scores 2
 - 0.6.3 count student grade
+- 0.6.4 count dim field rank
```

### Comparing `HawaData-0.6.3/HawaData.egg-info/SOURCES.txt` & `HawaData-0.6.4/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/PKG-INFO` & `HawaData-0.6.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.6.3
+Version: 0.6.4
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -99,7 +99,8 @@
 - 0.5.11 remove text
 - 0.5.12 get grade focus
 - 0.5.13 count grade class scores
 - 0.6.0 add student health api data
 - 0.6.1 count dim field scores
 - 0.6.2 count dim field scores 2
 - 0.6.3 count student grade
+- 0.6.4 count dim field rank
```

### Comparing `HawaData-0.6.3/README.md` & `HawaData-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/hawa/base/db.py` & `HawaData-0.6.4/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/hawa/base/init.py` & `HawaData-0.6.4/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/hawa/common/data.py` & `HawaData-0.6.4/hawa/common/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """通用的 report data 构造器，支持 校、区、市、省、全国级别的通用报告数据构造"""
 import json
-from collections import Counter
+from collections import Counter, defaultdict
 from dataclasses import dataclass, field
 from typing import Optional, ClassVar, Any, Set
 
 import pandas as pd
 import pendulum
 from munch import Munch
 
@@ -62,14 +62,15 @@
 
     item_ids: Optional[set[int]] = None
     items: Optional[pd.DataFrame] = None
 
     # 辅助工具
     grade_util: Optional[GradeData] = None
     case_util: Optional[CaseData] = None
+    rank_names = ['待提高', '中等', '良好', '优秀']
     measurement = Measurement()
 
     # 计算数据
     final_answers: pd.DataFrame = field(default_factory=pd.DataFrame)
     final_scores: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     # 去年全国数据
@@ -232,7 +233,40 @@
             else:
                 grade_data = data[str(3)]
 
         grade_data['people']['grade'] = f"{grade}年级"
         for k, v in grade_data['code'].items():
             grade_data['code'][k]['grade'] = grade
         return grade_data
+
+    def sort_rank(self, name: str) -> int:
+        order_map = dict(zip(self.rank_names, range(0, 4)))
+        return order_map[name]
+
+    def count_dim_field_ranks(self, item_code: str):
+        """
+        计算维度、领域的 ranks 分级比例
+        :param item_code:dimision or field
+        """
+        r = defaultdict(list)
+        codes = set()
+        for (s, c), student_code_group in self.final_answers.groupby(['student_id', item_code]):
+            s_c_score = round(student_code_group.score.mean() * 100, 2)
+            codes.add(c)
+            r[c].append(s_c_score)
+        codes = list(codes)
+        df = pd.DataFrame.from_records(r)
+        res = {}
+        for c in codes:
+            row = df[c]
+            base_row_ranks = {k: 0 for k in self.rank_names}
+            count_row_ranks = pd.cut(
+                row, bins=[0, 60, 80, 90, 100], labels=self.rank_names,
+                right=False, include_lowest=True,
+            ).value_counts().to_dict()
+            sum_value = sum(count_row_ranks.values())
+            row_ranks = {k: round(v / sum_value * 100, 2) for k, v in (base_row_ranks | count_row_ranks).items()}
+            res[c] = row_ranks
+
+        return {
+            "data": res, "codes": codes, "legend": self.rank_names,
+        }
```

### Comparing `HawaData-0.6.3/hawa/common/query.py` & `HawaData-0.6.4/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/hawa/common/utils.py` & `HawaData-0.6.4/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/hawa/config.py` & `HawaData-0.6.4/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/hawa/data/klass.py` & `HawaData-0.6.4/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/hawa/data/school.py` & `HawaData-0.6.4/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/hawa/data/student.py` & `HawaData-0.6.4/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/hawa/paper/health.py` & `HawaData-0.6.4/hawa/paper/health.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     def replace_hai(self, text: str, condition: list):
         if condition:
             return text
         else:
             return text.replace('还', '')
 
 
+
+
 @dataclass
 class HealthApiData(HealthData):
     """为 yingde api 项目提供基类"""
     grade: Optional[int] = None  # 必填
     grade_final_scores: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     def _to_init_d_cases(self):
```

### Comparing `HawaData-0.6.3/hawa/paper/mht.py` & `HawaData-0.6.4/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/setup.py` & `HawaData-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.3/test/test_query.py` & `HawaData-0.6.4/test/test_query.py`

 * *Files identical despite different names*

