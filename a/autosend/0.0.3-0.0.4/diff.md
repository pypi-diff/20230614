# Comparing `tmp/autosend-0.0.3-py3-none-any.whl.zip` & `tmp/autosend-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6295 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-15 07:56 autosend/__init__.py
--rw-rw-rw-  2.0 fat     8745 b- defN 23-May-15 10:29 autosend/autosend.py
--rw-rw-rw-  2.0 fat     1055 b- defN 23-May-15 10:41 autosend-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2388 b- defN 23-May-15 10:41 autosend-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 10:41 autosend-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-15 10:41 autosend-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      542 b- defN 23-May-15 10:41 autosend-0.0.3.dist-info/RECORD
-7 files, 12854 bytes uncompressed, 5333 bytes compressed:  58.5%
+Zip file size: 6457 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-14 06:14 autosend/__init__.py
+-rw-rw-rw-  2.0 fat     9269 b- defN 23-Jun-14 06:21 autosend/autosend.py
+-rw-rw-rw-  2.0 fat     1055 b- defN 23-Jun-14 06:22 autosend-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2388 b- defN 23-Jun-14 06:22 autosend-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 06:22 autosend-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-14 06:22 autosend-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      542 b- defN 23-Jun-14 06:22 autosend-0.0.4.dist-info/RECORD
+7 files, 13378 bytes uncompressed, 5495 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: autosend/__init__.py
 Comment: 
 
 Filename: autosend/autosend.py
 Comment: 
 
-Filename: autosend-0.0.3.dist-info/LICENSE
+Filename: autosend-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: autosend-0.0.3.dist-info/METADATA
+Filename: autosend-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: autosend-0.0.3.dist-info/WHEEL
+Filename: autosend-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: autosend-0.0.3.dist-info/top_level.txt
+Filename: autosend-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: autosend-0.0.3.dist-info/RECORD
+Filename: autosend-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## autosend/autosend.py

```diff
@@ -72,15 +72,15 @@
 '''
 
 def simulate_terminal_output(output_str):
     width = 140
     current_pos = 0
     lines = []
     current_line = ""
-    
+
     # Iterate through each character in the input string
     for char in output_str:
         # Handle control characters
         if char == '\b':
             if current_pos > 0:
                 current_pos -= 1
                 current_line = current_line[:-1]
@@ -138,38 +138,44 @@
         self.start_time_str=time.strftime('%Y-%m-%d %H:%M', time.localtime(self.start_time))
         self.log_start_time=time.time()
         self.args='; '.join(sys.argv)
         self.cwd = os.getcwd()
         self.should_send = False
 
         self.path=os.path.basename(os.getcwd())
-        self.__stdout__ = sys.stdout
-        self.__stderr__ = sys.stderr
+        for func in 'write','writelines','flush':
+            self.wrap_writer(sys.stdout,func)
+            self.wrap_writer(sys.stderr,func)
+
         print('#autosend: starting log')
-        sys.stdout = self
-        sys.stderr = self
+
         atexit.register(self.__del__)
 
     def read_config(self,path):
         with open(os.path.expanduser(path), "r", encoding='utf-8') as stream:
             return yaml.safe_load(stream)
 
-
-    def write(self, text):
-        self.buffer.write(text)
-        sys.__stdout__.write(text)
-        self.check()
-
-    def writelines(self,texts,/):
-        self.buffer.writelines(texts)
-        sys.__stdout__.writelines(texts)
-        self.check()
+    def write(self,obj):
+        sys.stderr._raw_write(obj)
 
     def flush(self):
-        sys.__stdout__.flush()
+        sys.stderr._raw_flush()
+
+    def wrap_writer(self,obj,func_name,wrap_back=False):
+        if wrap_back:
+            setattr(obj, func_name,getattr(obj,'_raw_' + func_name))
+            return
+        setattr(obj,'_raw_'+func_name,getattr(obj,func_name))
+        def func(*arg,**kwargs):
+            #self.write('--{} -- {} -|-\n'.format(arg,kwargs))
+            getattr(self.buffer,func_name)(*arg,**kwargs)
+            value=getattr(obj,'_raw_'+func_name)(*arg,**kwargs)
+            self.check()
+            return value
+        setattr(obj,func_name,func)
 
     def check(self):
         elapsed_time = time.time() - self.log_start_time
         self.should_send = time.time() - self.start_time > self.send_after_seconds
         if elapsed_time > self.send_periods:
             self.send_logs('running')
 
@@ -201,47 +207,49 @@
         smtp_server.login(username, password)
         smtp_server.sendmail(sender, receivers, msg.as_string())
         smtp_server.quit()
 
     def send_logs(self, status=''):
         if not self.should_send:
             return
-        self.__stderr__.write('#autosend: sending log\n')
-        self.__stderr__.flush()
+        self.write('#autosend: sending log\n')
+        self.flush()
 
         text_lines = simulate_terminal_output(self.buffer.getvalue())
         if self.clear_after_send:
-            self.buffer = StringIO() 
+            self.buffer = StringIO()
         self.log_start_time = time.time()
         try:
             subject = self.sbj_fmt.format(
                 path=self.path,
                 curtime=self.start_time_str,
                 status = status,
             )
             meta_info=[
                 ' start_time: ' + self.start_time_str,
                 'last update: ' + time.strftime('%Y-%m-%d %H:%M'),
                 '   work_dir: ' + self.cwd,
                 '       args: ' + self.args,
                 '================= last 100 lines of the log ================='
             ]
-            body=lines_to_text(meta_info + text_lines[-100:],plain=not self.html)
+            body=lines_to_text(simulate_terminal_output('\n'.join(meta_info)) + text_lines[-100:],plain=not self.html)
             attachments = [(f"logs_{time.strftime('%Y-%m-%d-%H-%M')}.txt", '\n'.join(text_lines))]
             self.send_email(subject, body, attachments)
 
         except Exception:
-            self.__stderr__.write('#autosend: email sending failed:\n')
-            self.__stderr__.write(traceback.format_exc())
-            self.__stderr__.flush()
+            self.write('#autosend: email sending failed:\n')
+            self.write(traceback.format_exc())
+            self.flush()
+        self.write('#autosend: sucessfully send the log\n')
 
     def __del__(self):
         if not self.enabled:
             return
         self.enabled=False
         self.send_logs('completed')
-        sys.stdout = self.__stdout__
-        sys.stderr = self.__stderr__
+        for func in 'write', 'writelines', 'flush':
+            self.wrap_writer(sys.stdout, func,wrap_back=True)
+            self.wrap_writer(sys.stderr, func,wrap_back=True)
 
-if int(os.environ.get('LOCAL_RANK',os.environ.get('RANK',0)))==0:
+if int(os.environ.get('LOCAL_RANK',os.environ.get('RANK',0)))==0 and not sys.gettrace():
     logger = TextIOWrapperWithLogging()
```

## Comparing `autosend-0.0.3.dist-info/LICENSE` & `autosend-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `autosend-0.0.3.dist-info/METADATA` & `autosend-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosend
-Version: 0.0.3
+Version: 0.0.4
 Summary: a simple tool that logs what is printed on the screen, and emails the logs to you
 Home-page: https://github.com/flishwang/autosend
 Author: flish_wang
 Author-email: flish_wang@sina.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `autosend-0.0.3.dist-info/RECORD` & `autosend-0.0.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 autosend/__init__.py,sha256=pIlNw8q7mTGMy7blog4Ji1AOfCu0sZ4r2CJd0B5JFk4,23
-autosend/autosend.py,sha256=RLHfsNLFcbl1-48wT5-k7lYneqfn_Wr6GFFG4RNXNXo,8745
-autosend-0.0.3.dist-info/LICENSE,sha256=ua2oZFI3AQveS_KUg4JiVBxwsfi7lHzCQMsboXaPfyc,1055
-autosend-0.0.3.dist-info/METADATA,sha256=9D1M1yzD4HFOaiaAokjcI9G9IsRMW6oUQeSJo7p4GVk,2388
-autosend-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-autosend-0.0.3.dist-info/top_level.txt,sha256=ZCgzjZrZThmJFpfzdLiab-y_aTzpyZ6LDf0mHbU7FSU,9
-autosend-0.0.3.dist-info/RECORD,,
+autosend/autosend.py,sha256=54Vn6Ak-j71u-bDxPwzTkARXRkDz1qah9vFAMwQs1ck,9269
+autosend-0.0.4.dist-info/LICENSE,sha256=ua2oZFI3AQveS_KUg4JiVBxwsfi7lHzCQMsboXaPfyc,1055
+autosend-0.0.4.dist-info/METADATA,sha256=jOdGffnQ9Shzf_Ri8lOUjqCEoUEkpwRSeZRnaYI8yIU,2388
+autosend-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+autosend-0.0.4.dist-info/top_level.txt,sha256=ZCgzjZrZThmJFpfzdLiab-y_aTzpyZ6LDf0mHbU7FSU,9
+autosend-0.0.4.dist-info/RECORD,,
```

