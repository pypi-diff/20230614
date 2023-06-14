# Comparing `tmp/yunxiao-0.2.6.tar.gz` & `tmp/yunxiao-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.2.6.tar", last modified: Wed Jun 14 17:22:08 2023, max compression
+gzip compressed data, was "yunxiao-0.2.7.tar", last modified: Wed Jun 14 17:49:56 2023, max compression
```

## Comparing `yunxiao-0.2.6.tar` & `yunxiao-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 17:22:08.044092 yunxiao-0.2.6/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.6/LICENSE
--rw-rw-rw-   0        0        0    12954 2023-06-14 17:22:08.044092 yunxiao-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.6/README.md
--rw-rw-rw-   0        0        0     1250 2023-06-14 17:21:42.000000 yunxiao-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 17:22:08.044092 yunxiao-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 17:22:08.029902 yunxiao-0.2.6/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.6/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:22:08.035495 yunxiao-0.2.6/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.6/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.6/yunxiao/app.py
--rw-rw-rw-   0        0        0    18535 2023-06-14 17:21:42.000000 yunxiao-0.2.6/yunxiao/v2.py
--rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.6/yunxiao/web.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.6/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:22:08.040038 yunxiao-0.2.6/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    12954 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 17:49:56.603193 yunxiao-0.2.7/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0    12954 2023-06-14 17:49:56.602184 yunxiao-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.7/README.md
+-rw-rw-rw-   0        0        0     1250 2023-06-14 17:49:40.000000 yunxiao-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 17:49:56.603193 yunxiao-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 17:49:56.591036 yunxiao-0.2.7/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:49:56.596099 yunxiao-0.2.7/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.7/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.7/yunxiao/app.py
+-rw-rw-rw-   0        0        0    18555 2023-06-14 17:49:30.000000 yunxiao-0.2.7/yunxiao/v2.py
+-rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.7/yunxiao/web.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.7/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:49:56.601157 yunxiao-0.2.7/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    12954 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 17:49:56.000000 yunxiao-0.2.7/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.2.6/LICENSE` & `yunxiao-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.6/PKG-INFO` & `yunxiao-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.6
+Version: 0.2.7
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.2.6/README.md` & `yunxiao-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.6/pyproject.toml` & `yunxiao-0.2.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.2.6"
+version = "0.2.7"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
```

### Comparing `yunxiao-0.2.6/yunxiao/app.py` & `yunxiao-0.2.7/yunxiao/app.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.6/yunxiao/v2.py` & `yunxiao-0.2.7/yunxiao/v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 "queryKey": name,
                 "statusList": [status],
                 "page": {"pageNum": 1, "pageSize": size}
             }
         )["data"]
 
     # 列出全部学生
-    @loop
+    @loop("")
     def student_listall(self, page, size):
         """
         列出全部学生
         :return:
         """
         return self.request(
             method="post",
@@ -165,15 +165,15 @@
                 "classStudentStatus": class_student_status,
                 "orgTag": 1,
                 "page": {"pageNum": 1, "pageSize": size}
             }
         )["data"]
 
     # 列出全部课程
-    @loop
+    @loop("")
     def curriculum_list_all(self, page, size):
         """
         列出全部课程
         :return:
         """
         return self.request(
             method="post",
@@ -206,15 +206,15 @@
                     "pageNum": 1,
                     "pageSize": size
                 }
             }
         )["data"]
 
     # 列出指定日期范围全部排课
-    @loop
+    @loop("")
     def arrange_list_daterange(self, page, size, before_today: int, after_today: int):
         """
         列出全部排课
         :return:
         """
         return self.request(
             method="post",
@@ -338,15 +338,15 @@
                 "orderByCampus": 1,
                 "_t_": UsedTime.stamp
             }
         )["data"]["dataReportVos"]
         return list(map(lambda item: {**item, "id": f"{date}-{item['campusId']}"}, data_list))
 
     # 列出全部班级
-    @loop
+    @loop("")
     def class_list_all(self, page, size):
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-edu/classInfo/page",
             json={
                 "_t_": UsedTime.stamp,
                 "orgTag": 1,
@@ -484,15 +484,15 @@
                 "startTime": startdate,
                 "endTime": enddate,
                 "displayInvalidOrder": True
             }
         )["data"]
 
     # 列出所有课程卡
-    @loop
+    @loop("")
     def card_list_all(self, page, size):
         """
         列出所有课程卡
         :return:
         """
         return self.request(
             method="post",
```

### Comparing `yunxiao-0.2.6/yunxiao/web.py` & `yunxiao-0.2.7/yunxiao/web.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.6/yunxiao/yunxiao.py` & `yunxiao-0.2.7/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.6/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.2.7/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.6
+Version: 0.2.7
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

