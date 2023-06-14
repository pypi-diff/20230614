# Comparing `tmp/mock_data_generator-1.2.8.tar.gz` & `tmp/mock_data_generator-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_data_generator-1.2.8.tar", max compression
+gzip compressed data, was "mock_data_generator-1.2.9.tar", max compression
```

## Comparing `mock_data_generator-1.2.8.tar` & `mock_data_generator-1.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.8/LICENSE
--rw-r--r--   0        0        0     3021 2023-06-07 11:12:55.484556 mock_data_generator-1.2.8/README.md
--rw-r--r--   0        0        0     1451 2023-06-06 05:48:30.284293 mock_data_generator-1.2.8/mock_data_generator/driver.py
--rw-r--r--   0        0        0     1030 2023-06-07 06:55:46.532920 mock_data_generator-1.2.8/mock_data_generator/generator/generate.py
--rw-r--r--   0        0        0     2097 2023-06-07 06:55:46.545446 mock_data_generator-1.2.8/mock_data_generator/generator/mappings.py
--rw-r--r--   0        0        0     2603 2023-06-07 06:55:46.579568 mock_data_generator-1.2.8/mock_data_generator/generator/misc.py
--rw-r--r--   0        0        0      747 2023-06-07 06:55:46.527612 mock_data_generator-1.2.8/mock_data_generator/generator/output.py
--rw-r--r--   0        0        0      415 2023-06-07 06:55:46.533975 mock_data_generator-1.2.8/mock_data_generator/generator/predefined.py
--rw-r--r--   0        0        0       81 2023-06-06 05:48:30.285866 mock_data_generator-1.2.8/mock_data_generator/resources/config.ini
--rw-r--r--   0        0        0     1954 2023-06-07 06:55:45.873670 mock_data_generator-1.2.8/mock_data_generator/resources/schema.json
--rw-r--r--   0        0        0     1085 2023-06-06 05:48:30.287087 mock_data_generator-1.2.8/mock_data_generator/schema_handler/schema_validator.py
--rw-r--r--   0        0        0      626 2023-06-06 05:48:30.287556 mock_data_generator-1.2.8/mock_data_generator/tests/fileutils_test.py
--rw-r--r--   0        0        0      735 2023-06-06 05:48:30.287921 mock_data_generator-1.2.8/mock_data_generator/tests/schema_validator_test.py
--rw-r--r--   0        0        0      133 2023-06-06 05:48:30.288539 mock_data_generator-1.2.8/mock_data_generator/tests/test.json
--rw-r--r--   0        0        0      846 2023-06-07 06:55:46.544663 mock_data_generator-1.2.8/mock_data_generator/utils/constants.py
--rw-r--r--   0        0        0     2088 2023-06-06 05:48:30.289966 mock_data_generator-1.2.8/mock_data_generator/utils/fileutils.py
--rw-r--r--   0        0        0      947 2023-06-07 11:15:45.168252 mock_data_generator-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 mock_data_generator-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 06:28:18.920052 mock_data_generator-1.2.9/LICENSE
+-rw-r--r--   0        0        0     3087 2023-06-14 04:03:09.863503 mock_data_generator-1.2.9/README.md
+-rw-r--r--   0        0        0     1006 2023-06-14 03:44:01.701116 mock_data_generator-1.2.9/mock_data_generator/driver.py
+-rw-r--r--   0        0        0     1030 2023-06-14 03:43:22.625357 mock_data_generator-1.2.9/mock_data_generator/generator/generate.py
+-rw-r--r--   0        0        0     2097 2023-06-07 06:55:46.545446 mock_data_generator-1.2.9/mock_data_generator/generator/mappings.py
+-rw-r--r--   0        0        0     2603 2023-06-07 06:55:46.579568 mock_data_generator-1.2.9/mock_data_generator/generator/misc.py
+-rw-r--r--   0        0        0      747 2023-06-07 06:55:46.527612 mock_data_generator-1.2.9/mock_data_generator/generator/output.py
+-rw-r--r--   0        0        0      415 2023-06-07 06:55:46.533975 mock_data_generator-1.2.9/mock_data_generator/generator/predefined.py
+-rw-r--r--   0        0        0       81 2023-06-06 05:48:30.285866 mock_data_generator-1.2.9/mock_data_generator/resources/config.ini
+-rw-r--r--   0        0        0     1980 2023-06-14 03:59:33.440925 mock_data_generator-1.2.9/mock_data_generator/resources/schema.json
+-rw-r--r--   0        0        0     1566 2023-06-14 04:01:16.329365 mock_data_generator-1.2.9/mock_data_generator/schema_handler/schema_validator.py
+-rw-r--r--   0        0        0      626 2023-06-06 05:48:30.287556 mock_data_generator-1.2.9/mock_data_generator/tests/fileutils_test.py
+-rw-r--r--   0        0        0      735 2023-06-06 05:48:30.287921 mock_data_generator-1.2.9/mock_data_generator/tests/schema_validator_test.py
+-rw-r--r--   0        0        0      133 2023-06-06 05:48:30.288539 mock_data_generator-1.2.9/mock_data_generator/tests/test.json
+-rw-r--r--   0        0        0      846 2023-06-07 06:55:46.544663 mock_data_generator-1.2.9/mock_data_generator/utils/constants.py
+-rw-r--r--   0        0        0     1988 2023-06-14 04:01:16.338298 mock_data_generator-1.2.9/mock_data_generator/utils/fileutils.py
+-rw-r--r--   0        0        0      948 2023-06-14 04:07:56.423952 mock_data_generator-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3879 1970-01-01 00:00:00.000000 mock_data_generator-1.2.9/PKG-INFO
```

### Comparing `mock_data_generator-1.2.8/LICENSE` & `mock_data_generator-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.8/README.md` & `mock_data_generator-1.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,38 @@
 To solve this, I’ve built a utility to generate the mock data based on the supplied json schema.
 This utility is using Python Faker module to randomly generate the test data.
 Step by step guide on [medium](https://medium.com/@rahulsmtauti/mock-data-generation-for-data-projects-3999865cb82c).
 
 ## How to use
 Follow below steps to run the utility. I am open to your suggestions, please add comments or mail me your suggestions.
 
+**Note: Data Types are case insensitive**
 ### Inputs
 It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP","ADDRESS","CITY","COUNTRY","COUNTRY_CODE","POSTCODE","LICENSE_PLATE","SWIFT","COMPANY","COMPANY_SUFFIX","CREDIT_CARD","CREDIT_CARD_PROVIDER","CREDIT_CARD_NUMBER","CURRENCY","DAY_NUM","DAY_NAME","MONTH_NUM","MONTH_NAME","YEAR","COORDINATE","LATITUDE","LONGITUDE","EMAIL","HOSTNAME","IPV4","IPV6","URI","URL","JOB","TEXT","PASSWORD","SHA1","SHA256","UUID","PASSPORT_NUMBER","NAME","LANGUAGE_NAME","LAST_NAME","FIRST_NAME","PHONE_NUMBER","SSN"`
 #### Supported Input Parameters
 
 - --input_json_schema_path: Provide absolute path of the json schema file/folder. It accepts folders(that contains valid json schema files) or absolute path of a json schema file.
 
 > Json schema file format.
 ```json
 {
   "type": "<object/record,etc>",
+  "number_of_rows": "<positive number>",
   "properties": {
     "<column_name>": { "type": "<data_type>" },
     "<column_name>": { "type": "<data_type>" }
   }
 }
 
 ```
 > The sample json schema file would look like below.
 ```json
 {
   "type": "object",
+  "number_of_rows": "<positive number>",
   "properties": {
     "price": { "type": "number" },
     "name": { "type": "name" },
     "location": { "type": "COORDINATE" },
     "flt": { "type": "float" },
     "email_id": { "type": "EMAIL" },
     "dt": { "type": "date" },
@@ -44,15 +47,14 @@
 ```
 The generator will skip the current json schema file if an error occurred. Mock data would get generated for rest of the valid schema files.
 
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
 - --output_path: Absolute path to store the generated mock dataset. If an output path does not exists, it will create it and store the data inside the directory into data.<output file format> file.
 
-- --number_of_rows: Number of output rows to be generated
 
 ### Pre-requisites
 1. Python ^3.10
 
 
 ### Steps to execute the utility
 1. pip install mock-data-generator
```

### Comparing `mock_data_generator-1.2.8/mock_data_generator/driver.py` & `mock_data_generator-1.2.9/mock_data_generator/driver.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,24 +7,14 @@
     if value.upper() not in FILE_FORMATS:
         raise argparse.ArgumentTypeError(
             f"Unsupported output file format {value} detected. Supported file formats are {FILE_FORMATS}"
         )
     return value
 
 
-def validate_num_rows(value):
-    num_rows = int(value)
-    if num_rows <= 0:
-        raise argparse.ArgumentTypeError(
-            "%s is an invalid number of rows. The value for number of rows should be positive integer"
-            % value
-        )
-    return num_rows
-
-
 def run():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--input_json_schema_path",
         help="Input absolute path of the schema json, schema file or schema folder",
         required=True,
     )
@@ -33,19 +23,13 @@
         type=validate_file_format,
         help="Expected output file format(csv,json,xml,excel,parquet)",
         required=True,
     )
     parser.add_argument(
         "--output_path", help="Output path for mock dataset.", required=True
     )
-    parser.add_argument(
-        "--number_of_rows",
-        type=validate_num_rows,
-        help="Number of mock records to be generated.",
-        required=True,
-    )
     args = parser.parse_args()
     proceed(args=args)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `mock_data_generator-1.2.8/mock_data_generator/generator/generate.py` & `mock_data_generator-1.2.9/mock_data_generator/generator/generate.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.8/mock_data_generator/generator/mappings.py` & `mock_data_generator-1.2.9/mock_data_generator/generator/mappings.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.8/mock_data_generator/generator/misc.py` & `mock_data_generator-1.2.9/mock_data_generator/generator/misc.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.8/mock_data_generator/generator/output.py` & `mock_data_generator-1.2.9/mock_data_generator/generator/output.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.8/mock_data_generator/resources/schema.json` & `mock_data_generator-1.2.9/mock_data_generator/resources/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'number_of_rows'": '5'}*

```diff
@@ -1,8 +1,9 @@
 {
+    "number_of_rows": 5,
     "properties": {
         "a": {
             "type": "integer"
         },
         "add": {
             "type": "ADDRESS"
         },
```

### Comparing `mock_data_generator-1.2.8/mock_data_generator/schema_handler/schema_validator.py` & `mock_data_generator-1.2.9/mock_data_generator/schema_handler/schema_validator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 import json
 import logging
 
 from mock_data_generator.utils.constants import DATA_TYPES
 
 
-class DataTypeError(Exception):
+class ValidationError(Exception):
     def __init__(self, value):
         self.value = value
 
     def __str__(self):
         return repr(self.value)
 
 
 def is_valid_json_schema_file(json_schema: str, file_name: str):
     try:
         json_object = json.loads(json_schema)
         schema_dict = json_object["properties"]
+        number_of_rows = json_object["number_of_rows"]
+
+        if number_of_rows <= 0:
+            logging.error(
+                f"Positive value expected for number_of_rows in the {file_name}"
+            )
+            raise (ValidationError(number_of_rows))
+
         for column_name in schema_dict:
             type_dict = schema_dict[column_name]
             data_type = type_dict["type"].upper()
             if data_type not in DATA_TYPES:
-                raise (DataTypeError(data_type))
+                logging.error(f"Skipping file {file_name}")
+                logging.error(
+                    f"Invalid data type {ex.value} detected in json. Supported data type {DATA_TYPES}"
+                )
+                raise (ValidationError(data_type))
 
     except ValueError as ex:
         logging.error(f"Skipping invalid schema file {file_name}")
         logging.error(f"Invalid json schema file({file_name}) provided: {ex}")
         return False
 
-    except DataTypeError as ex:
-        logging.error(f"Skipping file {file_name}")
+    except ValidationError as ex:
+        return False
+
+    except KeyError as kr:
         logging.error(
-            f"Invalid data type {ex.value} detected in json. Supported data type {DATA_TYPES}"
+            f"Skipping file {file_name}. Mandatory key {kr} not found in the json file provided."
         )
         return False
 
     return True
```

### Comparing `mock_data_generator-1.2.8/mock_data_generator/tests/fileutils_test.py` & `mock_data_generator-1.2.9/mock_data_generator/tests/fileutils_test.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.8/mock_data_generator/tests/schema_validator_test.py` & `mock_data_generator-1.2.9/mock_data_generator/tests/schema_validator_test.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.8/mock_data_generator/utils/constants.py` & `mock_data_generator-1.2.9/mock_data_generator/utils/constants.py`

 * *Files identical despite different names*

### Comparing `mock_data_generator-1.2.8/mock_data_generator/utils/fileutils.py` & `mock_data_generator-1.2.9/mock_data_generator/utils/fileutils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
-from mock_data_generator.schema_handler.schema_validator import is_valid_json_schema_file
+from mock_data_generator.schema_handler.schema_validator import (
+    is_valid_json_schema_file,
+)
 from mock_data_generator.generator.generate import runner
 from argparse import Namespace
 import logging
 import json
 
 
 def read_json_file_as_string(file_path: str):
@@ -12,26 +14,24 @@
 
 
 def make_path_if_not_exists(file_path: str):
     if not os.path.exists(file_path):
         os.makedirs(file_path)
 
 
-def mk_run_call(
-    schema_file_path: str, num_of_rows: str, output_path: str, output_file_format: str
-):
+def mk_run_call(schema_file_path: str, output_path: str, output_file_format: str):
     logging.info(f"Generating data for {schema_file_path}")
     json_schema_string = read_json_file_as_string(schema_file_path)
     if is_valid_json_schema_file(
         json_schema=json_schema_string, file_name=schema_file_path
     ):
         json_schema = json_str_to_json_object(json_schema=json_schema_string)
         runner(
             json_schema=json_schema,
-            num_of_rows=int(num_of_rows),
+            num_of_rows=json_schema["number_of_rows"],
             output_path=output_path,
             file_format=output_file_format,
         )
 
 
 def proceed(args: Namespace):
     json_schema_path = args.input_json_schema_path
@@ -39,23 +39,21 @@
         for each_file in os.listdir(json_schema_path):
             if each_file.endswith(".json"):
                 out_path = f'{args.output_path}/{each_file.replace(".json","")}'
                 make_path_if_not_exists(file_path=out_path)
                 file_path = f"{json_schema_path}/{each_file}"
                 mk_run_call(
                     schema_file_path=file_path,
-                    num_of_rows=args.number_of_rows,
                     output_path=out_path,
                     output_file_format=args.output_file_format,
                 )
     else:
         make_path_if_not_exists(args.output_path)
         mk_run_call(
             schema_file_path=json_schema_path,
-            num_of_rows=args.number_of_rows,
             output_path=args.output_path,
             output_file_format=args.output_file_format,
         )
 
 
 def json_str_to_json_object(json_schema: str):
     return json.loads(json_schema)
```

### Comparing `mock_data_generator-1.2.8/pyproject.toml` & `mock_data_generator-1.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mock_data_generator"
-version = "1.2.8"
-description = "Generate mock data using json schema supplied."
+version = "1.2.9"
+description = "Generate mock data using json schema supplied. "
 authors = ["Rahul Auti <rahulsmtauti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 generate = "mock_data_generator.driver:run"
 
@@ -32,13 +32,13 @@
 ]
 
 [build-system]
 requires = ["poetry>=1.3.2"]
 build-backend = "poetry.masonry.api"
 
 [tool.bumpver]
-current_version = "1.2.8"
+current_version = "1.2.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `mock_data_generator-1.2.8/PKG-INFO` & `mock_data_generator-1.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mock-data-generator
-Version: 1.2.8
-Summary: Generate mock data using json schema supplied.
+Version: 1.2.9
+Summary: Generate mock data using json schema supplied. 
 License: MIT
 Author: Rahul Auti
 Author-email: rahulsmtauti@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -27,35 +27,38 @@
 To solve this, I’ve built a utility to generate the mock data based on the supplied json schema.
 This utility is using Python Faker module to randomly generate the test data.
 Step by step guide on [medium](https://medium.com/@rahulsmtauti/mock-data-generation-for-data-projects-3999865cb82c).
 
 ## How to use
 Follow below steps to run the utility. I am open to your suggestions, please add comments or mail me your suggestions.
 
+**Note: Data Types are case insensitive**
 ### Inputs
 It accept valid json schema files only with supported data types: `"STRING","INT","INTEGER","NUMBER","FLOAT","DATE","BOOLEAN","BOOL","TIMESTAMP","ADDRESS","CITY","COUNTRY","COUNTRY_CODE","POSTCODE","LICENSE_PLATE","SWIFT","COMPANY","COMPANY_SUFFIX","CREDIT_CARD","CREDIT_CARD_PROVIDER","CREDIT_CARD_NUMBER","CURRENCY","DAY_NUM","DAY_NAME","MONTH_NUM","MONTH_NAME","YEAR","COORDINATE","LATITUDE","LONGITUDE","EMAIL","HOSTNAME","IPV4","IPV6","URI","URL","JOB","TEXT","PASSWORD","SHA1","SHA256","UUID","PASSPORT_NUMBER","NAME","LANGUAGE_NAME","LAST_NAME","FIRST_NAME","PHONE_NUMBER","SSN"`
 #### Supported Input Parameters
 
 - --input_json_schema_path: Provide absolute path of the json schema file/folder. It accepts folders(that contains valid json schema files) or absolute path of a json schema file.
 
 > Json schema file format.
 ```json
 {
   "type": "<object/record,etc>",
+  "number_of_rows": "<positive number>",
   "properties": {
     "<column_name>": { "type": "<data_type>" },
     "<column_name>": { "type": "<data_type>" }
   }
 }
 
 ```
 > The sample json schema file would look like below.
 ```json
 {
   "type": "object",
+  "number_of_rows": "<positive number>",
   "properties": {
     "price": { "type": "number" },
     "name": { "type": "name" },
     "location": { "type": "COORDINATE" },
     "flt": { "type": "float" },
     "email_id": { "type": "EMAIL" },
     "dt": { "type": "date" },
@@ -66,15 +69,14 @@
 ```
 The generator will skip the current json schema file if an error occurred. Mock data would get generated for rest of the valid schema files.
 
 - --output_file_format: The output file format should be one of the `"CSV","JSON","XML","EXCEL","PARQUET","ORC"`
 
 - --output_path: Absolute path to store the generated mock dataset. If an output path does not exists, it will create it and store the data inside the directory into data.<output file format> file.
 
-- --number_of_rows: Number of output rows to be generated
 
 ### Pre-requisites
 1. Python ^3.10
 
 
 ### Steps to execute the utility
 1. pip install mock-data-generator
```

