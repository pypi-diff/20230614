# Comparing `tmp/ats_case-0.8.1.tar.gz` & `tmp/ats_case-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.8.1.tar", last modified: Mon May 29 02:27:05 2023, max compression
+gzip compressed data, was "ats_case-0.8.2.tar", last modified: Tue May 30 00:58:05 2023, max compression
```

## Comparing `ats_case-0.8.1.tar` & `ats_case-0.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.236610 ats_case-0.8.1/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.1/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-05-29 02:27:05.234616 ats_case-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 02:27:04.752906 ats_case-0.8.1/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.1/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.045122 ats_case-0.8.1/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.1/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18705 2023-05-22 07:49:46.000000 ats_case-0.8.1/ats_case/case/command.py
--rw-rw-rw-   0        0        0    11367 2023-05-29 02:26:57.000000 ats_case-0.8.1/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.8.1/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.1/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.124909 ats_case-0.8.1/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.1/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.1/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.1/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.186743 ats_case-0.8.1/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.1/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.1/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.8.1/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.219654 ats_case-0.8.1/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.1/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.1/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-05-29 02:27:04.875580 ats_case-0.8.1/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-05-29 02:27:03.000000 ats_case-0.8.1/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-05-29 02:27:04.000000 ats_case-0.8.1/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 02:27:03.000000 ats_case-0.8.1/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-29 02:27:03.000000 ats_case-0.8.1/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 02:27:03.000000 ats_case-0.8.1/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 02:27:05.236610 ats_case-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-05-29 02:26:57.000000 ats_case-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.594403 ats_case-0.8.2/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.2/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-05-30 00:58:05.592409 ats_case-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.189480 ats_case-0.8.2/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.2/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.406902 ats_case-0.8.2/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.2/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18767 2023-05-30 00:52:23.000000 ats_case-0.8.2/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    11494 2023-05-30 00:50:05.000000 ats_case-0.8.2/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.8.2/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.2/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.486689 ats_case-0.8.2/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.2/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.2/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.2/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.548525 ats_case-0.8.2/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.2/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.2/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3771 2023-05-30 00:49:20.000000 ats_case-0.8.2/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.583432 ats_case-0.8.2/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.2/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.2/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-05-30 00:58:05.287221 ats_case-0.8.2/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 00:58:04.000000 ats_case-0.8.2/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 00:58:05.594403 ats_case-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-05-30 00:57:57.000000 ats_case-0.8.2/setup.py
```

### Comparing `ats_case-0.8.1/PKG-INFO` & `ats_case-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.8.1
+Version: 0.8.2
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.1/README.md` & `ats_case-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.1/ats_case/case/command.py` & `ats_case-0.8.2/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,23 +477,24 @@
         if self._interval > 0:
             if context.runtime.loop_index == 0 or (context.runtime.loop_index + 1) % self._interval != 0:
                 return
 
         self._exec_times += 1
 
     def exec(self, context: Context):
-        self._times(context)
+        if context.meter.index == 0:
+            self._times(context)
 
-        self.encode(context)
-        self._result = send(context, todo={'bench:{}'.format(self._operation): self._parameter})
-        self.decode(context)
+            self.encode(context)
+            self._result = send(context, todo={'bench:{}'.format(self._operation): self._parameter})
+            self.decode(context)
 
-        send(context, todo={'app:show': {'msg': self.acv(context)}})
+            send(context, todo={'app:show': {'msg': self.acv(context)}})
 
-        self.rest(context)
+            self.rest(context)
 
 
 """
     测试终端篇
 """
```

### Comparing `ats_case-0.8.1/ats_case/case/context.py` & `ats_case-0.8.2/ats_case/case/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
     #
     #     @property
     #     def req_params(self):
     #         return self._req_params
 
     class Meter(object):
         def __init__(self, data: dict):
+            self._index = data.get('index', 0)
             self._pos = data.get('pos')
             self._addr = data.get('addr')
             self._no = data.get('no')
             self._protocol = data.get('protocol')
             self._model = data.get('model')
             self._connect = data.get('connect')
             self._rated_voltage = data.get('rated_voltage')
@@ -229,14 +230,18 @@
         #         self._channel = {'RS485': data.get('baudrate_485'), 'IR': data.get('baudrate_ir'),
         #                          'PLC': data.get('baudrate_plc')}
         #
         #     def get_channel(self, c: CHANNEL):
         #         return func.to_dict(type=c.value, baudrate=self._channel.get(c.value))
 
         @property
+        def index(self):
+            return self._index
+
+        @property
         def pos(self):
             return self._pos
 
         @property
         def addr(self):
             return self._addr
 
@@ -322,15 +327,15 @@
                     fc += 1
                     fs.append(str(s))
                 else:
                     sc += 1
 
             msg = '步骤: {}步\r\n'.format(len(self._acvs))
             msg += '合格: {}步\r\n'.format(sc)
-            msg += '不合格: {}步 - {}\r\n'.format(fc, ','.join(fs))
+            msg += '不合格: {}步 ~ {}\r\n'.format(fc, ','.join(fs))
 
             return msg
 
         @property
         def step(self):
             return self._step
```

### Comparing `ats_case-0.8.1/ats_case/case/executor.py` & `ats_case-0.8.2/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.1/ats_case/case/translator.py` & `ats_case-0.8.2/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.1/ats_case/common/error.py` & `ats_case-0.8.2/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.1/ats_case/manage/core.py` & `ats_case-0.8.2/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.1/ats_case/manage/start.py` & `ats_case-0.8.2/ats_case/manage/start.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             self._sn = self._username.upper() + self._now
             mm.Dict.put('test:log', self._sn, self._data)
             self._save()
         else:  # 断点续测
             self._data = mm.Dict.get('test:log', self._sn)
             self._data['renew'] = 1
 
-        self._cases = self._data.get('cases', [])
+        self._cases = self._data.get('usercases', [])
         self.meters = self._data.get('meters', [])
 
     def _save(self):
         pass  # 存数据库
 
     def run(self):
         while self._cases:
@@ -84,17 +84,19 @@
         def __init__(self, parent, case):
             super(FormalMode.CaseTask, self).__init__()
             self._parent = parent
             self._case = case
 
         def run(self):
             gs = []
-            for meter in self._parent.meters:
+            for i in range(len(self._parent.meters)):
                 # i = 0 执行操作表台 传入参数index
-                gs.append(gevent.spawn(self._parent.exec, self._parent.flush(case=self._case, meter=meter)))
+                self._parent.meters[i]['index'] = i
+                gs.append(gevent.spawn(self._parent.exec, self._parent.flush(case=self._case,
+                                                                             meter=self._parent.meters[i])))
 
             gevent.joinall(gs)
 
     def flush(self, case, meter):
         self._data['usercase'] = case
         self._data['meter'] = meter
```

### Comparing `ats_case-0.8.1/ats_case/template/testcase_v1.tmp` & `ats_case-0.8.2/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.1/ats_case.egg-info/PKG-INFO` & `ats_case-0.8.2/ats_case.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.8.1
+Version: 0.8.2
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.1/ats_case.egg-info/SOURCES.txt` & `ats_case-0.8.2/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.1/setup.py` & `ats_case-0.8.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.8.1",
+    version="0.8.2",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

