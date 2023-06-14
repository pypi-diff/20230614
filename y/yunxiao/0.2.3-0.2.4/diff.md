# Comparing `tmp/yunxiao-0.2.3.tar.gz` & `tmp/yunxiao-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.2.3.tar", last modified: Mon Jun 12 20:59:39 2023, max compression
+gzip compressed data, was "yunxiao-0.2.4.tar", last modified: Mon Jun 12 22:17:32 2023, max compression
```

## Comparing `yunxiao-0.2.3.tar` & `yunxiao-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 20:59:39.390273 yunxiao-0.2.3/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    12954 2023-06-12 20:59:39.389265 yunxiao-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.3/README.md
--rw-rw-rw-   0        0        0     1031 2023-06-12 20:59:24.000000 yunxiao-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 20:59:39.390273 yunxiao-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 20:59:39.377084 yunxiao-0.2.3/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.3/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:59:39.382154 yunxiao-0.2.3/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.3/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.3/yunxiao/app.py
--rw-rw-rw-   0        0        0    17304 2023-06-12 20:58:35.000000 yunxiao-0.2.3/yunxiao/v2.py
--rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.3/yunxiao/web.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.3/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:59:39.388258 yunxiao-0.2.3/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    12954 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 22:17:32.101138 yunxiao-0.2.4/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0    12954 2023-06-12 22:17:32.101138 yunxiao-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.4/README.md
+-rw-rw-rw-   0        0        0     1100 2023-06-12 22:16:58.000000 yunxiao-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 22:17:32.101138 yunxiao-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 22:17:32.090017 yunxiao-0.2.4/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:17:32.095072 yunxiao-0.2.4/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.4/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.4/yunxiao/app.py
+-rw-rw-rw-   0        0        0    17196 2023-06-12 22:14:20.000000 yunxiao-0.2.4/yunxiao/v2.py
+-rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.4/yunxiao/web.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.4/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:17:32.100131 yunxiao-0.2.4/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    12954 2023-06-12 22:17:32.000000 yunxiao-0.2.4/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-12 22:17:32.000000 yunxiao-0.2.4/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 22:17:32.000000 yunxiao-0.2.4/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 22:17:32.000000 yunxiao-0.2.4/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 22:17:32.000000 yunxiao-0.2.4/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.2.3/LICENSE` & `yunxiao-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.3/PKG-INFO` & `yunxiao-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.3
+Version: 0.2.4
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.2.3/README.md` & `yunxiao-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.3/pyproject.toml` & `yunxiao-0.2.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.2.3"
+version = "0.2.4"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,11 +22,12 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.2.4" = "修复 v2 中一个API端点错误及鉴权更新错误"
 "0.2.2" = "新增 v2, 更清晰的函数命名，简洁快速的拉取全部数据。"
 "0.2.1" = "web 端请求 BUG 修复"
 "0.2.0" = "BUG修复"
 "0.1.9" = "更改鉴权方式，保存鉴权到系统环境变量。当因鉴权失效导致请求失败时，自动更新鉴权并重新发起请求。意图减少更新鉴权的次数。"
```

### Comparing `yunxiao-0.2.3/yunxiao/app.py` & `yunxiao-0.2.4/yunxiao/app.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.3/yunxiao/v2.py` & `yunxiao-0.2.4/yunxiao/v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         """
         super().__init__(configfile)
         if campus is None:
             self.campus = []
         else:
             self.campus = campus
 
-        self.reportpath = "https://yunxiao.xiaogj.com/api/cs-report/report/"
         self.orderpath = "https://yunxiao.xiaogj.com/api/cs-edu/order"
         self.edupath = "https://yunxiao.xiaogj.com/api/cs-edu/"
         self.crmpath = "https://yunxiao.xiaogj.com/api/cs-crm/"
 
     def request(self, **kwargs) -> dict:
         response = requests.request(
             method=kwargs.get("method"),
@@ -34,15 +33,18 @@
 
         if response.status_code != 200:
             logging.error("无法到连接云校服务器。")
             return {"data": "无法到连接云校服务器。"}
 
         if response.json()["code"] == 401:
             logging.error(response.json()["msg"])
-            self.renew_token()
+            if "cs-pc-" in kwargs.get("url"):
+                self.renew_cookie()
+            else:
+                self.renew_token()
             response = requests.request(
                 method=kwargs.get("method"),
                 url=kwargs.get("url"),
                 json=kwargs.get("json"),
                 params=kwargs.get("params"),
                 headers={"x3-authentication": self.token, "Cookie": self.cookie}
             )
@@ -76,15 +78,15 @@
     # 查询老师
     def teacher_query(self, name: str, status: int, size: int) -> list:
         """
         :return:
         """
         return self.request(
             method="post",
-            url=self.crmpath + "teacher/pageList",
+            url="https://yunxiao.xiaogj.com/api/cs-crm/teacher/pageList",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "queryKey": name,
                 "statusList": [status],
                 "page": {"pageNum": 1, "pageSize": size}
             }
@@ -122,15 +124,15 @@
         :param class_student_status: 0>不筛选 1>未入班 2>已入班
         :return:
         """
         if status is None:
             status = [1, 7]
         return self.request(
             method="post",
-            url=self.crmpath + "student/list",
+            url="https://yunxiao.xiaogj.com/api/cs-crm/student/list",
             json={
                 "_t_": UsedTime.stamp,
                 "name": name,
                 "campusIds": self.campus,
                 "status": status,
                 "intentionStatus": 0,
                 "curriculumIds": curriculumids,
@@ -145,15 +147,15 @@
     def curriculum_list_all(self) -> list:
         """
         列出全部课程[最大9999条]
         :return:
         """
         return self.request(
             method="post",
-            url=self.edupath + "curriculum/pageList",
+            url="https://yunxiao.xiaogj.com/api/cs-edu/curriculum/pageList",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "page": {
                     "pageNum": 1,
                     "pageSize": 9999
                 }
@@ -167,15 +169,15 @@
         :param size:
         :param searchname: 查找关键字。
         :param haltsalelist: 是否在售。0>在售 1>停售
         :return:
         """
         return self.request(
             method="post",
-            url=self.edupath + "curriculum/pageList",
+            url="https://yunxiao.xiaogj.com/api/cs-edu/curriculum/pageList",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "curriculumName": searchname,
                 "haltSaleList": haltsalelist,
                 "page": {
                     "pageNum": 1,
@@ -233,15 +235,15 @@
         :param size:
         :param starttime: 查询起始时间
         :param endtime: 查询截止时间
         :return:
         """
         return self.request(
             method="post",
-            url=self.edupath + "arrange/page",
+            url="https://yunxiao.xiaogj.com/api/cs-edu/arrange/page",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "startDate": starttime,
                 "endDate": endtime,
                 "displayCompletedClass": displayCompletedClass,
                 "page": {"pageNum": 1, "pageSize": size}
@@ -279,21 +281,21 @@
             method="post",
             url="https://yunxiao.xiaogj.com/api/cs-report/report/findCourseMoney",
             json={"campusIds": self.campus, "date": yy_mm, "dateType": 1, "_t_": UsedTime.stamp}
         )["data"]
 
         refund = self.request(
             method="post",
-            url=self.reportpath + "findRefundMoney",
+            url="https://yunxiao.xiaogj.com/api/cs-report/report/findRefundMoney",
             json={"campusIds": self.campus, "date": yy_mm, "dateType": 1, "_t_": UsedTime.stamp}
         )["data"]
 
         tuition = self.request(
             method="post",
-            url=self.reportpath + "findTuition",
+            url="https://yunxiao.xiaogj.com/api/cs-report/report/findTuition",
             json={"campusIds": self.campus, "date": yy_mm, "dateType": 1, "_t_": UsedTime.stamp}
         )["data"]
 
         return list(map(lambda x: {**x[0], **x[1], **x[2]}, zip(course, refund, tuition)))
 
     # 分校区列出指定日期的费用数据
     def campus_todaymoney_list_all(self, date: str = UsedTime.today) -> list:
@@ -374,15 +376,15 @@
         列出指定操作日期范围的所有订单记录
         :param enddate: YY-MM-DD
         :param startdate: YY-MM-DD
         :return:
         """
         return self.request(
             method="post",
-            url="https://yunxiao.xiaogj.com/api/cs-report/report/findOrderItemAll/page",
+            url="https://yunxiao.xiaogj.com/api/cs-pc-report/report/findOrderItemAll/page",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": 1, "pageSize": 10000},
                 "campusIds": self.campus,
                 "startTime": startdate,
                 "endTime": enddate
             }
@@ -453,15 +455,15 @@
     def card_list_all(self) -> list:
         """
         列出所有课程卡
         :return:
         """
         return self.request(
             method="post",
-            url="https://yunxiao.xiaogj.com/api/cs-report/report/studentCourseCard/report",
+            url="https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/studentCourseCard/report",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": 1, "pageSize": 100000},
                 "campusIds": self.campus,
                 "displayHistory": True
             }
         )["data"]
@@ -469,15 +471,7 @@
     # 列出所有招生来源选项
     def student_comefrom_select_item_list(self):
         return self.request(
             method="get",
             url=f"https://yunxiao.xiaogj.com/api/cs-crm/customField/get",
             params={"_t_": UsedTime.stamp, "customFieldId": "26118419"}
         )["data"]["selectItemList"]
-
-    # 列出所有公立年级选项
-    def student_grade_select_item_list(self):
-        return self.request(
-            method="get",
-            url=f"https://yunxiao.xiaogj.com/api/cs-crm/customField/get",
-            params={"_t_": UsedTime.stamp, "customFieldId": "26118418"}
-        )["data"]["selectItemList"]
```

### Comparing `yunxiao-0.2.3/yunxiao/web.py` & `yunxiao-0.2.4/yunxiao/web.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.3/yunxiao/yunxiao.py` & `yunxiao-0.2.4/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.3/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.2.4/yunxiao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.3
+Version: 0.2.4
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

