# Comparing `tmp/craft_ai_sdk-0.9.0.tar.gz` & `tmp/craft_ai_sdk-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft_ai_sdk-0.9.0.tar", max compression
+gzip compressed data, was "craft_ai_sdk-0.9.1.tar", max compression
```

## Comparing `craft_ai_sdk-0.9.0.tar` & `craft_ai_sdk-0.9.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10754 2023-01-26 11:30:44.371774 craft_ai_sdk-0.9.0/LICENSE
--rw-r--r--   0        0        0      865 2023-01-26 11:30:44.375774 craft_ai_sdk-0.9.0/README.md
--rw-r--r--   0        0        0      128 2023-01-26 11:32:14.451902 craft_ai_sdk-0.9.0/craft_ai_sdk/__init__.py
--rw-r--r--   0        0        0      980 2023-01-26 11:30:44.375774 craft_ai_sdk-0.9.0/craft_ai_sdk/exceptions.py
--rw-r--r--   0        0        0     2484 2023-01-26 11:30:44.375774 craft_ai_sdk-0.9.0/craft_ai_sdk/io.py
--rw-r--r--   0        0        0    33145 2023-01-26 11:30:44.375774 craft_ai_sdk-0.9.0/craft_ai_sdk/sdk.py
--rw-r--r--   0        0        0     4853 2023-01-26 11:30:44.375774 craft_ai_sdk-0.9.0/craft_ai_sdk/utils.py
--rw-r--r--   0        0        0   243130 2023-01-26 11:34:19.000000 craft_ai_sdk-0.9.0/documentation.pdf
--rw-r--r--   0        0        0     1308 2023-01-26 11:32:14.451902 craft_ai_sdk-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 craft_ai_sdk-0.9.0/setup.py
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 craft_ai_sdk-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    10754 2023-01-27 16:04:09.364546 craft_ai_sdk-0.9.1/LICENSE
+-rw-r--r--   0        0        0      865 2023-01-27 16:04:09.364546 craft_ai_sdk-0.9.1/README.md
+-rw-r--r--   0        0        0      128 2023-01-27 16:05:24.432699 craft_ai_sdk-0.9.1/craft_ai_sdk/__init__.py
+-rw-r--r--   0        0        0      980 2023-01-27 16:04:09.364546 craft_ai_sdk-0.9.1/craft_ai_sdk/exceptions.py
+-rw-r--r--   0        0        0     2696 2023-01-27 16:04:09.364546 craft_ai_sdk-0.9.1/craft_ai_sdk/io.py
+-rw-r--r--   0        0        0    33141 2023-01-27 16:04:09.364546 craft_ai_sdk-0.9.1/craft_ai_sdk/sdk.py
+-rw-r--r--   0        0        0     4853 2023-01-27 16:04:09.364546 craft_ai_sdk-0.9.1/craft_ai_sdk/utils.py
+-rw-r--r--   0        0        0   243348 2023-01-27 16:07:20.000000 craft_ai_sdk-0.9.1/documentation.pdf
+-rw-r--r--   0        0        0     1327 2023-01-27 16:05:24.432699 craft_ai_sdk-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 craft_ai_sdk-0.9.1/setup.py
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 craft_ai_sdk-0.9.1/PKG-INFO
```

### Comparing `craft_ai_sdk-0.9.0/LICENSE` & `craft_ai_sdk-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `craft_ai_sdk-0.9.0/README.md` & `craft_ai_sdk-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `craft_ai_sdk-0.9.0/craft_ai_sdk/exceptions.py` & `craft_ai_sdk-0.9.1/craft_ai_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `craft_ai_sdk-0.9.0/craft_ai_sdk/io.py` & `craft_ai_sdk-0.9.1/craft_ai_sdk/io.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,20 @@
+from strenum import LowercaseStrEnum
 from craft_ai_sdk.utils import remove_none_values
 
 
+class INPUT_OUTPUT_TYPES(LowercaseStrEnum):
+    STRING = "string"
+    NUMBER = "number"
+    BOOLEAN = "boolean"
+    JSON = "json"
+    ARRAY = "array"
+    FILE = "file"
+
+
 class Input:
     def __init__(
         self, name, data_type, description=None, is_required=None, default_value=None
     ):
         self.name = name
         self.data_type = data_type
         self.description = description
@@ -19,15 +29,15 @@
             "is_required": self.is_required,
             "default_value": self.default_value,
         }
         return remove_none_values(input)
 
 
 class Output:
-    def __init__(self, name, data_type, description):
+    def __init__(self, name, data_type, description=None):
         self.name = name
         self.data_type = data_type
         self.description = description
 
     def to_dict(self):
         output = {
             "name": self.name,
```

### Comparing `craft_ai_sdk-0.9.0/craft_ai_sdk/sdk.py` & `craft_ai_sdk-0.9.1/craft_ai_sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 from the website.
                 Defaults to ``CRAFT_AI_SDK_TOKEN`` environment variable.
             environment_url (:obj:`str`, optional): URL to CraftAI environment.
                 Defaults to ``CRAFT_AI_ENVIRONMENT_URL`` environment variable.
             control_url (:obj:`str`, optional): URL to CraftAI authorization server.
                 You probably don't need to set it.
                 Defaults to ``CRAFT_AI_CONTROL_URL`` environment variable, or
-                https://control-platform.craft.ai.
+                https://mlops-platform.craft.ai.
             verbose_log (:obj:`bool`, optional): If ``True``, information during method
                 execution will be printed.
                 Defaults to ``True`` if the environment variable ``SDK_VERBOSE_LOG`` is
                 set to ``true``; ``False`` if it is set to ``false``; else, defaults to
                 ``True`` in interactive mode; ``False`` otherwise.
 
         Raises:
@@ -90,15 +90,15 @@
         self.base_environment_url = environment_url
         self.base_environment_api_url = f"{environment_url}/api/v1"
 
         # Set base control url
         if control_url is None:
             control_url = os.environ.get("CRAFT_AI_CONTROL_URL")
         if not control_url:
-            control_url = "https://control-platform.craft.ai"
+            control_url = "https://mlops-platform.craft.ai"
         self.base_control_url = control_url
         self.base_control_api_url = f"{control_url}/api/v1"
 
         if verbose_log is None:
             env_verbose_log = os.environ.get("SDK_VERBOSE_LOG", "").lower()
             # Detect interactive mode: https://stackoverflow.com/a/64523765
             verbose_log = (
```

### Comparing `craft_ai_sdk-0.9.0/craft_ai_sdk/utils.py` & `craft_ai_sdk-0.9.1/craft_ai_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `craft_ai_sdk-0.9.0/documentation.pdf` & `craft_ai_sdk-0.9.1/documentation.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 12% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 Craft AI MLOps platform Python SDK
-Release 0.9.0
+Release 0.9.1
 
 Craft AI
 
-Jan 26, 2023
+Jan 27, 2023
 
 Contents
 
 1 craft_ai_sdk package
 1.1 craft_ai_sdk.exceptions module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 1.2 craft_ai_sdk.sdk module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 1.3 craft_ai_sdk.utils module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
@@ -62,15 +62,15 @@
 1.2 craft_ai_sdk.sdk module
 See CraftAiSdk class for more details.
 
 1.3 craft_ai_sdk.utils module
 
 1
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 2
 
 Chapter 1. craft_ai_sdk package
 
 CHAPTER
 
@@ -111,21 +111,21 @@
 
 Inits CraftAiSdk.
 Parameters
 • sdk_token (str, optional) – SDK token. You can retrieve it from the website.
 Defaults to CRAFT_AI_SDK_TOKEN environment variable.
 • environment_url (str, optional) – URL to CraftAI environment. Defaults to
 CRAFT_AI_ENVIRONMENT_URL environment variable.
-• control_url (str, optional) – URL to CraftAI authorization server. You probably don’t need to set it. Defaults to CRAFT_AI_CONTROL_URL environment variable, or https://control-platform.craft.ai.
+• control_url (str, optional) – URL to CraftAI authorization server. You probably don’t need to set it. Defaults to CRAFT_AI_CONTROL_URL environment variable, or https://mlops-platform.craft.ai.
 • verbose_log (bool, optional) – If True, information during method execution
 will be printed. Defaults to True if the environment variable SDK_VERBOSE_LOG
 
 3
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 is set to true; False if it is set to false; else, defaults to True in interactive
 mode; False otherwise.
 Raises
 • ValueError – if the sdk_token or environment_url is not defined and
 • the corresponding environment variable is not set. –
 
@@ -169,15 +169,15 @@
 
 following keys:
 
 4
 
 Chapter 2. CraftAiSdk class
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 • "name" (str): Name of the step.
 • "status" (str): either "Pending" or "Ready".
 • "created_at" (str): The creation date in ISO format.
 • "updated_at" (str): The last updation date in ISO format.
 • "inputs" (dict): The inputs of the step.
 • "outputs" (dict): The outputs of the step.
@@ -219,15 +219,15 @@
 Return type
 list of dict
 
 2.1. Step
 
 5
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 CraftAiSdk.delete_step(step_name)
 
 Delete one step.
 Parameters
 step_name (str) – Name of the step to delete as defined in the config.yaml
 
@@ -274,15 +274,15 @@
 The deleted pipeline and assiocated deleted endpoints. The returned dict
 contains two keys:
 
 6
 
 Chapter 2. CraftAiSdk class
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 • "pipeline" (dict): Deleted pipeline represented as dict (with keys "id"
 and "name").
 • "endpoints" (list): List of deleted endpoints represented as dict (with
 keys "id" and "name").
 Return type
 dict
@@ -344,15 +344,15 @@
 as dict (with keys "execution_id", "status", "created_at, "steps",
 "pipeline_name", "created_by"). In particular the keys:
 
 2.3. Pipeline Execution
 
 7
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 • "steps" is a list of the execution steps represented as dict (with keys
 "name", "status").
 • "pipeline_name" is the executed pipeline name.
 Return type
 dict
 CraftAiSdk.get_pipeline_execution_logs(pipeline_name, execution_id,
@@ -396,15 +396,15 @@
 List of endpoints represented as dict (with keys "id", "name" and
 "pipeline").
 
 8
 
 Chapter 2. CraftAiSdk class
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 Return type
 list of dict
 CraftAiSdk.get_endpoint(endpoint_name)
 
 Get information of an endpoint.
 Parameters
@@ -454,15 +454,15 @@
 • object_path_in_datastore (str) – Location of the object to download
 from the data store.
 
 2.5. Data store
 
 9
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 • filepath_or_buffer (str or file-like object) – String, filepath to save the
 file to ; or a file-like object implementing a write() method, (e.g. via
 builtin open function). The file object must be opened in binary mode,
 not text mode.
 Returns
 content of the file
@@ -510,15 +510,15 @@
 Return type
 list of dict
 
 10
 
 Chapter 2. CraftAiSdk class
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 CraftAiSdk.delete_environment_variable(environment_variable_name)
 
 Delete the specified environment variable
 Parameters
 environment_variable_name (str) – Name of the environment variable to
 
@@ -526,30 +526,30 @@
 Returns
 dict (with keys "name" and "value") of the deleted environment variable
 
 2.6. Environment Variables
 
 11
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 12
 
 Chapter 2. CraftAiSdk class
 
 Python Module Index
 
 c
 craft_ai_sdk.exceptions, 1
 craft_ai_sdk.sdk, 1
 craft_ai_sdk.utils, 1
 
 13
 
-Craft AI MLOps platform Python SDK, Release 0.9.0
+Craft AI MLOps platform Python SDK, Release 0.9.1
 
 14
 
 Python Module Index
 
 Index
```

### Comparing `craft_ai_sdk-0.9.0/pyproject.toml` & `craft_ai_sdk-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "craft-ai-sdk"
-version = "0.9.0"
+version = "0.9.1"
 description = "Craft AI MLOps platform SDK"
 license = "Apache-2.0"
 authors = ["Craft AI <contact@craft.ai>"]
 readme = "README.md"
 homepage = "https://www.craft.ai/"
 packages = [
     { include = "craft_ai_sdk" },
@@ -28,14 +28,15 @@
     ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.27.1"
 PyJWT = "^2.3.0"
 python-dotenv = "^0.20.0"
+StrEnum = "^0.4.9"
 
 [tool.poetry.dev-dependencies]
 ipython = "^8.0.1"
 ipykernel = "^6.9.1"
 black = "^22.1.0"
 flake8 = "^4.0.1"
 pylint = "^2.12.2"
```

### Comparing `craft_ai_sdk-0.9.0/setup.py` & `craft_ai_sdk-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ['craft_ai_sdk']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyJWT>=2.3.0,<3.0.0',
+ 'StrEnum>=0.4.9,<0.5.0',
  'python-dotenv>=0.20.0,<0.21.0',
  'requests>=2.27.1,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['bump-version = scripts.scripts:bump_version',
                      'format = scripts.scripts:format',
                      'lint = scripts.scripts:lint',
@@ -22,15 +23,15 @@
                      'test-base = scripts.scripts:test_base',
                      'test-platform = scripts.scripts:test_platform',
                      'update-testrunner-token = '
                      'scripts.scripts:update_testrunner_token']}
 
 setup_kwargs = {
     'name': 'craft-ai-sdk',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Craft AI MLOps platform SDK',
     'long_description': '# Craft AI Python SDK\n\nThis Python SDK lets you interact with Craft AI MLOps Platform.\n\n## Installation\nThis project relies on **Python 3.8+**. Once a supported version of Python is installed, you can install `craft-ai-sdk` from PyPI with:\n\n```console\npip install craft-ai-sdk\n```\n\n## Basic usage\nYou can configure the SDK by instantiating the `CraftAiSdk` class in this way:\n\n```python\nfrom craft_ai_sdk import CraftAiSdk\n\nCRAFT_AI_SDK_TOKEN =  # your access key obtained from your settings page\nCRAFT_AI_ENVIRONMENT_URL =  # url to your environment\n\nsdk = CraftAiSdk(sdk_token=CRAFT_AI_SDK_TOKEN, environment_url=CRAFT_AI_ENVIRONMENT_URL)\n```\n\nIf using the SDK in interactive mode, some additional feedbacks will be printed. You can force disable or enable those logs by either\n* Setting the `verbose_log` SDK parameter\n* Or setting the `SDK_VERBOSE_LOG` env var\n',
     'author': 'Craft AI',
     'author_email': 'contact@craft.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.craft.ai/',
```

### Comparing `craft_ai_sdk-0.9.0/PKG-INFO` & `craft_ai_sdk-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: craft-ai-sdk
-Version: 0.9.0
+Version: 0.9.1
 Summary: Craft AI MLOps platform SDK
 Home-page: https://www.craft.ai/
 License: Apache-2.0
 Author: Craft AI
 Author-email: contact@craft.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=2.3.0,<3.0.0)
+Requires-Dist: StrEnum (>=0.4.9,<0.5.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Craft AI Python SDK
 
 This Python SDK lets you interact with Craft AI MLOps Platform.
```

