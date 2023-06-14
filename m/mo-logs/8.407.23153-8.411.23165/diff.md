# Comparing `tmp/mo_logs-8.407.23153-py2.py3-none-any.whl.zip` & `tmp/mo_logs-8.411.23165-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 42724 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat    14801 b- defN 23-Jun-02 01:32 mo_logs/__init__.py
+Zip file size: 43030 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat    15496 b- defN 23-Jun-14 02:49 mo_logs/__init__.py
 -rw-rw-rw-  2.0 fat     2329 b- defN 23-Apr-30 18:00 mo_logs/constants.py
 -rw-rw-rw-  2.0 fat     2407 b- defN 23-May-30 00:22 mo_logs/convert.py
--rw-rw-rw-  2.0 fat     8766 b- defN 23-May-30 00:22 mo_logs/exceptions.py
+-rw-rw-rw-  2.0 fat     8762 b- defN 23-Jun-14 02:49 mo_logs/exceptions.py
 -rw-rw-rw-  2.0 fat     3524 b- defN 23-Apr-30 18:00 mo_logs/log_usingEmail.py
 -rw-rw-rw-  2.0 fat     1099 b- defN 23-Apr-30 18:00 mo_logs/log_usingFile.py
 -rw-rw-rw-  2.0 fat     3301 b- defN 23-May-09 22:44 mo_logs/log_usingHandler.py
 -rw-rw-rw-  2.0 fat     2013 b- defN 23-Apr-30 18:00 mo_logs/log_usingLogger.py
 -rw-rw-rw-  2.0 fat     2589 b- defN 23-Apr-30 18:00 mo_logs/log_usingMozLog.py
 -rw-rw-rw-  2.0 fat     1454 b- defN 23-Apr-30 18:00 mo_logs/log_usingMulti.py
 -rw-rw-rw-  2.0 fat      450 b- defN 23-Apr-30 18:00 mo_logs/log_usingNothing.py
 -rw-rw-rw-  2.0 fat     4069 b- defN 23-Apr-30 18:00 mo_logs/log_usingSES.py
 -rw-rw-rw-  2.0 fat     1525 b- defN 23-May-30 00:22 mo_logs/log_usingStream.py
 -rw-rw-rw-  2.0 fat     2325 b- defN 23-Apr-30 18:00 mo_logs/log_usingThread.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-May-30 00:22 mo_logs/startup.py
--rw-rw-rw-  2.0 fat    24689 b- defN 23-May-30 00:22 mo_logs/strings.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    17648 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1700 b- defN 23-Jun-02 01:32 mo_logs-8.407.23153.dist-info/RECORD
-21 files, 117842 bytes uncompressed, 39990 bytes compressed:  66.1%
+-rw-rw-rw-  2.0 fat    25364 b- defN 23-Jun-14 02:49 mo_logs/strings.py
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17648 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1700 b- defN 23-Jun-14 02:49 mo_logs-8.411.23165.dist-info/RECORD
+21 files, 119208 bytes uncompressed, 40296 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: mo_logs/startup.py
 Comment: 
 
 Filename: mo_logs/strings.py
 Comment: 
 
-Filename: mo_logs-8.407.23153.dist-info/LICENSE
+Filename: mo_logs-8.411.23165.dist-info/LICENSE
 Comment: 
 
-Filename: mo_logs-8.407.23153.dist-info/METADATA
+Filename: mo_logs-8.411.23165.dist-info/METADATA
 Comment: 
 
-Filename: mo_logs-8.407.23153.dist-info/WHEEL
+Filename: mo_logs-8.411.23165.dist-info/WHEEL
 Comment: 
 
-Filename: mo_logs-8.407.23153.dist-info/top_level.txt
+Filename: mo_logs-8.411.23165.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_logs-8.407.23153.dist-info/RECORD
+Filename: mo_logs-8.411.23165.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_logs/__init__.py

```diff
@@ -19,26 +19,29 @@
 from mo_logs import constants as _constants, exceptions, strings
 from mo_logs.exceptions import (
     Except,
     LogItem,
     suppress_exception,
     format_trace,
     WARNING,
+    get_stacktrace,
 )
 from mo_logs.log_usingStream import StructuredLogger_usingStream
 from mo_logs.strings import CR, indent
 
 STACKTRACE = "\n{trace_text|indent}\n{cause_text}"
 
 StructuredLogger_usingMulti = delay_import("mo_logs.log_usingMulti.StructuredLogger_usingMulti")
 StructuredLogger_usingThread = delay_import("mo_logs.log_usingThread.StructuredLogger_usingThread")
 
 _Thread = delay_import("mo_threads.Thread")
 startup_read_settings = delay_import("mo_logs.startup.read_settings")
 
+all_log_callers = {}
+
 
 class Log(object):
     """
     FOR STRUCTURED LOGGING AND EXCEPTION CHAINING
     """
 
     trace = False
@@ -196,15 +199,15 @@
         template: str,  # human readable string with placeholders for parameters
         default_params={},  # parameters to fill in template
         cause=None,  # for chaining
         *,
         stack_depth=0,  # how many calls you want popped off the stack to report the *true* caller
         log_severity=WARNING,  # set the logging severity
         exc_info=None,  # used by python logging as the cause
-        **more_params  # any more parameters (which will overwrite default_params)
+        **more_params,  # any more parameters (which will overwrite default_params)
     ):
         if exc_info is True:
             exc_type, exc_value, exc_traceback = sys.exc_info()
             exc_info = Except.wrap(exc_value)
         if not is_text(template):
             logger.error("logger.warning was expecting a string template")
         if "values" in more_params.keys():
@@ -228,15 +231,15 @@
         cls,
         template,  # human readable template
         default_params={},  # parameters for template
         *,
         cause=None,  # pausible cause
         stack_depth=0,
         exc_info=None,  # used by python logging as the cause
-        **more_params
+        **more_params,
     ):
         """
         raise an exception with a trace for the cause too
 
         :param template: *string* human readable string with placeholders for parameters
         :param default_params: *dict* parameters to fill in template
         :param cause: *Exception* for chaining
@@ -267,48 +270,58 @@
     @classmethod
     def _annotate(cls, item, stack_depth):
         """
         :param item:  A LogItem THE TYPE OF MESSAGE
         :param stack_depth: FOR TRACKING WHAT LINE THIS CAME FROM
         :return:
         """
-        template = item.template
-        template = strings.limit(template, 10000)
-        template = "".join(f"{text}{{params.{code}}}" for text, code in strings.parse_template(template))
+        given_template = item.template
+        given_template = strings.limit(given_template, 10000)
+        param_template = "".join(f"{text}{{params.{code}}}" for text, code in strings.parse_template(given_template))
 
         if isinstance(item, Except):
-            template = "{severity}: " + template + STACKTRACE
+            param_template = "{severity}: " + param_template + STACKTRACE
             temp = item.__data__()
             temp.trace_text = item.trace_text
             temp.cause_text = item.cause_text
             item = temp
         else:
             item = item.__data__()
 
-        if not template.startswith(CR) and CR in template:
-            template = CR + template
+        if not param_template.startswith(CR) and CR in param_template:
+            param_template = CR + param_template
 
         if cls.trace:
             item.machine = machine_metadata()
             log_format = item.template = (
                 "{machine.name} (pid {machine.pid}) - {timestamp|datetime} -"
-                ' {thread.name} - "{location.file}:{location.line}" -'
+                ' {thread.name} - ""{location.file}:{location.line}"" -'
                 " ({location.method}) - "
-                + template
+                + param_template
             )
             f = sys._getframe(stack_depth + 1)
             item.location = {
                 "line": f.f_lineno,
                 "file": f.f_code.co_filename,
                 "method": f.f_code.co_name,
             }
+            last_caller_loc = (f.f_code.co_filename, f.f_lineno)
+            prev_template = all_log_callers.get(last_caller_loc)
+            if prev_template != given_template:
+                if prev_template:
+                    raise Except(
+                        template="Expecting logger call to be static: was {a|quote} now {b|quote}",
+                        params={"a": prev_template, "b": given_template},
+                        trace=get_stacktrace(stack_depth + 1),
+                    )
+                all_log_callers[last_caller_loc] = given_template
             thread = _Thread.current()
             item.thread = {"name": thread.name, "id": thread.id}
         else:
-            log_format = template
+            log_format = param_template
             # log_format = item.template = "{timestamp|datetime} - " + template
 
         item.params = {**cls.extra, **item.params}
         cls.main_log.write(log_format, item)
 
     def write(self):
         raise NotImplementedError
```

## mo_logs/exceptions.py

```diff
@@ -207,15 +207,15 @@
         })
         tb = tb.tb_next
     trace.reverse()
     return trace
 
 
 def format_trace(tbs, start=0):
-    return "".join(expand_template('File "{{file}}", line {{line}}, in {{method}}\n', d) for d in tbs[start::])
+    return "".join(expand_template('File ""{file}"", line {line}, in {method}\n', d) for d in tbs[start::])
 
 
 class Suppress(object):
     """
     IGNORE EXCEPTIONS
     """
```

## mo_logs/strings.py

```diff
@@ -660,15 +660,15 @@
             try:
                 if cause.message.find("is not JSON serializable"):
                     # WORK HARDER
                     val = toString(val)
                     result.append(val)
             except Exception as f:
                 logger.warning(
-                    f"Can not expand {op}|{rest} in template: {{template_|json}}",
+                    f"Can not expand {op}|{rest} in template: {template_|json}",
                     template_=template,
                     cause=cause,
                 )
             result.append(f"[template expansion error: ({cause.message})]")
 
     return "".join(result)
 
@@ -876,51 +876,71 @@
     a = next(i)
 
     for b in i:
         yield (a, b)
         a = b
 
 
-body_pattern = re.compile(r"[^][)(}{\"']*")
+code_pattern = re.compile(r"[^][)(}{\"']*")
 bodies = {
-    "(": body_pattern,
-    "[": body_pattern,
-    "{": body_pattern,
+    "(": code_pattern,
+    "[": code_pattern,
+    "{": code_pattern,
     '"': re.compile(r'(\\"|[^"])*'),
     "'": re.compile(r"(\\'|[^'])*"),
 }
 closers = {
     ")": "(",
     "}": "{",
     "]": "[",
     '"': '"',
     "'": "'",
 }
 any_opener = re.compile(r'[\[{("\']')
+code_opener = re.compile(r'[{"\']')
 
 
 def parse_template(template):
     """
     WITH template = "a {b} c {d} e"
     RETURN LIST OF (str, code) PAIRS [("a ", b), (" c ", d), (" e", "")]
     """
 
     result = []
-    while "{" in template:
-        start = template.index("{")
-        text, code = template[:start], template[start:]
-        code, template = parse_code(code)
-        if code.startswith("{{") and code.endswith("}}"):
+
+    def append(prefix, code):
+        if result:
+            if not code or not prefix:
+                prev_prefix, prev_code = result[-1]
+                if not prev_code:
+                    result[-1] = (prev_prefix + prefix, code)
+                    return
+        result.append((prefix, code))
+
+    while True:
+        opener = code_opener.search(template)
+        if not opener:
+            if template:
+                append(template, "")
+            return result
+        i = opener.start()
+        prefix, residue = template[:i], template[i:]
+        code, template = parse_code(residue)
+        if code == '""':
+            append(prefix+'"', "")
+        elif code == "''":
+            append(prefix + "'", "")
+        elif code.startswith("{{") and code.endswith("}}"):
+        # STILL ALLOWING MOUSTACHES TO BE USED AS ESCAPE SEQUENCE
+            append(prefix, code[2:-2])
+        elif code.startswith("{") and code.endswith("}"):
             # STILL ALLOWING MOUSTACHES TO BE USED AS ESCAPE SEQUENCE
-            result.append((text, code[2:-2]))
+            append(prefix, code[1:-1])
         else:
-            result.append((text, code[1:-1]))
-    if template:
-        result.append((template, ""))
-    return result
+            append(prefix + code, "")
 
 
 def parse_code(code):
     """
     EXPECTING any_opener.match(code) TO BE TRUE
     """
     first, residue = code[0], code[1:]
```

## Comparing `mo_logs-8.407.23153.dist-info/LICENSE` & `mo_logs-8.411.23165.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_logs-8.407.23153.dist-info/METADATA` & `mo_logs-8.411.23165.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-logs
-Version: 8.407.23153
+Version: 8.411.23165
 Summary: More Logs! Structured Logging and Exception Handling
 Home-page: https://github.com/klahnakoski/mo-logs
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -12,18 +12,18 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots (==9.401.23144)
+Requires-Dist: mo-dots (==9.408.23161)
 Requires-Dist: mo-future (==7.401.23144)
-Requires-Dist: mo-imports (==7.401.23144)
-Requires-Dist: mo-kwargs (==7.403.23150)
+Requires-Dist: mo-imports (==7.408.23161)
+Requires-Dist: mo-kwargs (==7.409.23162)
 Provides-Extra: tests
 Requires-Dist: mo-json ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-kwargs ; extra == 'tests'
 Requires-Dist: jx-python ; extra == 'tests'
 Requires-Dist: boto ; extra == 'tests'
```

## Comparing `mo_logs-8.407.23153.dist-info/RECORD` & `mo_logs-8.411.23165.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-mo_logs/__init__.py,sha256=PZYfv6ooiGHmYppyksfFuXSsN5-qUcQyXd2HLD7_us8,14801
+mo_logs/__init__.py,sha256=KYKMsFdMyGXae7XHQX_OjOa23UNs9aLpAcAegWkLBQ4,15496
 mo_logs/constants.py,sha256=uYmXrreY2PJ4nXwFhRCySuqvBJmwRsrjFoTpy6dSf1I,2329
 mo_logs/convert.py,sha256=LjY9G-sgb64KctRkMQA2bYLMZj8iK226bwgS52wvMyA,2407
-mo_logs/exceptions.py,sha256=hrn-eoq8D69GiWw8t3O6V_lbTXySDt-ixI7kXhrtGWU,8766
+mo_logs/exceptions.py,sha256=T0zXkl5v-M0IOL5LmMOxGNGI_He565uGU4Fm9wq_2rs,8762
 mo_logs/log_usingEmail.py,sha256=R2wxQX0KolEQt_qtkwhISICAAlSQSU1Xus9iWaoDaW8,3524
 mo_logs/log_usingFile.py,sha256=wDRvM45WarKZqAfTZKqPkO6fleGwZaM0M_qFPRVmC-k,1099
 mo_logs/log_usingHandler.py,sha256=h67fvo7PJCKx85TrE-QOMCZe2lLyCvBHBcr6BUo-2Gs,3301
 mo_logs/log_usingLogger.py,sha256=4OOsUZPemh27cUOYdLetHuI9KmF47Ut0IRmdRU0p7EM,2013
 mo_logs/log_usingMozLog.py,sha256=lvWWbWSnt0MzwtrzJRBZVoNiolxLcnVYOKAjoXq9Oc4,2589
 mo_logs/log_usingMulti.py,sha256=2uUM3zHgpviKL5xJUIhi-5ReFEC51Zqv9-imi0xjBi0,1454
 mo_logs/log_usingNothing.py,sha256=RAJGGPwg4bw-eX4kDFT0kdEHH4hFsLicnJeq9Pf4Y3Q,450
 mo_logs/log_usingSES.py,sha256=hzfmQSiMnBudy4ptn73nGLUOXB-uhBXbOdUpv42HYjs,4069
 mo_logs/log_usingStream.py,sha256=t9q7Ju7F9wMKjReWXkUIcpkKRkiat2FHa---s8gdJ4s,1525
 mo_logs/log_usingThread.py,sha256=LbWlEBNGbjPBEFFIegmXhuT1_AA7H18Lv8YGDRVUpMc,2325
 mo_logs/startup.py,sha256=sMOxbRnsb-GPoMidGoTYAS9ooasv4BfwJRvyklY7fKM,6310
-mo_logs/strings.py,sha256=jo6J2Y5w2tjyOK2fMeIrfcSjBoMVgTFI6ZvY-80s2cc,24689
-mo_logs-8.407.23153.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_logs-8.407.23153.dist-info/METADATA,sha256=OEl8NQQKy4whgts9r4OihgY_Hlv3kllfcuIhnJjxVq4,17648
-mo_logs-8.407.23153.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_logs-8.407.23153.dist-info/top_level.txt,sha256=yqpeBBL3Yw2CDh1_FthlIK34KbT5cyZcAEjxlQ3MpDA,8
-mo_logs-8.407.23153.dist-info/RECORD,,
+mo_logs/strings.py,sha256=d63f-90qN-YlyqSDU8YqSS3HzcN18OT8zY-UMk6HF5I,25364
+mo_logs-8.411.23165.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_logs-8.411.23165.dist-info/METADATA,sha256=JkCYPImeOd4EVyhQh9xLp0RnEnpdlM7z2dQB-KAR9vY,17648
+mo_logs-8.411.23165.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_logs-8.411.23165.dist-info/top_level.txt,sha256=yqpeBBL3Yw2CDh1_FthlIK34KbT5cyZcAEjxlQ3MpDA,8
+mo_logs-8.411.23165.dist-info/RECORD,,
```

