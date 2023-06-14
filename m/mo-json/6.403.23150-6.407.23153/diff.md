# Comparing `tmp/mo_json-6.403.23150-py2.py3-none-any.whl.zip` & `tmp/mo_json-6.407.23153-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 31606 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat    13329 b- defN 23-May-30 00:28 mo_json/__init__.py
+Zip file size: 32151 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat    14994 b- defN 23-Jun-02 01:41 mo_json/__init__.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-14 10:26 mo_json/decoder.py
 -rw-rw-rw-  2.0 fat    15429 b- defN 23-Apr-14 10:26 mo_json/encoder.py
 -rw-rw-rw-  2.0 fat    16185 b- defN 23-Apr-14 10:26 mo_json/stream.py
 -rw-rw-rw-  2.0 fat    17835 b- defN 23-May-04 10:50 mo_json/typed_encoder.py
 -rw-rw-rw-  2.0 fat     2896 b- defN 23-May-04 10:50 mo_json/typed_object.py
 -rw-rw-rw-  2.0 fat    10240 b- defN 23-Apr-30 12:14 mo_json/types.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11595 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      956 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/RECORD
-12 files, 105621 bytes uncompressed, 30024 bytes compressed:  71.6%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-02 01:41 mo_json-6.407.23153.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11595 b- defN 23-Jun-02 01:41 mo_json-6.407.23153.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-02 01:41 mo_json-6.407.23153.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-02 01:41 mo_json-6.407.23153.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      956 b- defN 23-Jun-02 01:41 mo_json-6.407.23153.dist-info/RECORD
+12 files, 107286 bytes uncompressed, 30569 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: mo_json/typed_object.py
 Comment: 
 
 Filename: mo_json/types.py
 Comment: 
 
-Filename: mo_json-6.403.23150.dist-info/LICENSE
+Filename: mo_json-6.407.23153.dist-info/LICENSE
 Comment: 
 
-Filename: mo_json-6.403.23150.dist-info/METADATA
+Filename: mo_json-6.407.23153.dist-info/METADATA
 Comment: 
 
-Filename: mo_json-6.403.23150.dist-info/WHEEL
+Filename: mo_json-6.407.23153.dist-info/WHEEL
 Comment: 
 
-Filename: mo_json-6.403.23150.dist-info/top_level.txt
+Filename: mo_json-6.407.23153.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_json-6.403.23150.dist-info/RECORD
+Filename: mo_json-6.407.23153.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_json/__init__.py

```diff
@@ -26,15 +26,15 @@
     integer_types,
     is_binary,
     is_text,
 )
 from mo_imports import delay_import
 from mo_json.types import *
 from mo_logs import Except, strings
-from mo_logs.strings import expand_template
+from mo_logs.strings import expand_template, toString, FORMATTERS
 from mo_times import Duration
 
 logger = delay_import("mo_logs.logger")
 
 FIND_LOOPS = True  # FIND LOOPS IN DATA STRUCTURES
 SNAP_TO_BASE_10 = False  # Identify floats near a round base10 value (has 000 or 999) and shorten
 CAN_NOT_DECODE_JSON = "Can not decode JSON"
@@ -357,15 +357,15 @@
     json_string = text(json_string)
     if not is_text(json_string) and json_string.__class__.__name__ != "FileString":
         logger.error("only unicode json accepted")
 
     try:
         if params:
             # LOOKUP REFERENCES
-            json_string = expand_template(json_string, params)
+            json_string = _simple_expand(json_string, (params, ))
 
         if flexible:
             value = hjson2value(json_string)
         else:
             value = to_data(json_decoder(text(json_string)))
 
         if leaves:
@@ -438,9 +438,59 @@
             logger.error(
                 "Can not convert {{value}} of type {{type}}", value=value, type=value.__class__,
             )
     except Exception as e:
         logger.error("Can not convert {{value}}", value=value, cause=e)
 
 
+_variable_pattern = re.compile(r"\{\{([\w_\.]+(\|[^\}^\|]+)*)\}\}")
+
+
+def _simple_expand(template, seq):
+    """
+    seq IS TUPLE OF OBJECTS IN PATH ORDER INTO THE DATA TREE
+    seq[-1] IS THE CURRENT CONTEXT
+    """
+
+    def replacer(found):
+        ops = found.group(1).split("|")
+
+        path = ops[0]
+        var = path.lstrip(".")
+        depth = min(len(seq), max(1, len(path) - len(var)))
+        try:
+            val = seq[-depth]
+            if var:
+                if is_sequence(val) and float(var) == round(float(var), 0):
+                    val = val[int(var)]
+                else:
+                    val = val[var]
+            for func_name in ops[1:]:
+                parts = func_name.split("(")
+                if len(parts) > 1:
+                    val = eval(parts[0] + "(val, " + "(".join(parts[1::]))
+                else:
+                    val = FORMATTERS[func_name](val)
+            val = toString(val)
+            return val
+        except Exception as cause:
+            from mo_logs import Except
+
+            cause = Except.wrap(cause)
+            try:
+                if cause.message.find("is not JSON serializable"):
+                    # WORK HARDER
+                    val = toString(val)
+                    return val
+            except Exception as f:
+                Log.warning(
+                    "Can not expand " + "|".join(ops) + " in template: {{template_|json}}",
+                    template_=template,
+                    cause=cause,
+                )
+            return "[template expansion error: (" + str(cause.message) + ")]"
+
+    return _variable_pattern.sub(replacer, template)
+
+
 from mo_json.decoder import json_decoder
 from mo_json.encoder import json_encoder, pypy_json_encode
```

## Comparing `mo_json-6.403.23150.dist-info/LICENSE` & `mo_json-6.407.23153.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_json-6.403.23150.dist-info/METADATA` & `mo_json-6.407.23153.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json
-Version: 6.403.23150
+Version: 6.407.23153
 Summary: More JSON Tools! 
 Home-page: https://github.com/klahnakoski/mo-json
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -15,16 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
 Requires-Dist: mo-dots (==9.401.23144)
 Requires-Dist: mo-future (==7.401.23144)
-Requires-Dist: mo-logs (==7.403.23150)
-Requires-Dist: mo-times (==5.403.23150)
+Requires-Dist: mo-logs (==8.407.23153)
+Requires-Dist: mo-times (==5.407.23153)
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 
 # More JSON Tools
```

## Comparing `mo_json-6.403.23150.dist-info/RECORD` & `mo_json-6.407.23153.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-mo_json/__init__.py,sha256=tfCrE8yLs0ESbkwwfbOeAh34-s6oc8HmBKMNt2Kr7e0,13329
+mo_json/__init__.py,sha256=W4Bc_NQlPQaM6r8rAhx-QFaeOwYutz8Dyyy7P72hqys,14994
 mo_json/decoder.py,sha256=iCE9aa_bwOCD6iDk461ywcHIBMJye-YIicGM6ILMlBk,313
 mo_json/encoder.py,sha256=PH8y_YEz9TSNhm1QJy2eW1PKUSPE2GdZwtHkASb18Js,15429
 mo_json/stream.py,sha256=DRbMb3IwpyW1s2J-Udws1wjCVCbaXGiXAa_7Ao9W4tI,16185
 mo_json/typed_encoder.py,sha256=ZLYbbeqgVbllDmxmQ4v83EM48w9hfdYnjK9q1R8mU0k,17835
 mo_json/typed_object.py,sha256=BAFhhVEdzsOIW6ZBEPlgaak7AnKr8UBIZzwxyGAsJGo,2896
 mo_json/types.py,sha256=VSLHgpQ8KF1iTXuqV0XTZILaLO28AGSrab_wdFLgo48,10240
-mo_json-6.403.23150.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_json-6.403.23150.dist-info/METADATA,sha256=PqFASI79Fe4Xm0CUCL7zp3pKpuCNxuZKqOfh1oUCqwo,11595
-mo_json-6.403.23150.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_json-6.403.23150.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
-mo_json-6.403.23150.dist-info/RECORD,,
+mo_json-6.407.23153.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_json-6.407.23153.dist-info/METADATA,sha256=Dzkf7fxPU6WF245dqIBQyE6xAwvob6o_G7TBcJGTVvc,11595
+mo_json-6.407.23153.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_json-6.407.23153.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
+mo_json-6.407.23153.dist-info/RECORD,,
```

