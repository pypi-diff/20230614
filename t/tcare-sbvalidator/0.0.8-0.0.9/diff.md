# Comparing `tmp/tcare_sbvalidator-0.0.8.tar.gz` & `tmp/tcare_sbvalidator-0.0.9.tar.gz`

## Comparing `tcare_sbvalidator-0.0.8.tar` & `tcare_sbvalidator-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/Makefile
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/reqs.txt
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/requirements.txt
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/test.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/test2.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/uploadkey
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/__init__.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/sb_validator.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/sms_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/models/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/models/cloudevents.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/Makefile
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/reqs.txt
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/test.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/test2.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/uploadkey
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/src/tcare_sbvalidator/__init__.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/src/tcare_sbvalidator/sb_validator.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/src/tcare_sbvalidator/sms_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/src/tcare_sbvalidator/models/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/src/tcare_sbvalidator/models/cloudevents.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 tcare_sbvalidator-0.0.9/PKG-INFO
```

### Comparing `tcare_sbvalidator-0.0.8/requirements.txt` & `tcare_sbvalidator-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.8/test.py` & `tcare_sbvalidator-0.0.9/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 async def main():
     handler = Sms()
 
     json = handler.build_json(
         id="123",
         recipient="+15713024423",
         sender="+18722782273",
-        content="Hey!"
+        content="Helloo!"
     )
 
     await handler.publish_message(NAMESPACE, TOPIC, json)
 
 asyncio.run(main())
```

### Comparing `tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/sb_validator.py` & `tcare_sbvalidator-0.0.9/src/tcare_sbvalidator/sb_validator.py`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.8/src/tcare_sbvalidator/sms_handler.py` & `tcare_sbvalidator-0.0.9/src/tcare_sbvalidator/sms_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,13 +26,13 @@
                     "sender": sender
                 },
                 "options": options,
             }, default=str)
         except Exception as e:
             print(e)
 
-    async def publish_message(self, namespace, topic, message, cred=DefaultAzureCredential()):
+    async def publish_message(self, namespace, topic, message_json, cred=DefaultAzureCredential()):
         async with ServiceBusClient(namespace, cred) as client:
             async with client.get_topic_sender(topic) as sender:
-                msg = ServiceBusMessage(message)
+                msg = ServiceBusMessage(message_json)
                 await sender.send_messages(msg)
-                print(f"message sent with content: {message}")
+                print(f"message sent with content: {message_json}")
```

### Comparing `tcare_sbvalidator-0.0.8/.gitignore` & `tcare_sbvalidator-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.8/LICENSE.txt` & `tcare_sbvalidator-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tcare_sbvalidator-0.0.8/pyproject.toml` & `tcare_sbvalidator-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcare_sbvalidator"
-version = "0.0.8"
-dependencies = [ "pydantic", "azure-identity", "azure-servicebus"]
+version = "0.0.9"
+dependencies = [ "pydantic", "azure-identity", "azure-servicebus", "aiohttp"]
 authors = [
   { name="TCARE", email="elijah.kennedy@tcare.ai" },
 ]
 description = "Validate that servicebus messages are in the correct format"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcare_sbvalidator-0.0.8/PKG-INFO` & `tcare_sbvalidator-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tcare_sbvalidator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Validate that servicebus messages are in the correct format
 Project-URL: Homepage, https://github.com/TCARE1/tcare_sbvalidator
 Project-URL: Bug Tracker, https://github.com/TCARE1/tcare_sbvalidator/issues
 Author-email: TCARE <elijah.kennedy@tcare.ai>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: aiohttp
 Requires-Dist: azure-identity
 Requires-Dist: azure-servicebus
 Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 # Tcare Servicebus Validotor (tcare-sbv)
```

