# Comparing `tmp/WqUtils-0.0.3-py3-none-any.whl.zip` & `tmp/WqUtils-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2700 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2987 b- defN 22-Dec-30 10:43 WqUtils/Utils.py
+Zip file size: 2953 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     4334 b- defN 23-Jun-14 06:17 WqUtils/Utils.py
 -rw-r--r--  2.0 unx      250 b- defN 22-Nov-25 08:56 WqUtils/__init__.py
--rw-r--r--  2.0 unx      208 b- defN 23-Jan-05 05:52 WqUtils-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-05 05:52 WqUtils-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jan-05 05:52 WqUtils-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      444 b- defN 23-Jan-05 05:52 WqUtils-0.0.3.dist-info/RECORD
-6 files, 3989 bytes uncompressed, 1896 bytes compressed:  52.5%
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-14 06:18 WqUtils-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 06:18 WqUtils-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-14 06:18 WqUtils-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      444 b- defN 23-Jun-14 06:18 WqUtils-0.0.4.dist-info/RECORD
+6 files, 5289 bytes uncompressed, 2149 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: WqUtils/Utils.py
 Comment: 
 
 Filename: WqUtils/__init__.py
 Comment: 
 
-Filename: WqUtils-0.0.3.dist-info/METADATA
+Filename: WqUtils-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.0.3.dist-info/WHEEL
+Filename: WqUtils-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.0.3.dist-info/top_level.txt
+Filename: WqUtils-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: WqUtils-0.0.3.dist-info/RECORD
+Filename: WqUtils-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## WqUtils/Utils.py

```diff
@@ -15,62 +15,92 @@
 
 
 def get_base_file(name=None):
     base_path = os.path.dirname(os.path.abspath(name))
     return base_path
 
 
-class Log(object):
+class Singleton(type):
+    _instances = {}
+
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
+        return cls._instances[cls]
+
+
+class Log(metaclass=Singleton):
     def __init__(self, filename=None):
         """日志logger类"""
         # 创建logs文件夹
         self.file_name = filename
         cur_path = os.path.dirname(os.path.realpath(self.file_name))
         self.log_path = os.path.join(cur_path, 'logs')
         # 如果不存在这个logs文件夹，就自动创建一个
         if not os.path.exists(self.log_path): os.mkdir(self.log_path)
         # 文件的命名
         self.logname = os.path.join(self.log_path, f"{os.path.basename(self.file_name).split('.')[0]}.log")
+        self.log_name_error = os.path.join(self.log_path,
+                              f"{os.path.basename(self.file_name).split('.')[0]}-error.log")
         logging.basicConfig()
         self.logger = logging.getLogger(self.logname)
         self.logger.setLevel(logging.INFO)
         self.logger.propagate = False
         # 日志输出格式
-        self.formatter = logging.Formatter('[%(asctime)s] - %(filename)s] - %(levelname)s: %(message)s')
+        self.formatter = logging.Formatter('[%(asctime)s]-%(filename)s]-%(levelname)s:%(message)s')
 
     def __console(self, level, message):
         # 创建一个FileHandler，用于写到本地
         # fh = logging.FileHandler(self.logname, 'a', encoding='utf-8')
         # fh.setLevel(logging.INFO)
         # fh.setFormatter(self.formatter)
         # self.logger.addHandler(fh)
-        th = handlers.TimedRotatingFileHandler(filename=self.logname, interval=1, when='MIDNIGHT', backupCount=7,
+        th = handlers.TimedRotatingFileHandler(filename=self.logname, interval=1,
+                                               when='MIDNIGHT', backupCount=5,
                                                encoding='utf-8')
         th.suffix = "%Y-%m-%d.log"  # 设置文件后缀
+        info_filter = logging.Filter()
+        info_filter.filter = lambda record: record.levelno <= logging.WARNING  # 设置过滤等级
+        th.addFilter(info_filter)
         th.setFormatter(self.formatter)  # 设置文件里写入的格式
         self.logger.addHandler(th)
 
         # 创建一个StreamHandler,用于输出到控制台
-        ch = logging.StreamHandler()
-        ch.setLevel(logging.ERROR)
-        ch.setFormatter(self.formatter)
-        self.logger.addHandler(ch)
+        # ch = logging.StreamHandler()
+        # ch.setLevel(logging.ERROR)
+        # ch.setFormatter(self.formatter)
+        # self.logger.addHandler(ch)
+
+        # 创建TimedRotatingFileHandler,错误信息输出到对应文件
+        th_error = handlers.TimedRotatingFileHandler(filename=self.log_name_error,
+                                                  interval=1,
+                                               when='MIDNIGHT', backupCount=2,
+                                               encoding='utf-8')
+        th_error.suffix = "%Y-%m-%d.log"  # 设置文件后缀
+        th_error.setLevel(logging.ERROR)
+        th_error.setFormatter(self.formatter)  # 设置文件里写入的格式
+        self.logger.addHandler(th_error)
 
         if level == 'info':
             self.logger.info(message)
         elif level == 'debug':
             self.logger.debug(message)
         elif level == 'warning':
             self.logger.warning(message)
         elif level == 'error':
             self.logger.error(message)
         # 这两行代码是为了避免日志输出重复问题
-        self.logger.removeHandler(ch)
+        # self.logger.removeHandler(ch)
         self.logger.removeHandler(th)
+        self.logger.removeHandler(th_error)
 
+        # 关闭
+        # ch.close()
+        th.close()
+        th_error.close()
     def set_log_level(self, log_level=logging.INFO):
         self.logger.setLevel(log_level)
 
     def debug(self, message):
         self.__console('debug', message)
 
     def info(self, message):
@@ -81,7 +111,8 @@
 
     def error(self, message):
         self.__console('error', message)
 
 
 if __name__ == '__main__':
     print(get_base_file(__file__))
+
```

