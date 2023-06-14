# Comparing `tmp/WqUtils-0.0.4-py3-none-any.whl.zip` & `tmp/WqUtils-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2953 bytes, number of entries: 6
--rw-r--r--  2.0 unx     4334 b- defN 23-Jun-14 06:17 WqUtils/Utils.py
+Zip file size: 2985 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     4339 b- defN 23-Jun-14 09:18 WqUtils/Utils.py
 -rw-r--r--  2.0 unx      250 b- defN 22-Nov-25 08:56 WqUtils/__init__.py
--rw-r--r--  2.0 unx      161 b- defN 23-Jun-14 06:18 WqUtils-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 06:18 WqUtils-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-14 06:18 WqUtils-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      444 b- defN 23-Jun-14 06:18 WqUtils-0.0.4.dist-info/RECORD
-6 files, 5289 bytes uncompressed, 2149 bytes compressed:  59.4%
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-14 09:32 WqUtils-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 09:32 WqUtils-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-14 09:32 WqUtils-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      444 b- defN 23-Jun-14 09:32 WqUtils-0.0.5.dist-info/RECORD
+6 files, 5341 bytes uncompressed, 2181 bytes compressed:  59.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: WqUtils/Utils.py
 Comment: 
 
 Filename: WqUtils/__init__.py
 Comment: 
 
-Filename: WqUtils-0.0.4.dist-info/METADATA
+Filename: WqUtils-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.0.4.dist-info/WHEEL
+Filename: WqUtils-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.0.4.dist-info/top_level.txt
+Filename: WqUtils-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: WqUtils-0.0.4.dist-info/RECORD
+Filename: WqUtils-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## WqUtils/Utils.py

```diff
@@ -91,16 +91,17 @@
         # 这两行代码是为了避免日志输出重复问题
         # self.logger.removeHandler(ch)
         self.logger.removeHandler(th)
         self.logger.removeHandler(th_error)
 
         # 关闭
         # ch.close()
-        th.close()
-        th_error.close()
+        # th.close()
+        # th_error.close()
+
     def set_log_level(self, log_level=logging.INFO):
         self.logger.setLevel(log_level)
 
     def debug(self, message):
         self.__console('debug', message)
 
     def info(self, message):
```

