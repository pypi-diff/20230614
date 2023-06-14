# Comparing `tmp/smart_app_framework-2.2.0rc1-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.2.0rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 307125 bytes, number of entries: 334
+Zip file size: 307110 bytes, number of entries: 334
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -322,15 +322,15 @@
 -rw-r--r--  2.0 unx    13525 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/text2num.py
 -rw-r--r--  2.0 unx    24231 b- defN 80-Jan-01 00:00 smart_kit/text_preprocessing/utils.py
 -rw-r--r--  2.0 unx     8290 b- defN 80-Jan-01 00:00 smart_kit/utils/SmartAppToMessage_pb2.py
 -rw-r--r--  2.0 unx      486 b- defN 80-Jan-01 00:00 smart_kit/utils/__init__.py
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     2899 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
--rw-r--r--  2.0 unx     3385 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
+-rw-r--r--  2.0 unx     3322 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32375 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc1.dist-info/RECORD
-334 files, 987972 bytes uncompressed, 254343 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32375 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc2.dist-info/RECORD
+334 files, 987909 bytes uncompressed, 254328 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -987,17 +987,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc1.dist-info/METADATA
+Filename: smart_app_framework-2.2.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc1.dist-info/WHEEL
+Filename: smart_app_framework-2.2.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc1.dist-info/RECORD
+Filename: smart_app_framework-2.2.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smart_kit/utils/logger_writer/logger_formatter.py

```diff
@@ -58,35 +58,37 @@
             log_record["args"] = self._check_fields(record.args)
 
     def _check_fields(self, record_args: Dict[str, Any], types: Optional[Dict[str, dict]] = None):
         if types is None:
             types = self.fields_type
         if types is None:
             return record_args
+
+        new_args = {}
         for k, v in record_args.items():
             if k not in types or v is None:  # скипаем проверку если поля нет в конфиге, или value = None
+                new_args[k] = v
                 continue
             if types[k]["type"] == "dict":  # отдельно рекурсивно обрабатываем словари
                 if not isinstance(v, dict):  # преобразуем в строку в новое поле, если тип не соответсвует
-                    record_args[k] = "__del__"
-                    record_args[f"{k}__str"] = str(v)
+                    new_args[f"{k}__str"] = str(v)
                     continue
-                record_args[k] = self._check_fields(v, types[k]["fields"])
+                new_args[k] = self._check_fields(v, types[k]["fields"])
                 continue
             if isinstance(v, TYPES[types[k]["type"]]):  # noqa
+                new_args[k] = v
                 continue
 
             # пытаемся кастануть тип
             try:
-                record_args[k] = TYPE_CASTS[types[k]["type"]](v)
+                new_args[k] = TYPE_CASTS[types[k]["type"]](v)
             except (ValueError, TypeError):
-                record_args[k] = "__del__"
-                record_args[f"{k}__str"] = str(v)
+                new_args[f"{k}__str"] = str(v)
 
-        return {k: v for k, v in record_args.items() if v != "__del__"}
+        return new_args
 
     def format(self, record: logging.LogRecord) -> str:
         # В готовый json логов добавляем поле с размером json-а.
         result = super(SmartKitJsonFormatter, self).format(record)
         log_size = len(result)
         # Убираем последнюю закрывающую скобку и добавляем поле log_size и закрываем скобки
         return f'{result[:-1]},"log_size":{log_size}}}'
```

## Comparing `smart_app_framework-2.2.0rc1.dist-info/METADATA` & `smart_app_framework-2.2.0rc2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.2.0rc1
+Version: 2.2.0rc2
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

## Comparing `smart_app_framework-2.2.0rc1.dist-info/RECORD` & `smart_app_framework-2.2.0rc2.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -321,14 +321,14 @@
 smart_kit/text_preprocessing/text2num.py,sha256=5g5kSefNNtzwwiVyCfLvsCaoZTjqF8aAox9XRa_GuVQ,13525
 smart_kit/text_preprocessing/utils.py,sha256=MgLlYFmmCByWmNFBM_rf1RnvBZFQTvR_YCnlcEe0-A8,24231
 smart_kit/utils/SmartAppToMessage_pb2.py,sha256=PVabsQZGv0mQu5meCe8IWk0t3CcoJmVUIC83emQuYic,8290
 smart_kit/utils/__init__.py,sha256=CpZK3Ygk7w6USZDlrTu1GNjNlqboIm-Za_6eoGTbWuQ,486
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=rUdzi6f8mtXacNL6HvVYVoOnXD_M3FEMHFsMhPo0YL0,2899
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-smart_kit/utils/logger_writer/logger_formatter.py,sha256=bC7tdYW480irANhxaFxiKgnAsvmz-luf52WSu7ZjnIU,3385
+smart_kit/utils/logger_writer/logger_formatter.py,sha256=n5N4FHjXyeZAASjVB2zhoOMsbnWiixI0OQsk4KkcDFg,3322
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.2.0rc1.dist-info/METADATA,sha256=ffzo1oCWUmHOEcHICAuwfw-WfJAUk92gr_ukg-JR15E,10823
-smart_app_framework-2.2.0rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-smart_app_framework-2.2.0rc1.dist-info/RECORD,,
+smart_app_framework-2.2.0rc2.dist-info/METADATA,sha256=z9izWwgeVNoE0kvQOJOmyIDrRKS5rW8TeFHl9XmL9LY,10823
+smart_app_framework-2.2.0rc2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+smart_app_framework-2.2.0rc2.dist-info/RECORD,,
```

