# Comparing `tmp/yunxiao-0.2.5.tar.gz` & `tmp/yunxiao-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.2.5.tar", last modified: Wed Jun 14 17:04:56 2023, max compression
+gzip compressed data, was "yunxiao-0.2.6.tar", last modified: Wed Jun 14 17:22:08 2023, max compression
```

## Comparing `yunxiao-0.2.5.tar` & `yunxiao-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 17:04:56.087885 yunxiao-0.2.5/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.5/LICENSE
--rw-rw-rw-   0        0        0    12954 2023-06-14 17:04:56.086878 yunxiao-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.5/README.md
--rw-rw-rw-   0        0        0     1205 2023-06-14 17:04:35.000000 yunxiao-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 17:04:56.087885 yunxiao-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 17:04:56.074196 yunxiao-0.2.5/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.5/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:04:56.080309 yunxiao-0.2.5/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.5/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.5/yunxiao/app.py
--rw-rw-rw-   0        0        0    18511 2023-06-14 17:03:03.000000 yunxiao-0.2.5/yunxiao/v2.py
--rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.5/yunxiao/web.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.5/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:04:56.085374 yunxiao-0.2.5/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    12954 2023-06-14 17:04:56.000000 yunxiao-0.2.5/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-14 17:04:56.000000 yunxiao-0.2.5/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 17:04:56.000000 yunxiao-0.2.5/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 17:04:56.000000 yunxiao-0.2.5/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 17:04:56.000000 yunxiao-0.2.5/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 17:22:08.044092 yunxiao-0.2.6/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0    12954 2023-06-14 17:22:08.044092 yunxiao-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.6/README.md
+-rw-rw-rw-   0        0        0     1250 2023-06-14 17:21:42.000000 yunxiao-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 17:22:08.044092 yunxiao-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 17:22:08.029902 yunxiao-0.2.6/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.6/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:22:08.035495 yunxiao-0.2.6/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.6/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.6/yunxiao/app.py
+-rw-rw-rw-   0        0        0    18535 2023-06-14 17:21:42.000000 yunxiao-0.2.6/yunxiao/v2.py
+-rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.6/yunxiao/web.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.6/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:22:08.040038 yunxiao-0.2.6/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    12954 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 17:22:08.000000 yunxiao-0.2.6/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.2.5/LICENSE` & `yunxiao-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.5/PKG-INFO` & `yunxiao-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.5
+Version: 0.2.6
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.2.5/README.md` & `yunxiao-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.5/pyproject.toml` & `yunxiao-0.2.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.2.5"
+version = "0.2.6"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,14 +22,14 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
-
+"0.2.6" = "V2 中更多使用分片读取。"
 "0.2.5" = "修复 V2 中的 API端点错误。新增 loop 装饰器便于分片提取大量数据。"
 "0.2.4" = "修复 v2 中一个API端点错误及鉴权更新错误"
 "0.2.2" = "新增 v2, 更清晰的函数命名，简洁快速的拉取全部数据。"
 "0.2.1" = "web 端请求 BUG 修复"
 "0.2.0" = "BUG修复"
 "0.1.9" = "更改鉴权方式，保存鉴权到系统环境变量。当因鉴权失效导致请求失败时，自动更新鉴权并重新发起请求。意图减少更新鉴权的次数。"
```

### Comparing `yunxiao-0.2.5/yunxiao/app.py` & `yunxiao-0.2.6/yunxiao/app.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.5/yunxiao/v2.py` & `yunxiao-0.2.6/yunxiao/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 result = []
                 count = 1
                 page = kwargs.get("page")
                 size = kwargs.get("size")
                 while (now := len(result)) != count:
                     page += 1
                     res = func(*args, **kwargs)
-                    data = res["data"][KEY]
+                    data = res["data"][KEY] if KEY else res["data"]
                     result.extend(data)
                     count = res["page"]["totalCount"]
                     print(f"size: {size}, page: {page}, {now}/{count}")
                     size = size if (count - len(result)) > size else (count - len(result))
                     kwargs["size"] = size
                     kwargs["page"] = page
                 print(f"size: {size}, page: {page}, {now}/{count}")
@@ -78,28 +78,28 @@
     # 列出全部校区
     def campus_list_all(self) -> list:
         return self.request(
             method="get",
             url="https://yunxiao.xiaogj.com/api/cs-crm/campus/list?type=2"
         )["data"]
 
-    # 列出全部老师[最大9999条]
+    # 列出全部老师[最大999条]
     def teacher_list_all(self) -> list:
         """
         列出全部老师<MAX-9999>
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-crm/teacher/pageList",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": [],
                 "statusList": [1, 0],
-                "page": {"pageNum": 1, "pageSize": 9999}
+                "page": {"pageNum": 1, "pageSize": 999}
             }
         )["data"]
 
     # 查询老师
     def teacher_query(self, name: str, status: int, size: int) -> list:
         """
         :return:
@@ -112,35 +112,36 @@
                 "campusIds": self.campus,
                 "queryKey": name,
                 "statusList": [status],
                 "page": {"pageNum": 1, "pageSize": size}
             }
         )["data"]
 
-    # 列出全部学生[最大99999条]
-    def student_listall(self) -> list:
+    # 列出全部学生
+    @loop
+    def student_listall(self, page, size):
         """
-        列出全部学生[最大99999条]
+        列出全部学生
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-crm/student/list",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "status": [],
                 "orgTag": 1,
-                "page": {"pageNum": 1, "pageSize": 99999}
+                "page": {"pageNum": page, "pageSize": size}
             }
-        )["data"]
+        )
 
     # 查询学生
     def student_query(self, curriculumids: list = None, classids: list = None, name: str = "",
-                      status: list = None, class_student_status: int = 0, size: int = 99999) -> list:
+                      status: list = None, class_student_status: int = 0, size: int = 999) -> list:
         """
         [教务管理/学员]
         列出学生
         :param size: 项目数量
         :param curriculumids: 课程筛选
         :param classids: 班级筛选
         :param name: 姓名查询关键字
@@ -163,32 +164,30 @@
                 "classIds": classids,
                 "classStudentStatus": class_student_status,
                 "orgTag": 1,
                 "page": {"pageNum": 1, "pageSize": size}
             }
         )["data"]
 
-    # 列出全部课程[最大9999条]
-    def curriculum_list_all(self) -> list:
+    # 列出全部课程
+    @loop
+    def curriculum_list_all(self, page, size):
         """
-        列出全部课程[最大9999条]
+        列出全部课程
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-edu/curriculum/pageList",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
-                "page": {
-                    "pageNum": 1,
-                    "pageSize": 9999
-                }
+                "page": {"pageNum": page, "pageSize": size}
             }
-        )["data"]
+        )
 
     # 查询课程
     def curriculum_query(self, searchname: str = None, haltsalelist: list = None, size: int = 9999) -> list:
         """
         查询所有在开的课程
         :param size:
         :param searchname: 查找关键字。
@@ -206,34 +205,35 @@
                 "page": {
                     "pageNum": 1,
                     "pageSize": size
                 }
             }
         )["data"]
 
-    # 列出指定日期范围全部排课[最大99999条]
-    def arrange_list_daterange(self, before_today: int, after_today: int) -> list:
+    # 列出指定日期范围全部排课
+    @loop
+    def arrange_list_daterange(self, page, size, before_today: int, after_today: int):
         """
-        列出全部排课[最大99999条]
+        列出全部排课
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-edu/arrange/page",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "startDate": time.strftime('%Y-%m-%d', time.localtime(time.time() - 86400 * before_today)),
                 "endDate": time.strftime('%Y-%m-%d', time.localtime(time.time() + 86400 * after_today)),
                 "displayCompletedClass": True,
-                "page": {"pageNum": 1, "pageSize": 99999}
+                "page": {"pageNum": page, "pageSize": size}
             }
-        )["data"]
+        )
 
-    # 列出指定日期全部排课[最大9999条]
+    # 列出指定日期全部排课[最大999条]
     def arrange_list_date(self, date: str = UsedTime.today) -> list:
         """
         列出日期范围全部排课[最大9999条]
         :param date:
         :return:
         """
         return self.request(
@@ -241,15 +241,15 @@
             url="https://yunxiao.xiaogj.com/api/cs-edu/arrange/getCompanyCourse",
             json={
                 "_t_": UsedTime.stamp,
                 "date": date,
                 "campusIds": self.campus,
                 "page": {
                     "pageNum": 1,
-                    "pageSize": 9999
+                    "pageSize": 999
                 }
             }
         )["data"]
 
     # 查询指定日期范围排课
     def arrange_query_daterange(self, starttime: str = None, endtime: str = None,
                                 displayCompletedClass=False, size: int = 99999) -> list:
@@ -338,29 +338,30 @@
                 "orderByCampus": 1,
                 "_t_": UsedTime.stamp
             }
         )["data"]["dataReportVos"]
         return list(map(lambda item: {**item, "id": f"{date}-{item['campusId']}"}, data_list))
 
     # 列出全部班级
-    def class_list_all(self) -> list:
+    @loop
+    def class_list_all(self, page, size):
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-edu/classInfo/page",
             json={
                 "_t_": UsedTime.stamp,
                 "orgTag": 1,
                 "campusIds": self.campus,
-                "page": {"pageNum": 1, "pageSize": 9999}
+                "page": {"pageNum": page, "pageSize": size}
             }
-        )["data"]
+        )
 
     # 列出指定上课日期范围的所有课消记录
     @loop("courseConsumeList")
-    def charge_record_list_daterange(self, startdate: str = "", enddate: str = "", page=0, size=1):
+    def charge_record_list_daterange(self, page, size, startdate: str = "", enddate: str = ""):
         """
         :param size: 每次取数据的分片量
         :param page: 从第几页开始取数据。应设为 0
         :param startdate: YY-MM-DD
         :param enddate: YY-MM-DD
         :return:
         """
@@ -374,15 +375,15 @@
                 "courseStartTime": startdate,
                 "courseEndTime": enddate
             }
         )
 
     # 列出指定上课日期范围的所有课消详情
     @loop("courseConsumeDetailList")
-    def charge_detail_list_daterange(self, startdate: str = "", enddate: str = "", page=1, size=1):
+    def charge_detail_list_daterange(self, page, size, startdate: str = "", enddate: str = ""):
         """
         :param size: 每次取数据的分片量
         :param page: 从第几页开始取数据。应设为 0
         :param startdate: YY-MM-DD
         :param enddate: YY-MM-DD
         :return:
         """
@@ -399,32 +400,35 @@
                 "curriculumIds": [],
                 "studentIds": [],
                 "teacherIds": []
             }
         )
 
     # 列出指定操作日期范围的所有订单记录
-    def order_item_list_all(self, startdate: str = "", enddate: str = "") -> list:
+    @loop("orderItemAllList")
+    def order_item_list_all(self, page, size, startdate: str = "", enddate: str = ""):
         """
         列出指定操作日期范围的所有订单记录
+        :param size: 每次取数据的分片量
+        :param page: 从第几页开始取数据。应设为 0
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/findOrderItemAll/page",
             json={
                 "_t_": UsedTime.stamp,
-                "page": {"pageNum": 1, "pageSize": 10000},
+                "page": {"pageNum": page, "pageSize": size},
                 "campusIds": self.campus,
                 "startTime": startdate,
                 "endTime": enddate
             }
-        )["data"]["orderItemAllList"]
+        )
 
     # 列出指定操作日期范围的所有退费详情
     def payment_refund_list_all(self, startdate: str = "", enddate: str = "") -> list:
         """
         列出指定操作日期范围的所有订单记录
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
@@ -480,29 +484,30 @@
                 "startTime": startdate,
                 "endTime": enddate,
                 "displayInvalidOrder": True
             }
         )["data"]
 
     # 列出所有课程卡
-    def card_list_all(self) -> list:
+    @loop
+    def card_list_all(self, page, size):
         """
         列出所有课程卡
         :return:
         """
         return self.request(
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/studentCourseCard/report",
             json={
                 "_t_": UsedTime.stamp,
-                "page": {"pageNum": 1, "pageSize": 100000},
+                "page": {"pageNum": page, "pageSize": size},
                 "campusIds": self.campus,
                 "displayHistory": True
             }
-        )["data"]
+        )
 
     # 列出所有招生来源选项
     def student_comefrom_select_item_list(self):
         return self.request(
             method="get",
             url=f"https://yunxiao.xiaogj.com/api/cs-crm/customField/get",
             params={"_t_": UsedTime.stamp, "customFieldId": "26118419"}
```

### Comparing `yunxiao-0.2.5/yunxiao/web.py` & `yunxiao-0.2.6/yunxiao/web.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.5/yunxiao/yunxiao.py` & `yunxiao-0.2.6/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.5/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.2.6/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.5
+Version: 0.2.6
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

