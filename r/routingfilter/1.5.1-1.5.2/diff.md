# Comparing `tmp/routingfilter-1.5.1.tar.gz` & `tmp/routingfilter-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingfilter-1.5.1.tar", last modified: Tue Jun 13 14:18:42 2023, max compression
+gzip compressed data, was "routingfilter-1.5.2.tar", last modified: Tue Jun 13 14:25:52 2023, max compression
```

## Comparing `routingfilter-1.5.1.tar` & `routingfilter-1.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:18:42.868234 routingfilter-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-13 14:18:25.000000 routingfilter-1.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:18:25.000000 routingfilter-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-13 14:18:42.868234 routingfilter-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-13 14:18:25.000000 routingfilter-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 14:18:25.000000 routingfilter-1.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:18:42.864234 routingfilter-1.5.1/routingfilter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/configfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/dictquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    40228 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/routing_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-06-13 14:18:25.000000 routingfilter-1.5.1/routingfilter/routing_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:18:42.868234 routingfilter-1.5.1/routingfilter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 14:18:42.000000 routingfilter-1.5.1/routingfilter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:18:42.868234 routingfilter-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 14:18:25.000000 routingfilter-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:25:52.981181 routingfilter-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-13 14:25:41.000000 routingfilter-1.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:25:41.000000 routingfilter-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-13 14:25:52.981181 routingfilter-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-13 14:25:41.000000 routingfilter-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 14:25:41.000000 routingfilter-1.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:25:52.981181 routingfilter-1.5.2/routingfilter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:25:41.000000 routingfilter-1.5.2/routingfilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-06-13 14:25:41.000000 routingfilter-1.5.2/routingfilter/configfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-13 14:25:41.000000 routingfilter-1.5.2/routingfilter/dictquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-06-13 14:25:41.000000 routingfilter-1.5.2/routingfilter/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40397 2023-06-13 14:25:41.000000 routingfilter-1.5.2/routingfilter/routing_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-06-13 14:25:41.000000 routingfilter-1.5.2/routingfilter/routing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:25:52.981181 routingfilter-1.5.2/routingfilter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-13 14:25:52.000000 routingfilter-1.5.2/routingfilter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 14:25:52.000000 routingfilter-1.5.2/routingfilter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:25:52.000000 routingfilter-1.5.2/routingfilter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 14:25:52.000000 routingfilter-1.5.2/routingfilter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 14:25:52.000000 routingfilter-1.5.2/routingfilter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:25:52.981181 routingfilter-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 14:25:41.000000 routingfilter-1.5.2/setup.py
```

### Comparing `routingfilter-1.5.1/LICENSE.txt` & `routingfilter-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingfilter-1.5.1/PKG-INFO` & `routingfilter-1.5.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.5.1
+Version: 1.5.2
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -31,9 +31,12 @@
 ### Release steps
 * (If needed) Update the requirements in `requirements.txt` and `setup.py`
 * Add a new entry in `CHANGELOG.md` with the new version number
 * Update the version number in `setup.py`
 * Commit and merge the changes into `master` branch
 * Publish a new release with the version number as a tag: the CI will automatically publish the new version un PyPI
 
+### Benchmark tests
+In order to launch the benchmark tests, run ```python routing_benchmark.py```
+
 ### License
 This project is licensed under the **GNU LGPLv3** license.
```

### Comparing `routingfilter-1.5.1/routingfilter/configfilter.py` & `routingfilter-1.5.2/routingfilter/configfilter.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.5.1/routingfilter/dictquery.py` & `routingfilter-1.5.2/routingfilter/dictquery.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.5.1/routingfilter/routing.py` & `routingfilter-1.5.2/routingfilter/routing.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.5.1/routingfilter/routing_benchmark.py` & `routingfilter-1.5.2/routingfilter/routing_benchmark.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     with open(os.path.join('test_data', name + '.json')) as file:
         data = json.load(file)
     return data
 
 MAX_RULE = 1000
 MAX_EVENT = 100
 MAX_LIST_VALUES = 100
+MAX_LIST_VALUES_EVENT = 10
 
 class RoutingBenchMark():
     """Class to test the routing performance in order to monitor the trend of the execution time after new features or changes"""       
     
     def test1_EQUALS_no_key_match(self):
         """Performance test, for the EQUALS routing filter type, with:
             - 100 same rules (type: EQUALS)
@@ -47,15 +48,15 @@
         my_dict = load_test_data("benchmark_rule_equals_dict")
         # Create 100 EQUALS same rules
         rule = load_test_data("benchmark_rule_equals")
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
         # Adding the field 'wheel_model' but with a value different from 'Superlight'
-        benchmark_event_1.update({"wheel_model": "test"})
+        benchmark_event_1.update({"wheel_model": "no_match"})
         routing.load_from_dicts([rule])
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test2_EQUALS_key_exists.__name__}: {(end_time - start_time).total_seconds()}")
@@ -72,24 +73,24 @@
         for i in range(MAX_LIST_VALUES):
             my_dict["filters"][0]["value"].append("test-" + str(i))
         rule = load_test_data("benchmark_rule_equals")
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
-        benchmark_event_1.update({"wheel_model": "test"})
+        benchmark_event_1.update({"wheel_model": "no_match"})
         routing.load_from_dicts([rule])
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test3_EQUALS_list_values.__name__}: {(end_time - start_time).total_seconds()}")
 
-    def test4_EQUALS_list_values_message(self):
+    def test4_EQUALS_values_message(self):
         """Performance test, for the EQUALS routing filter type, with:
             - 100 values in the "wheel_model" of the rule and of the message, but none of them triggers a match (no 'Superlight')
         """
         routing = Routing()
         my_dict = load_test_data("benchmark_rule_equals_dict")
         # Create a list of 100 values in the "value" field of the rule
         for i in range(MAX_LIST_VALUES):
@@ -98,22 +99,22 @@
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         routing.load_from_dicts([rule])
         # Create a list of values in the message for "wheel_model"
         benchmark_event_1 = load_test_data("benchmark_event_1")
         benchmark_event_1.update({"wheel_model": []})
-        for i in range(MAX_LIST_VALUES):
-            benchmark_event_1["wheel_model"].append("test-" + str(i))
+        for i in range(MAX_LIST_VALUES_EVENT):
+            benchmark_event_1["wheel_model"].append("no_match-" + str(MAX_LIST_VALUES+i))
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
-        print(f"{self.test4_EQUALS_list_values_message.__name__}: {(end_time - start_time).total_seconds()}")
+        print(f"{self.test4_EQUALS_values_message.__name__}: {(end_time - start_time).total_seconds()}")
 
     def test1_STARTSWITH_no_key_match(self):
         """Performance test, for the STARTSWITH routing filter type, with:
             - 100 same rules (type: STARTSWITH)
             - 100 messages with 50 fields different from 'wheel_model'
         """
         routing = Routing()
@@ -140,15 +141,15 @@
         my_dict = load_test_data("benchmark_rule_startswith_dict")
         # Create 100 EQUALS same rules
         rule = load_test_data("benchmark_rule_startswith")
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
         # Adding the field 'wheel_model' but with a value different from 'Superlight'
-        benchmark_event_1.update({"wheel_model": "test"})
+        benchmark_event_1.update({"wheel_model": "no_match"})
         routing.load_from_dicts([rule])
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test2_STARTSWITH_key_exists.__name__}: {(end_time - start_time).total_seconds()}")
@@ -165,24 +166,24 @@
         for i in range(MAX_LIST_VALUES):
             my_dict["filters"][0]["value"].append("test-" + str(i))
         rule = load_test_data("benchmark_rule_startswith")
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
-        benchmark_event_1.update({"wheel_model": "test"})
+        benchmark_event_1.update({"wheel_model": "no_match"})
         routing.load_from_dicts([rule])
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test3_STARTSWITH_list_values.__name__}: {(end_time - start_time).total_seconds()}")
 
-    def test4_STARTSWITH_list_values_exists(self):
+    def test4_STARTSWITH_values_message(self):
         """Performance test, for the EQUALS routing filter type, with:
             - 100 values in the "wheel_model" of the rule and of the message, but none of them triggers a match (no 'Superlight')
         """
         routing = Routing()
         my_dict = load_test_data("benchmark_rule_startswith_dict")
         # Create a list of 100 values in the "value" field of the rule
         for i in range(MAX_LIST_VALUES):
@@ -191,22 +192,22 @@
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         routing.load_from_dicts([rule])
         # Create a list of values in the message for "wheel_model"
         benchmark_event_1 = load_test_data("benchmark_event_1")
         benchmark_event_1.update({"wheel_model": []})
-        for i in range(MAX_LIST_VALUES):
-            benchmark_event_1["wheel_model"].append("test-" + str(i))
+        for i in range(MAX_LIST_VALUES_EVENT):
+            benchmark_event_1["wheel_model"].append("no_match-" + str(i))
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
-        print(f"{self.test4_STARTSWITH_list_values_exists.__name__}: {(end_time - start_time).total_seconds()}")
+        print(f"{self.test4_STARTSWITH_values_message.__name__}: {(end_time - start_time).total_seconds()}")
 
     def test1_ENDSWITH_no_key_match(self):
         """Performance test, for the ENDSWITH routing filter type, with:
             - 100 same rules (type: ENDSWITH)
             - 100 messages with 50 fields different from 'wheel_model'
         """
         routing = Routing()
@@ -233,15 +234,15 @@
         my_dict = load_test_data("benchmark_rule_endswith_dict")
         # Create 100 EQUALS same rules
         rule = load_test_data("benchmark_rule_endswith")
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
         # Adding the field 'wheel_model' but with a value different from 'Superlight'
-        benchmark_event_1.update({"wheel_model": "test"})
+        benchmark_event_1.update({"wheel_model": "no_match"})
         routing.load_from_dicts([rule])
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test2_ENDSWITH_key_exists.__name__}: {(end_time - start_time).total_seconds()}")
@@ -258,24 +259,24 @@
         for i in range(MAX_LIST_VALUES):
             my_dict["filters"][0]["value"].append("test-" + str(i))
         rule = load_test_data("benchmark_rule_endswith")
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
-        benchmark_event_1.update({"wheel_model": "test"})
+        benchmark_event_1.update({"wheel_model": "no_match"})
         routing.load_from_dicts([rule])
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test3_ENDSWITH_list_values.__name__}: {(end_time - start_time).total_seconds()}")
 
-    def test4_ENDSWITH_list_values_exists(self):
+    def test4_ENDSWITH_values_message(self):
         """Performance test, for the ENDSWITH routing filter type, with:
             - 100 values in the "wheel_model" of the rule and of the message, but none of them triggers a match (no 'Superlight')
         """
         routing = Routing()
         my_dict = load_test_data("benchmark_rule_endswith_dict")
         # Create a list of 100 values in the "value" field of the rule
         for i in range(MAX_LIST_VALUES):
@@ -284,22 +285,22 @@
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         routing.load_from_dicts([rule])
         # Create a list of values in the message for "wheel_model"
         benchmark_event_1 = load_test_data("benchmark_event_1")
         benchmark_event_1.update({"wheel_model": []})
-        for i in range(MAX_LIST_VALUES):
-            benchmark_event_1["wheel_model"].append("test-" + str(i))
+        for i in range(MAX_LIST_VALUES_EVENT):
+            benchmark_event_1["wheel_model"].append("no_match-" + str(i))
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
-        print(f"{self.test4_ENDSWITH_list_values_exists.__name__}: {(end_time - start_time).total_seconds()}")
+        print(f"{self.test4_ENDSWITH_values_message.__name__}: {(end_time - start_time).total_seconds()}")
 
     def test1_KEYWORD_no_key_match(self):
         """Performance test, for the KEYWORD routing filter type, with:
             - 100 same rules (type: KEYWORD)
             - 100 messages with 50 fields different from 'wheel_model'
         """
         routing = Routing()
@@ -351,24 +352,24 @@
         for i in range(MAX_LIST_VALUES):
             my_dict["filters"][0]["value"].append("test-" + str(i))
         rule = load_test_data("benchmark_rule_keyword")
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
-        benchmark_event_1.update({"wheel_model": "test"})
+        benchmark_event_1.update({"wheel_model": "no_match"})
         routing.load_from_dicts([rule])
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test3_KEYWORD_list_values.__name__}: {(end_time - start_time).total_seconds()}")
 
-    def test4_KEYWORD_list_values_exists(self):
+    def test4_KEYWORD_values_message(self):
         """Performance test, for the KEYWORD routing filter type, with:
             - 100 values in the "wheel_model" of the rule and of the message, but none of them triggers a match (no 'Superlight')
         """
         routing = Routing()
         my_dict = load_test_data("benchmark_rule_keyword_dict")
         # Create a list of 100 values in the "value" field of the rule
         for i in range(MAX_LIST_VALUES):
@@ -377,22 +378,22 @@
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         routing.load_from_dicts([rule])
         # Create a list of values in the message for "wheel_model"
         benchmark_event_1 = load_test_data("benchmark_event_1")
         benchmark_event_1.update({"wheel_model": []})
-        for i in range(MAX_LIST_VALUES):
-            benchmark_event_1["wheel_model"].append("test-" + str(i))
+        for i in range(MAX_LIST_VALUES_EVENT):
+            benchmark_event_1["wheel_model"].append("no_match-" + str(i))
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
-        print(f"{self.test4_KEYWORD_list_values_exists.__name__}: {(end_time - start_time).total_seconds()}")
+        print(f"{self.test4_KEYWORD_values_message.__name__}: {(end_time - start_time).total_seconds()}")
 
     def test1_REGEXP_no_key_match(self):
         """Performance test, for the REGEXP routing filter type, with:
             - 100 same rules (type: REGEXP)
             - 100 messages with 50 fields different from 'wheel_model'
         """
         routing = Routing()
@@ -419,15 +420,15 @@
         my_dict = load_test_data("benchmark_rule_regexp_dict")
         # Create 100 EQUALS same rules
         rule = load_test_data("benchmark_rule_regexp")
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
         # Adding the field 'wheel_model' but with a value different from 'Superlight'
-        benchmark_event_1.update({"wheel_model": "test"})
+        benchmark_event_1.update({"wheel_model": "no_match"})
         routing.load_from_dicts([rule])
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test2_REGEXP_key_exists.__name__}: {(end_time - start_time).total_seconds()}")
@@ -444,24 +445,24 @@
         for i in range(MAX_LIST_VALUES):
             my_dict["filters"][0]["value"].append("test-" + str(i))
         rule = load_test_data("benchmark_rule_regexp")
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
-        benchmark_event_1.update({"wheel_model": "test"})
+        benchmark_event_1.update({"wheel_model": "no_match"})
         routing.load_from_dicts([rule])
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test3_REGEXP_list_values.__name__}: {(end_time - start_time).total_seconds()}")
 
-    def test4_REGEXP_list_values_exists(self):
+    def test4_REGEXP_values_message(self):
         """Performance test, for the REGEXP routing filter type, with:
             - 100 values in the "wheel_model" of the rule and of the message, but none of them triggers a match (no 'Superlight')
         """
         routing = Routing()
         my_dict = load_test_data("benchmark_rule_regexp_dict")
         # Create a list of 100 values in the "value" field of the rule
         for i in range(MAX_LIST_VALUES):
@@ -470,22 +471,22 @@
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         routing.load_from_dicts([rule])
         # Create a list of values in the message for "wheel_model"
         benchmark_event_1 = load_test_data("benchmark_event_1")
         benchmark_event_1.update({"wheel_model": []})
-        for i in range(MAX_LIST_VALUES):
-            benchmark_event_1["wheel_model"].append("test-" + str(i))
+        for i in range(MAX_LIST_VALUES_EVENT):
+            benchmark_event_1["wheel_model"].append("no_match-" + str(i))
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
-        print(f"{self.test4_REGEXP_list_values_exists.__name__}: {(end_time - start_time).total_seconds()}")
+        print(f"{self.test4_REGEXP_values_message.__name__}: {(end_time - start_time).total_seconds()}")
 
     def test1_NETWORK_no_key_match(self):
         """Performance test, for the NETWORK routing filter type, with:
             - 100 same rules (type: NETWORK)
             - 100 messages with 50 fields different from 'wheel_model'
         """
         routing = Routing()
@@ -530,15 +531,16 @@
             - 100 same rules (type: NETWORK)
             - 100 messages with 50 fields (one of them 'wheel_model' but not in the 10.10.10.0/24 network
             - 100 different values in the rules (no matches with the message field)
         """
         routing = Routing()
         my_dict = load_test_data("benchmark_rule_network_dict")
         # Create a list of 100 values in the "value" field of the rule
-        for i in range(MAX_LIST_VALUES):
+        # Different value (no MAX_LIST_VALUES constant) because it takes a while
+        for i in range(20):
             my_dict["filters"][0]["value"].append("10.10.10." + str(i))
         rule = load_test_data("benchmark_rule_network")
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         benchmark_event_1 = load_test_data("benchmark_event_1")
         benchmark_event_1.update({"wheel_model": "192.168.1.0/24"})
@@ -546,39 +548,40 @@
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test3_NETWORK_list_values.__name__}: {(end_time - start_time).total_seconds()}")
 
-    def test4_NETWORK_list_values_exists(self):
+    def test4_NETWORK_values_message(self):
         """Performance test, for the REGEXP routing filter type, with:
             - 100 values in the "wheel_model" of the rule and of the message, but none of them triggers a match (no network 10.10.10.0/24)
         """
         routing = Routing()
         my_dict = load_test_data("benchmark_rule_network_dict")
         # Create a list of 100 values in the "value" field of the rule
-        for i in range(MAX_LIST_VALUES):
+        # Different value (no MAX_LIST_VALUES constant) because it takes a while
+        for i in range(20):
             my_dict["filters"][0]["value"].append("10.10.10." + str(i))
         rule = load_test_data("benchmark_rule_network")
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         routing.load_from_dicts([rule])
         # Create a list of values in the message for "wheel_model"
         benchmark_event_1 = load_test_data("benchmark_event_1")
         benchmark_event_1.update({"wheel_model": []})
-        for i in range(MAX_LIST_VALUES):
+        for i in range(MAX_LIST_VALUES_EVENT):
             benchmark_event_1["wheel_model"].append("192.168.1." + str(i))
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
-        print(f"{self.test4_NETWORK_list_values_exists.__name__}: {(end_time - start_time).total_seconds()}")
+        print(f"{self.test4_NETWORK_values_message.__name__}: {(end_time - start_time).total_seconds()}")
 
     def test1_DOMAIN_no_key_match(self):
         """Performance test, for the DOMAIN routing filter type, with:
             - 100 same rules (type: DOMAIN)
             - 100 messages with 50 fields different from 'wheel_model'
         """
         routing = Routing()
@@ -639,15 +642,15 @@
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test3_DOMAIN_list_values.__name__}: {(end_time - start_time).total_seconds()}")
 
-    def test4_DOMAIN_list_values_exists(self):
+    def test4_DOMAIN_values_message(self):
         """Performance test, for the DOMAIN routing filter type, with:
             - 100 values in the "wheel_model" of the rule and of the message, but none of them triggers a match (no domain google.com)
         """
         routing = Routing()
         my_dict = load_test_data("benchmark_rule_domain_dict")
         # Create a list of 100 values in the "value" field of the rule
         for i in range(MAX_LIST_VALUES):
@@ -656,22 +659,22 @@
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         routing.load_from_dicts([rule])
         # Create a list of values in the message for "wheel_model"
         benchmark_event_1 = load_test_data("benchmark_event_1")
         benchmark_event_1.update({"wheel_model": []})
-        for i in range(MAX_LIST_VALUES):
-            benchmark_event_1["wheel_model"].append("test-" + str(i))
+        for i in range(MAX_LIST_VALUES_EVENT):
+            benchmark_event_1["wheel_model"].append("no_match-" + str(i))
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
-        print(f"{self.test4_DOMAIN_list_values_exists.__name__}: {(end_time - start_time).total_seconds()}")
+        print(f"{self.test4_DOMAIN_values_message.__name__}: {(end_time - start_time).total_seconds()}")
 
     def test1_GREATER_no_key_match(self):
         """Performance test, for the GREATER routing filter type, with:
             - 100 same rules (type: GREATER)
             - 100 messages with 50 fields different from 'wheel_model'
         """
         routing = Routing()
@@ -732,15 +735,15 @@
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
         print(f"{self.test3_GREATER_list_values.__name__}: {(end_time - start_time).total_seconds()}")
 
-    def test4_GREATER_list_values_exists(self):
+    def test4_GREATER_values_message(self):
         """Performance test, for the GREATER routing filter type, with:
             - 100 values in the "wheel_model" of the rule and of the message, but none of them triggers a match (no domain google.com)
         """
         routing = Routing()
         my_dict = load_test_data("benchmark_rule_greater_dict")
         # Create a list of 100 values in the "value" field of the rule
         for i in range(MAX_LIST_VALUES):
@@ -749,54 +752,54 @@
         # Create 100 EQUALS same rules with 100 values
         for i in range(MAX_RULE):
             rule["streams"]["rules"]["mountain_bike"].append(my_dict)
         routing.load_from_dicts([rule])
         # Create a list of values in the message for "wheel_model"
         benchmark_event_1 = load_test_data("benchmark_event_1")
         benchmark_event_1.update({"wheel_model": []})
-        for i in range(MAX_LIST_VALUES):
-            benchmark_event_1["wheel_model"].append( MAX_LIST_VALUES + i)
+        for i in range(MAX_LIST_VALUES_EVENT):
+            benchmark_event_1["wheel_model"].append(0)
         start_time = datetime.now()
         # Sending 100 messages to the routing
         for i in range(MAX_EVENT):
             routing.match(benchmark_event_1)
         end_time = datetime.now()
-        print(f"{self.test4_GREATER_list_values_exists.__name__}: {(end_time - start_time).total_seconds()}")
+        print(f"{self.test4_GREATER_values_message.__name__}: {(end_time - start_time).total_seconds()}")
 
 
 def main():
     routing_benchmark = RoutingBenchMark()
     routing_benchmark.test1_EQUALS_no_key_match()
     routing_benchmark.test2_EQUALS_key_exists()
     routing_benchmark.test3_EQUALS_list_values()
-    routing_benchmark.test4_EQUALS_list_values_message()
+    routing_benchmark.test4_EQUALS_values_message()
     routing_benchmark.test1_STARTSWITH_no_key_match()
     routing_benchmark.test2_STARTSWITH_key_exists()
     routing_benchmark.test3_STARTSWITH_list_values()
-    routing_benchmark.test4_STARTSWITH_list_values_exists()
+    routing_benchmark.test4_STARTSWITH_values_message()
     routing_benchmark.test1_ENDSWITH_no_key_match()
     routing_benchmark.test2_ENDSWITH_key_exists()
     routing_benchmark.test3_ENDSWITH_list_values()
-    routing_benchmark.test4_ENDSWITH_list_values_exists()
+    routing_benchmark.test4_ENDSWITH_values_message()
     routing_benchmark.test1_KEYWORD_no_key_match()
     routing_benchmark.test2_KEYWORD_key_exists()
     routing_benchmark.test3_KEYWORD_list_values()
-    routing_benchmark.test4_KEYWORD_list_values_exists()
+    routing_benchmark.test4_KEYWORD_values_message()
     routing_benchmark.test1_REGEXP_no_key_match()
     routing_benchmark.test2_REGEXP_key_exists()
     routing_benchmark.test3_REGEXP_list_values()
-    routing_benchmark.test4_REGEXP_list_values_exists()
+    routing_benchmark.test4_REGEXP_values_message()
     routing_benchmark.test1_NETWORK_no_key_match()
     routing_benchmark.test2_NETWORK_key_exists()
     routing_benchmark.test3_NETWORK_list_values()
-    routing_benchmark.test4_NETWORK_list_values_exists()
+    routing_benchmark.test4_NETWORK_values_message()
     routing_benchmark.test1_DOMAIN_no_key_match()
     routing_benchmark.test2_DOMAIN_key_exists()
     routing_benchmark.test3_DOMAIN_list_values()
-    routing_benchmark.test4_DOMAIN_list_values_exists()
+    routing_benchmark.test4_DOMAIN_values_message()
     routing_benchmark.test1_GREATER_no_key_match()
     routing_benchmark.test2_GREATER_key_exists()
     routing_benchmark.test3_GREATER_list_values()
-    routing_benchmark.test4_GREATER_list_values_exists()
+    routing_benchmark.test4_GREATER_values_message()
 
 if __name__ == "__main__":
     main()
```

### Comparing `routingfilter-1.5.1/routingfilter/routing_test.py` & `routingfilter-1.5.2/routingfilter/routing_test.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.5.1/routingfilter.egg-info/PKG-INFO` & `routingfilter-1.5.2/routingfilter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.5.1
+Version: 1.5.2
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -31,9 +31,12 @@
 ### Release steps
 * (If needed) Update the requirements in `requirements.txt` and `setup.py`
 * Add a new entry in `CHANGELOG.md` with the new version number
 * Update the version number in `setup.py`
 * Commit and merge the changes into `master` branch
 * Publish a new release with the version number as a tag: the CI will automatically publish the new version un PyPI
 
+### Benchmark tests
+In order to launch the benchmark tests, run ```python routing_benchmark.py```
+
 ### License
 This project is licensed under the **GNU LGPLv3** license.
```

### Comparing `routingfilter-1.5.1/setup.py` & `routingfilter-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='routingfilter',
-    version='1.5.1',
+    version='1.5.2',
     packages=['routingfilter'],
     include_package_data=True,
     install_requires=["IPy~=1.1", "macaddress~=2.0.2"],
     url='https://github.com/certego/RoutingFilter',
     license='GNU LGPLv3',
     author='Certego S.r.l.',
     author_email='support@certego.net',
```

