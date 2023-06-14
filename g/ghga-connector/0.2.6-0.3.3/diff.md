# Comparing `tmp/ghga_connector-0.2.6.tar.gz` & `tmp/ghga_connector-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_connector-0.2.6.tar", last modified: Wed Feb  1 18:20:59 2023, max compression
+gzip compressed data, was "ghga_connector-0.3.3.tar", last modified: Wed Jun 14 09:42:43 2023, max compression
```

## Comparing `ghga_connector-0.2.6.tar` & `ghga_connector-0.3.3.tar`

### file list

```diff
@@ -1,55 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.382596 ghga_connector-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-02-01 18:20:59.382596 ghga_connector-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.374596 ghga_connector-0.2.6/ghga_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.378596 ghga_connector-0.2.6/ghga_connector/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/core/api_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/core/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/core/http_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/core/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/core/message_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/ghga_connector/core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.378596 ghga_connector-0.2.6/ghga_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-02-01 18:20:59.000000 ghga_connector-0.2.6/ghga_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-01 18:20:59.000000 ghga_connector-0.2.6/ghga_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 18:20:59.000000 ghga_connector-0.2.6/ghga_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-01 18:20:59.000000 ghga_connector-0.2.6/ghga_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 18:20:59.000000 ghga_connector-0.2.6/ghga_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-01 18:20:59.000000 ghga_connector-0.2.6/ghga_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-01 18:20:59.000000 ghga_connector-0.2.6/ghga_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-02-01 18:20:59.382596 ghga_connector-0.2.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.370596 ghga_connector-0.2.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.382596 ghga_connector-0.2.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/fixtures/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.382596 ghga_connector-0.2.6/tests/fixtures/mock_api/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/fixtures/mock_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/fixtures/mock_api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/fixtures/mock_api/testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/fixtures/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/fixtures/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.382596 ghga_connector-0.2.6/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.382596 ghga_connector-0.2.6/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/integration/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/integration/test_file_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.382596 ghga_connector-0.2.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:20:59.382596 ghga_connector-0.2.6/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/unit/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/unit/test_api_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-02-01 18:20:47.000000 ghga_connector-0.2.6/tests/unit/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.225463 ghga_connector-0.3.3/ghga_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.233463 ghga_connector-0.3.3/ghga_connector/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.233463 ghga_connector-0.3.3/ghga_connector/core/api_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/work_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/batch_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/http_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/message_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.229463 ghga_connector-0.3.3/ghga_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:42:42.000000 ghga_connector-0.3.3/ghga_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.221463 ghga_connector-0.3.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.233463 ghga_connector-0.3.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.233463 ghga_connector-0.3.3/tests/fixtures/mock_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/mock_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/mock_api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/mock_api/testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/test_api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/test_file_operations.py
```

### Comparing `ghga_connector-0.2.6/LICENSE` & `ghga_connector-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/ghga_connector/__init__.py` & `ghga_connector-0.3.3/ghga_connector/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 CLI - Client to perform up- and download operations to and from a local ghga instance
 """
 
-__version__ = "0.2.6"
+__version__ = "0.3.3"
```

### Comparing `ghga_connector-0.2.6/ghga_connector/__main__.py` & `ghga_connector-0.3.3/ghga_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/ghga_connector/config.py` & `ghga_connector-0.3.3/ghga_connector/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,38 +12,40 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Global Config Parameters"""
 
-from ghga_service_chassis_lib.config import config_from_yaml
+from hexkit.config import config_from_yaml
 from pydantic import BaseSettings, Field
 
-from ghga_connector import core
+from ghga_connector.core.constants import DEFAULT_PART_SIZE, MAX_RETRIES, MAX_WAIT_TIME
 
 
 @config_from_yaml(prefix="ghga_connector")
 class Config(BaseSettings):
     "Global Config Parameters"
 
     upload_api: str = Field(
         "https://hd-dev.ghga-dev.de/ucs",
         description="URL to the root of the upload controller API.",
     )
     download_api: str = Field(
         "https://hd-dev.ghga-dev.de/drs3/ga4gh/drs/v1",
         description="URL to the root of the DRS-compatible API used for download.",
     )
-
     max_retries: int = Field(
-        core.MAX_RETRIES, description="Number of times to retry failed API calls."
+        MAX_RETRIES, description="Number of times to retry failed API calls."
     )
     max_wait_time: int = Field(
-        core.MAX_WAIT_TIME,
-        description=(
-            "Maximal time in seconds to wait before quitting without a download."
-        ),
+        MAX_WAIT_TIME,
+        description="Maximal time in seconds to wait before quitting without a download.",
     )
     part_size: int = Field(
-        core.DEFAULT_PART_SIZE, description="The part size to use for download."
+        DEFAULT_PART_SIZE, description="The part size to use for download."
+    )
+    server_pubkey: str = Field(
+        ...,
+        description="Base64 encoded current GHGA public key for Crypt4GH encryption.",
     )
+    wps_api_url: str = Field(..., description="URL to the root of the WPS API.")
```

### Comparing `ghga_connector-0.2.6/ghga_connector/core/__init__.py` & `ghga_connector-0.3.3/ghga_connector/core/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 
 """
 This sub-package contains the main business functionality of this service.
 It should not contain any service API-related code.
 """
 
 from . import exceptions  # noqa: F401
+from .api_calls import WorkPackageAccessor  # noqa: F401
+from .batch_processing import CliIoHandler, FileStager, StagingParameters  # noqa: F401
 from .constants import (  # noqa: F401
     DEFAULT_PART_SIZE,
     MAX_PART_NUMBER,
     MAX_RETRIES,
     MAX_WAIT_TIME,
 )
-from .main import download, upload  # noqa: F401
+from .main import decrypt_file, download, upload  # noqa: F401
 from .message_display import AbstractMessageDisplay, MessageColors  # noqa: F401
 from .session import RequestsSession  # noqa: F401
```

### Comparing `ghga_connector-0.2.6/ghga_connector/core/api_calls.py` & `ghga_connector-0.3.3/tests/fixtures/mock_api/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,423 +11,415 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """
-Contains calls to the GHGA storage API
+Runs a small fastapi mock server for testing purposes.
+All mocks work correclty with file_id == "1".
+The drs3 mock sends back a "wait 1 minute" for file_id == "1m"
+All other file_ids will fail
 """
 
 import base64
-import json
+import os
+from datetime import datetime, timezone
 from enum import Enum
-from pathlib import Path
-from time import sleep
-from typing import Dict, Iterator, Tuple, Union
-
-import crypt4gh.keys
-import requests
-from requests.structures import CaseInsensitiveDict
-
-from ghga_connector.core import exceptions
-from ghga_connector.core.constants import MAX_PART_NUMBER, TIMEOUT
-from ghga_connector.core.http_translation import ResponseExceptionTranslator
-from ghga_connector.core.message_display import AbstractMessageDisplay
-from ghga_connector.core.session import RequestsSession
-
-# Constants for clarity of return values
-NO_DOWNLOAD_URL = None
-NO_FILE_SIZE = None
-NO_RETRY_TIME = None
+from typing import List
+
+try:  # workaround for https://github.com/pydantic/pydantic/issues/5821
+    from typing_extensions import Literal
+except ImportError:
+    from typing import Literal  # type: ignore
+
+
+from fastapi import FastAPI, Header, HTTPException, Request, status
+from fastapi.responses import JSONResponse, Response
+from pydantic import BaseModel
+
+DEFAULT_PART_SIZE = 16 * 1024 * 1024
 
 
 class UploadStatus(str, Enum):
     """
-    Enum for the possible statuses of an upload attempt.
+    Enum for the possible UploadStatus of a specific upload_id
     """
 
     ACCEPTED = "accepted"
     CANCELLED = "cancelled"
     FAILED = "failed"
     PENDING = "pending"
     REJECTED = "rejected"
     UPLOADED = "uploaded"
 
 
-def initiate_multipart_upload(
-    *,
-    api_url: str,
-    file_id: str,
-    pubkey_path: Path,
-) -> Tuple[str, int]:
-    """
-    Perform a RESTful API call to initiate a multipart upload
-    Returns an upload id and a part size
-    """
-
-    # build url and headers
-    url = f"{api_url}/uploads"
-    headers = {"Accept": "application/json", "Content-Type": "application/json"}
-    public_key = base64.b64encode(crypt4gh.keys.get_public_key(pubkey_path)).decode()
-
-    post_data = {"file_id": file_id, "submitter_public_key": public_key}
-    serialized_data = json.dumps(post_data)
-
-    # Make function call to get upload url
-    try:
-        response = RequestsSession.post(
-            url=url, headers=headers, data=serialized_data, timeout=TIMEOUT
-        )
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
-        raise exceptions.RequestFailedError(url=url) from request_error
-
-    status_code = response.status_code
-    if status_code != 200:
-        spec = {
-            400: {
-                "existingActiveUpload": lambda: exceptions.NoUploadPossibleError(
-                    file_id=file_id
-                ),
-                "fileNotRegistered": lambda: exceptions.FileNotRegisteredError(
-                    file_id=file_id
-                ),
-            },
-            403: {
-                "noFileAccess": lambda: exceptions.UserHasNoFileAccessError(
-                    file_id=file_id
-                )
-            },
-        }
-        ResponseExceptionTranslator(spec=spec).handle(response=response)
-        raise exceptions.BadResponseCodeError(url=url, response_code=status_code)
+class StatePatch(BaseModel):
+    """
+    Model containing a state parameter. Needed for the UCS patch: /uploads/... api call
+    """
+
+    status: UploadStatus
+
 
-    response_body = response.json()
+class StatePost(BaseModel):
+    """
+    Model containing a state parameter. Needed for the UCS post: /uploads api call
+    """
 
-    return response_body["upload_id"], int(response_body["part_size"])
+    file_id: str
 
 
-def get_part_upload_url(*, api_url: str, upload_id: str, part_no: int):
+class PresignedPostURL(BaseModel):
     """
-    Get a presigned url to upload a specific part
+    Model containing an url
     """
 
-    # build url and headers
-    url = f"{api_url}/uploads/{upload_id}/parts/{part_no}/signed_urls"
-    headers = {"Accept": "application/json", "Content-Type": "application/json"}
+    url: str
 
-    # Make function call to get upload url
-    try:
-        response = RequestsSession.post(url=url, headers=headers, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
-        raise exceptions.RequestFailedError(url=url) from request_error
 
-    status_code = response.status_code
-    if status_code != 200:
-        spec = {
-            403: {
-                "noFileAccess": lambda: exceptions.UserHasNoUploadAccessError(
-                    upload_id=upload_id
-                )
-            },
-            404: {
-                "noSuchUpload": lambda: exceptions.UploadNotRegisteredError(
-                    upload_id=upload_id
-                )
-            },
-        }
-        ResponseExceptionTranslator(spec=spec).handle(response=response)
-        raise exceptions.BadResponseCodeError(url=url, response_code=status_code)
+class Checksum(BaseModel):
+    """
+    A Checksum as per the DRS OpenApi specs.
+    """
 
-    response_body = response.json()
-    presigned_url = response_body["url"]
+    checksum: str
+    type: Literal["md5", "sha-256"]
 
-    return presigned_url
 
+class AccessURL(BaseModel):
+    """Describes the URL for accessing the actual bytes of the object as per the
+    DRS OpenApi spec."""
+
+    url: str
+
+
+class AccessMethod(BaseModel):
+    """An AccessMethod as per the DRS OpenApi spec."""
+
+    access_url: AccessURL
+    type: Literal["s3"] = "s3"  # currently only s3 is supported
+
+
+class UploadProperties(BaseModel):
+    """The Upload Properties returned by the UCS post /uploads endpoint"""
+
+    upload_id: str
+    file_id: str
+    part_size: int
 
-def get_part_upload_urls(
-    *,
-    api_url: str,
-    upload_id: str,
-    from_part: int = 1,
-    get_url_func=get_part_upload_url,
-) -> Iterator[str]:
-    """
-    For a specific mutli-part upload identified by the `upload_id`, it returns an
-    iterator to iterate through file parts and obtain the corresponding upload urls.
 
-    By default it start with the first part but you may also start from a specific part
-    in the middle of the file using the `from_part` argument. This might be useful to
-    resume an interrupted upload process.
+class FileProperties(BaseModel):
+    """The File Properties returned by the UCS get /files/{file_id} endpoint"""
 
-    Please note: the upload corresponding to the `upload_id` must have already been
-    initiated.
+    file_id: str
+    file_name: str
+    md5_checksum: str
+    size: int
+    grouping_label: str
+    creation_date: datetime
+    update_date: datetime
+    format: str
+    current_upload_id: str
 
-    `get_url_func` only for testing purposes.
+
+class DrsObjectServe(BaseModel):
+    """
+    A model containing a DrsObject as per the DRS OpenApi specs.
+    This is used to serve metadata on a DrsObject (including the access methods) to the
+    user.
     """
 
-    for part_no in range(from_part, MAX_PART_NUMBER + 1):
-        yield get_url_func(api_url=api_url, upload_id=upload_id, part_no=part_no)
+    file_id: str  # the file ID
+    self_uri: str
+    size: int
+    created_time: str
+    updated_time: str
+    checksums: List[Checksum]
+    access_methods: List[AccessMethod]
+
+
+class HttpEnvelopeResponse(JSONResponse):
+    """Return base64 encoded envelope bytes"""
+
+    response_id = "envelope"
+
+    def __init__(self, *, envelope: str, status_code: int = 200):
+        """Construct message and init the response."""
+
+        super().__init__(content=envelope, status_code=status_code)
+
+
+class HttpyException(Exception):
+    """Testing stand in for httpyexpect HttpException without content validation"""
+
+    def __init__(
+        self, *, status_code: int, exception_id: str, description: str, data: dict
+    ):
+        self.status_code = status_code
+        self.exception_id = exception_id
+        self.description = description
+        self.data = data
+        super().__init__(description)
+
 
-    raise exceptions.MaxPartNoExceededError()
+app = FastAPI()
 
 
-def patch_multipart_upload(
-    *, api_url: str, upload_id: str, upload_status: UploadStatus
-) -> None:
+@app.exception_handler(HttpyException)
+async def httpy_exception_handler(request: Request, exc: HttpyException):
+    """Transform HttpException data into a proper response object"""
+    return JSONResponse(
+        status_code=exc.status_code,
+        content={
+            "exception_id": exc.exception_id,
+            "description": exc.description,
+            "data": exc.data,
+        },
+    )
+
+
+@app.get("/ready", summary="readiness_probe")
+async def ready():
     """
-    Set the status of a specific upload attempt.
-    The API accepts "uploaded" or "accepted",
-    if the upload_id is currently set to "pending"
+    Readyness probe.
     """
+    return JSONResponse(None, status_code=status.HTTP_204_NO_CONTENT)
 
-    # build url and headers
-    url = f"{api_url}/uploads/{upload_id}"
-    headers = {"Accept": "*/*", "Content-Type": "application/json"}
-    post_data = {"status": upload_status}
-    serialized_data = json.dumps(post_data)
 
-    try:
-        response = RequestsSession.patch(
-            url=url, headers=headers, data=serialized_data, timeout=TIMEOUT
+@app.get("/objects/{file_id}", summary="drs3_mock")
+async def drs3_objects(file_id: str, authorization=Header()):
+    """
+    Mock for the drs3 /objects/{file_id} call
+    """
+
+    # simulate token authorization error
+    if authorization == "Bearer authfail_normal":
+        raise HTTPException(
+            status_code=403, detail="This is not the token you're looking for."
         )
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
-        raise exceptions.RequestFailedError(url=url) from request_error
 
-    status_code = response.status_code
-    if status_code != 204:
-        spec = {
-            400: {
-                "uploadNotPending": lambda: exceptions.CantChangeUploadStatusError(
-                    upload_id=upload_id, upload_status=upload_status
-                ),
-                "uploadStatusChange": lambda: exceptions.CantChangeUploadStatusError(
-                    upload_id=upload_id, upload_status=upload_status
-                ),
-            },
-            403: {
-                "noFileAccess": lambda: exceptions.UserHasNoUploadAccessError(
-                    upload_id=upload_id
-                )
-            },
-            404: {
-                "noSuchUpload": lambda: exceptions.UploadNotRegisteredError(
-                    upload_id=upload_id
-                )
-            },
-        }
-        ResponseExceptionTranslator(spec=spec).handle(response=response)
-        raise exceptions.BadResponseCodeError(url=url, response_code=status_code)
-
-
-def get_upload_info(
-    *,
-    api_url: str,
-    upload_id: str,
-) -> Dict:
-    """
-    Get details on a specific upload
-    """
-
-    # build url and headers
-    url = f"{api_url}/uploads/{upload_id}"
-    headers = {"Accept": "*/*", "Content-Type": "application/json"}
-
-    try:
-        response = RequestsSession.get(url=url, headers=headers, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
-        raise exceptions.RequestFailedError(url=url) from request_error
-
-    status_code = response.status_code
-    if status_code != 200:
-        spec = {
-            403: {
-                "noFileAccess": lambda: exceptions.UserHasNoUploadAccessError(
-                    upload_id=upload_id
-                )
-            },
-            404: {
-                "noSuchUpload": lambda: exceptions.UploadNotRegisteredError(
-                    upload_id=upload_id
+    # simulate token file_id/object_id mismatch
+    if authorization == "Bearer file_id_mismatch":
+        raise HttpyException(
+            status_code=403,
+            exception_id="wrongFileAuthorizationError",
+            description="Endpoint file ID did not match file ID announced in work order token.",
+            data={},
+        )
+
+    if file_id == "retry":
+        return Response(
+            status_code=status.HTTP_202_ACCEPTED, headers={"Retry-After": "10"}
+        )
+
+    if file_id in ("downloadable", "big-downloadable", "envelope-missing"):
+        return DrsObjectServe(
+            file_id=file_id,
+            self_uri=f"drs://localhost:8080//{file_id}",
+            size=int(os.environ["S3_DOWNLOAD_FIELD_SIZE"]),
+            created_time=datetime.now(timezone.utc).isoformat(),
+            updated_time=datetime.now(timezone.utc).isoformat(),
+            checksums=[Checksum(checksum="1", type="md5")],
+            access_methods=[
+                AccessMethod(
+                    access_url=AccessURL(url=os.environ["S3_DOWNLOAD_URL"]), type="s3"
                 )
-            },
-        }
-        ResponseExceptionTranslator(spec=spec).handle(response=response)
-        raise exceptions.BadResponseCodeError(url=url, response_code=status_code)
+            ],
+        )
 
-    return response.json()
+    raise HTTPException(
+        status_code=404,
+        detail=(f'The DRSObject with the id "{file_id}" does not exist.'),
+    )
 
 
-def get_file_metadata(*, api_url: str, file_id: str) -> Dict:
+@app.get("/objects/{file_id}/envelopes/{public_key}", summary="drs3_envelope_mock")
+async def drs3_objects_envelopes(file_id: str, public_key: str, authorization=Header()):
     """
-    Get all file metadata
+    Mock for the dcs /objects/{file_id}/envelopes/{public_key} call
     """
 
-    # build url and headers
-    url = f"{api_url}/files/{file_id}"
-    headers = {"Accept": "application/json", "Content-Type": "application/json"}
+    if file_id in ("downloadable", "big-downloadable"):
+        response_str = str.encode(os.environ["FAKE_HEADER_ENVELOPE"])
+        envelope = base64.b64encode(response_str).decode("utf-8")
+        return HttpEnvelopeResponse(envelope=envelope)
+
+    raise HttpyException(
+        status_code=404,
+        exception_id="noSuchObject",
+        description=(f'The DRSObject with the id "{file_id}" does not exist.'),
+        data={"file_id": file_id},
+    )
 
-    try:
-        response = RequestsSession.get(url=url, headers=headers, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
-        raise exceptions.RequestFailedError(url=url) from request_error
 
-    status_code = response.status_code
-    if status_code != 200:
-        spec = {
-            403: {
-                "noFileAccess": lambda: exceptions.UserHasNoFileAccessError(
-                    file_id=file_id
-                )
-            },
-            404: {
-                "fileNotRegistered": lambda: exceptions.FileNotRegisteredError(
-                    file_id=file_id
-                )
-            },
-        }
-        ResponseExceptionTranslator(spec=spec).handle(response=response)
-        raise exceptions.BadResponseCodeError(url=url, response_code=status_code)
+@app.get("/files/{file_id}", summary="ulc_get_files_mock", status_code=200)
+async def ulc_get_files(file_id: str):
+    """
+    Mock for the ulc GET /files/{file_id} call.
+    """
+
+    if file_id == "pending":
+        return FileProperties(
+            file_id=file_id,
+            file_name=file_id,
+            md5_checksum="",
+            size=0,
+            grouping_label="inbox",
+            creation_date=datetime.utcnow(),
+            update_date=datetime.utcnow(),
+            format="",
+            current_upload_id="pending",
+        )
 
-    file_metadata = response.json()
+    raise HttpyException(
+        status_code=404,
+        exception_id="fileNotRegistered",
+        description=f'The file with the file_id "{file_id}" does not exist.',
+        data={"file_id": file_id},
+    )
 
-    return file_metadata
 
+@app.get("/uploads/{upload_id}", summary="ulc_get_uploads_mock", status_code=200)
+async def ulc_get_uploads(upload_id: str):
+    """
+    Mock for the ulc GET /uploads/{upload_id} call.
+    """
+    if upload_id == "pending":
+        return UploadProperties(
+            upload_id="pending",
+            file_id="pending",
+            part_size=DEFAULT_PART_SIZE,
+        )
 
-def download_api_call(
-    *, api_url: str, file_id: str
-) -> Union[Tuple[None, None, int], Tuple[str, int, None]]:
+    raise HttpyException(
+        status_code=404,
+        exception_id="noSuchUpload",
+        description=f'The upload with the id "{upload_id}" does not exist.',
+        data={"upload_id": upload_id},
+    )
+
+
+@app.post("/uploads", summary="ulc_post_uploads_mock", status_code=200)
+async def ulc_post_files_uploads(state: StatePost):
     """
-    Perform a RESTful API call to retrieve a presigned download URL.
-    Returns:
-        A tuple of three elements:
-            1. the download url
-            2. the file size (in bytes)
-            3. the retry-time
-        If the download url is not available yet, the first two elements are None and
-        the retry-time is set.
-        Otherwise, only the last element is None while the others are set.
+    Mock for the ulc POST /uploads call.
     """
 
-    # build url and headers
-    url = f"{api_url}/objects/{file_id}"
+    file_id = state.file_id
 
-    headers = CaseInsensitiveDict(
-        {"Accept": "application/json", "Content-Type": "application/json"}
-    )
+    if file_id == "uploadable":
+        return UploadProperties(
+            upload_id="pending",
+            file_id=file_id,
+            part_size=DEFAULT_PART_SIZE,
+        )
+    if file_id == "uploadable-16":
+        return UploadProperties(
+            upload_id="pending",
+            file_id=file_id,
+            part_size=16 * 1024 * 1024,
+        )
 
-    # Make function call to get upload url
-    try:
-        response = RequestsSession.get(url=url, headers=headers, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
-        raise exceptions.RequestFailedError(url=url) from request_error
-
-    status_code = response.status_code
-    if status_code != 200:
-        if status_code != 202:
-            raise exceptions.BadResponseCodeError(url=url, response_code=status_code)
-
-        headers = response.headers
-        if "retry-after" not in headers:
-            raise exceptions.RetryTimeExpectedError(url=url)
-
-        return (NO_DOWNLOAD_URL, NO_FILE_SIZE, int(headers["retry-after"]))
-
-    # look for an access method of type s3 in the response:
-    response_body = response.json()
-    download_url = None
-    access_methods = response_body["access_methods"]
-    for access_method in access_methods:
-        if access_method["type"] == "s3":
-            download_url = access_method["access_url"]["url"]
-            file_size = response_body["size"]
-            break
-
-    if download_url is None:
-        raise exceptions.NoS3AccessMethodError(url=url)
-
-    return download_url, file_size, NO_RETRY_TIME
-
-
-def start_multipart_upload(
-    *, api_url: str, file_id: str, pubkey_path: Path
-) -> Tuple[str, int]:
-    """Try to initiate a multipart upload. If it fails, try to cancel the current upload
-    can and then try to initiate a multipart upload again."""
-
-    try:
-        multipart_upload = initiate_multipart_upload(
-            api_url=api_url,
+    if file_id == "uploadable-8":
+        return UploadProperties(
+            upload_id="pending",
             file_id=file_id,
-            pubkey_path=pubkey_path,
+            part_size=8 * 1024 * 1024,
+        )
+    if file_id == "pending":
+        raise HttpyException(
+            status_code=403,
+            exception_id="noFileAccess",
+            description=f'Can`t start multipart upload for file with file id "{file_id}".',
+            data={"file_id": file_id},
+        )
+
+    raise HttpyException(
+        status_code=400,
+        exception_id="fileNotRegistered",
+        description=f'The file with the file_id "{file_id}" does not exist.',
+        data={"file_id": file_id},
+    )
+
+
+@app.post(
+    "/uploads/{upload_id}/parts/{part_no}/signed_urls",
+    summary="ulc_post_uploads_parts_files_signed_urls_mock",
+    status_code=200,
+)
+async def ulc_post_uploads_parts_files_signed_posts(upload_id: str, part_no: int):
+    """
+    Mock for the ulc POST /uploads/{upload_id}/parts/{part_no}/signed_urls call.
+    """
+
+    if upload_id == "pending":
+        if part_no == 1:
+            url = os.environ["S3_UPLOAD_URL_1"]
+            return {"url": url}
+        if part_no == 2:
+            url = os.environ["S3_UPLOAD_URL_2"]
+            return {"url": url}
+
+    raise HttpyException(
+        status_code=404,
+        exception_id="noSuchUpload",
+        description=f'The file with the upload id "{upload_id}" does not exist.',
+        data={"upload_id": upload_id},
+    )
+
+
+@app.patch("/uploads/{upload_id}", summary="ulc_patch_uploads_mock", status_code=204)
+async def ulc_patch_uploads(upload_id: str, state: StatePatch):
+    """
+    Mock for the ulc PATCH /uploads/{upload_id} call
+    """
+    upload_status = state.status
+
+    if upload_id == "uploaded":
+        if upload_status == UploadStatus.CANCELLED:
+            return JSONResponse(None, status_code=status.HTTP_204_NO_CONTENT)
+
+        raise HttpyException(
+            status_code=400,
+            exception_id="uploadNotPending",
+            description=f'The upload with id "{upload_id}" can`t be set to "{upload_status}"',
+            data={"upload_id": upload_id, "current_upload_status": upload_id},
         )
-        return multipart_upload
-    except exceptions.NoUploadPossibleError as error:
-        file_metadata = get_file_metadata(api_url=api_url, file_id=file_id)
-        upload_id = file_metadata["current_upload_id"]
-        if upload_id is None:
-            raise error
-
-        patch_multipart_upload(
-            api_url=api_url,
-            upload_id=upload_id,
-            upload_status=UploadStatus.CANCELLED,
-        )
-
-        multipart_upload = initiate_multipart_upload(
-            api_url=api_url, file_id=file_id, pubkey_path=pubkey_path
-        )
-
-    except Exception as error:
-        raise error
-
-    return multipart_upload
-
-
-def await_download_url(
-    *,
-    api_url: str,
-    file_id: str,
-    max_wait_time: int,
-    message_display: AbstractMessageDisplay,
-    pubkey_path: Path,  # pylint: disable=unused-argument
-) -> Tuple[str, int]:
-    """Wait until download URL can be generated.
-    Returns a tuple with two elements:
-        1. the download url
-        2. the file size in bytes
-    """
-
-    # get the download_url, wait if needed
-    wait_time = 0
-    while wait_time < max_wait_time:
-        try:
-            response_body = download_api_call(api_url=api_url, file_id=file_id)
-        except exceptions.BadResponseCodeError as error:
-            message_display.failure(
-                "The request was invalid and returnd a wrong HTTP status code."
-            )
-            raise error
-        except exceptions.RequestFailedError as error:
-            message_display.failure("The request has failed.")
-            raise error
-
-        if response_body[0] is not None:
-            download_url: str = response_body[0]
-            file_size: int = response_body[1]
-            return (download_url, file_size)
-
-        retry_time: int = response_body[2]
-
-        wait_time += retry_time
-        message_display.display(
-            f"File staging, will try to download again in {retry_time} seconds"
+
+    if upload_id == "pending":
+        if upload_status == UploadStatus.UPLOADED:
+            return JSONResponse(None, status_code=status.HTTP_204_NO_CONTENT)
+
+        raise HttpyException(
+            status_code=400,
+            exception_id="uploadStatusChange",
+            description=f'The upload with id "{upload_id}" can`t be set to "{upload_status}"',
+            data={"upload_id": upload_id, "target_status": upload_status},
         )
-        sleep(retry_time)
 
-    raise exceptions.MaxWaitTimeExceededError(max_wait_time=max_wait_time)
+    if upload_id == "uploadable":
+        raise HttpyException(
+            status_code=400,
+            exception_id="uploadNotPending",
+            description=f'The upload with id "{upload_id}" can`t be set to "{upload_status}"',
+            data={"upload_id": upload_id, "current_upload_status": upload_id},
+        )
+
+    raise HttpyException(
+        status_code=404,
+        exception_id="noSuchUpload",
+        description=f'The upload with id "{upload_id}" does not exist',
+        data={"upload_id": upload_id},
+    )
+
+
+@app.post(
+    "/work-packages/{package_id}/files/{file_id}/work-order-tokens", status_code=201
+)
+async def create_work_order_token(
+    package_id: str, file_id: str, authorization=Header()
+):
+    """Mock Work Order Token endpoint"""
+
+    # has to be at least 48 chars long
+    return base64.b64encode(b"1234567890" * 5).decode()
```

### Comparing `ghga_connector-0.2.6/ghga_connector/core/constants.py` & `ghga_connector-0.3.3/ghga_connector/core/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Constants used throught the core."""
 
 DEFAULT_PART_SIZE = 16 * 1024 * 1024
-TIMEOUT = 120
+TIMEOUT = 60
 MAX_PART_NUMBER = 10000
 MAX_RETRIES = 5
 MAX_WAIT_TIME = 60 * 60
```

### Comparing `ghga_connector-0.2.6/ghga_connector/core/file_operations.py` & `ghga_connector-0.3.3/ghga_connector/core/file_operations.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,48 +14,144 @@
 # limitations under the License.
 #
 
 """
 Contains Calls of the Presigned URLs in order to Up- and Download Files
 """
 
+import base64
+import concurrent.futures
 import math
 from io import BufferedReader
-from typing import Iterator, Sequence
+from pathlib import Path
+from queue import Queue
+from tempfile import mkstemp
+from typing import Any, Iterator, Sequence, Tuple, Union
 
+import crypt4gh.keys
+import crypt4gh.lib
 import requests
 
 from ghga_connector.core import exceptions
 from ghga_connector.core.constants import TIMEOUT
 from ghga_connector.core.session import RequestsSession
 
 
+class Crypt4GHEncryptor:
+    """Convenience class to deal with Crypt4GH encryption"""
+
+    def __init__(
+        self,
+        server_pubkey: str,
+        submitter_private_key_path: Path,
+    ) -> None:
+        self.server_public = base64.b64decode(server_pubkey)
+        self.submitter_private = crypt4gh.keys.get_private_key(
+            submitter_private_key_path, callback=None
+        )
+
+    def encrypt_file(self, *, file_path: Path) -> Path:
+        """Encrypt provided file using Crypt4GH lib"""
+        keys = [(0, self.submitter_private, self.server_public)]
+        with file_path.open("rb") as infile:
+            # NamedTemporaryFile cannot be opened a second time on Windows, manually
+            # deal with setup + teardown instead
+            raw_fd, outfile_path = mkstemp()
+            with open(raw_fd, "wb") as outfile:
+                crypt4gh.lib.encrypt(keys=keys, infile=infile, outfile=outfile)
+            return Path(outfile_path)
+
+
+class Crypt4GHDecryptor:
+    """Convenience class to deal with Crypt4GH decryption"""
+
+    def __init__(self, decryption_key_path: Path):
+        self.decryption_key = crypt4gh.keys.get_private_key(
+            decryption_key_path, callback=None
+        )
+
+    def decrypt_file(self, *, input_path: Path, output_path: Path):
+        """Decrypt provided file using Crypt4GH lib"""
+        keys = [(0, self.decryption_key, None)]
+        with input_path.open("rb") as infile:
+            with output_path.open("wb") as outfile:
+                crypt4gh.lib.decrypt(keys=keys, infile=infile, outfile=outfile)
+
+
+def is_file_encrypted(file_path: Path):
+    """Checks if a file is Crypt4GH encrypted"""
+
+    with file_path.open("rb") as input_file:
+        num_relevant_bytes = 12
+        file_header = input_file.read(num_relevant_bytes)
+
+        magic_number = b"crypt4gh"
+        version = b"\x01\x00\x00\x00"
+
+        if file_header != magic_number + version:
+            return False
+
+    # If file header is correct, assume file is Crypt4GH encrypted
+    return True
+
+
 def download_content_range(
     *,
     download_url: str,
     start: int,
     end: int,
-) -> bytes:
+    queue: Queue,
+) -> None:
     """Download a specific range of a file's content using a presigned download url."""
 
     headers = {"Range": f"bytes={start}-{end}"}
     try:
-        response = RequestsSession.get(download_url, headers=headers, timeout=TIMEOUT)
+        response = RequestsSession.get(
+            download_url, headers=headers, timeout=TIMEOUT, allow_redirects=False
+        )
     except requests.exceptions.RequestException as request_error:
         exceptions.raise_if_max_retries(request_error=request_error, url=download_url)
         raise exceptions.RequestFailedError(url=download_url) from request_error
 
     status_code = response.status_code
-    # 200, if the full file was returned, 206 else
+
+    # 200, if the full file was returned, 206 else.
     if status_code in (200, 206):
-        return response.content
+        queue.put((start, response.content))
+        return
 
     raise exceptions.BadResponseCodeError(url=download_url, response_code=status_code)
 
 
+def download_file_parts(
+    max_concurrent_downloads: int,
+    queue: Queue,
+    part_ranges: Sequence[Tuple[int, int]],
+    download_urls: Iterator[Union[Tuple[None, None, int], Tuple[str, int, None]]],
+    download_part_funct=download_content_range,
+) -> None:
+    """
+    Download stuff
+    """
+    # Download the parts using a thread pool executor
+    executor = concurrent.futures.ThreadPoolExecutor(
+        max_workers=max_concurrent_downloads,
+    )
+
+    for part_range, download_url in zip(part_ranges, download_urls):
+        kwargs: dict[str, Any] = {
+            "download_url": download_url[0],
+            "start": part_range[0],
+            "end": part_range[1],
+            "queue": queue,
+        }
+
+        executor.submit(download_part_funct, **kwargs)
+
+
 def calc_part_ranges(
     *, part_size: int, total_file_size: int, from_part: int = 1
 ) -> Sequence[tuple[int, int]]:
     """
     Calculate and return the ranges (start, end) of file parts as a list of tuples.
 
     By default it starts with the first part but you may also start from a specific part
@@ -66,47 +162,20 @@
     full_part_number = math.floor(total_file_size / part_size)
     part_ranges = [
         (part_size * (part_no - 1), part_size * part_no - 1)
         for part_no in range(from_part, full_part_number + 1)
     ]
 
     if (total_file_size % part_size) > 0:
-        # if the last part is smaller than the part_size, calculate it range separately:
+        # if the last part is smaller than the part_size, calculate its range separately:
         part_ranges.append((part_size * full_part_number, total_file_size - 1))
 
     return part_ranges
 
 
-def download_file_parts(
-    *,
-    download_url: str,
-    part_size: int,
-    total_file_size: int,
-    from_part: int = 1,
-    download_range_func=download_content_range,
-    calc_ranges_func=calc_part_ranges,
-) -> Iterator[bytes]:
-    """
-    Returns an iterator to obtain the bytes content of a file in a part by part fashion.
-
-    By default it start with the first part but you may also start from a specific part
-    in the middle of the file using the `from_part` argument. This might be useful to
-    resume an interrupted reading process.
-    """
-
-    part_ranges = calc_ranges_func(
-        part_size=part_size, total_file_size=total_file_size, from_part=from_part
-    )
-
-    for part_start, part_end in part_ranges:
-        yield download_range_func(
-            download_url=download_url, start=part_start, end=part_end
-        )
-
-
 def read_file_parts(
     file: BufferedReader, *, part_size: int, from_part: int = 1
 ) -> Iterator[bytes]:
     """
     Returns an iterator to iterate through file parts of the given size (in bytes).
 
     By default it start with the first part but you may also start from a specific part
```

### Comparing `ghga_connector-0.2.6/ghga_connector/core/http_translation.py` & `ghga_connector-0.3.3/ghga_connector/core/http_translation.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/ghga_connector/core/message_display.py` & `ghga_connector-0.3.3/ghga_connector/core/message_display.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/ghga_connector/core/session.py` & `ghga_connector-0.3.3/ghga_connector/core/session.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/ghga_connector.egg-info/SOURCES.txt` & `ghga_connector-0.3.3/ghga_connector.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,27 @@
 ghga_connector.egg-info/SOURCES.txt
 ghga_connector.egg-info/dependency_links.txt
 ghga_connector.egg-info/entry_points.txt
 ghga_connector.egg-info/not-zip-safe
 ghga_connector.egg-info/requires.txt
 ghga_connector.egg-info/top_level.txt
 ghga_connector/core/__init__.py
-ghga_connector/core/api_calls.py
+ghga_connector/core/batch_processing.py
 ghga_connector/core/constants.py
 ghga_connector/core/exceptions.py
 ghga_connector/core/file_operations.py
 ghga_connector/core/http_translation.py
 ghga_connector/core/main.py
 ghga_connector/core/message_display.py
 ghga_connector/core/session.py
+ghga_connector/core/api_calls/__init__.py
+ghga_connector/core/api_calls/download.py
+ghga_connector/core/api_calls/upload.py
+ghga_connector/core/api_calls/utils.py
+ghga_connector/core/api_calls/work_package.py
 tests/fixtures/__init__.py
 tests/fixtures/config.py
 tests/fixtures/s3.py
 tests/fixtures/state.py
 tests/fixtures/utils.py
 tests/fixtures/mock_api/__init__.py
 tests/fixtures/mock_api/app.py
```

### Comparing `ghga_connector-0.2.6/setup.cfg` & `ghga_connector-0.3.3/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -16,32 +16,24 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	ghga-service-chassis-lib[s3]==0.17.4
-	httpyexpect==0.2.4
 	typer==0.7.0
 	crypt4gh==1.6
+	ghga-service-commons[api, crypt]==0.4.2
+	hexkit[s3]==0.10.0
 python_requires = >= 3.9.10
 
 [options.entry_points]
 console_scripts = 
 	ghga-connector = ghga_connector.__main__:run
 
-[options.extras_require]
-dev = 
-	ghga-service-chassis-lib[dev]==0.17.4
-	fastapi==0.89.1
-	uvicorn[standard]==0.20.0
-all = 
-	%(dev)s
-
 [options.packages.find]
 exclude = tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ghga_connector-0.2.6/setup.py` & `ghga_connector-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/tests/fixtures/__init__.py` & `ghga_connector-0.3.3/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/tests/fixtures/config.py` & `ghga_connector-0.3.3/tests/fixtures/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 DEFAULT_TEST_CONFIG = Config(
     upload_api="http:/example.org/upload",
     download_api="http:/example.org/download",
     max_retries=0,
     max_wait_time=2,
     part_size=core.DEFAULT_PART_SIZE,
+    server_pubkey="qx5g31H7rdsq7sgkew9ElkLIXvBje4RxDVcAHcJD8XY=",
+    wps_api_url="http://127.0.0.1",
 )
 
 
 def get_test_config(**kwargs):
     """Get test config params with the defaults being overwritting by the parameter
     passed as kwargs.
     """
```

### Comparing `ghga_connector-0.2.6/tests/fixtures/mock_api/__init__.py` & `ghga_connector-0.3.3/tests/fixtures/mock_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/tests/fixtures/mock_api/testcontainer.py` & `ghga_connector-0.3.3/tests/fixtures/mock_api/testcontainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,34 +33,36 @@
 
     def __init__(
         self,
         s3_download_url: str = "test://download.url",
         s3_upload_url_1: str = "test://upload.url",
         s3_upload_url_2: str = "test://upload.url",
         s3_download_file_size: int = 146,
-        image: str = "ghga/fastapi_essentials:0.73.0",
+        fake_envelope: str = "Fake_envelope",
+        image: str = "ghga/fastapi_essentials:0.94.1",
         port: int = 8000,
     ) -> None:
         """Initialize the Fastapi test container.
 
         Args:
             image (str, optional):
-                The docker image from docker hub. Defaults to "ghga/fastapi_essentials:0.73.0".
+                The docker image from docker hub. Defaults to "ghga/fastapi_essentials:0.94.1".
             port (int, optional):
                 The port to reach the FastAPI. Defaults to 8000.
         """
-        super(MockAPIContainer, self).__init__(image=image)
+        super().__init__(image=image)
 
         self._port = port
 
         self.with_exposed_ports(self._port)
         self.with_env("S3_DOWNLOAD_URL", s3_download_url)
         self.with_env("S3_UPLOAD_URL_1", s3_upload_url_1)
         self.with_env("S3_UPLOAD_URL_2", s3_upload_url_2)
         self.with_env("S3_DOWNLOAD_FIELD_SIZE", s3_download_file_size)
+        self.with_env("FAKE_HEADER_ENVELOPE", fake_envelope)
         self.with_volume_mapping(host=str(APP_MODULE_PATH), container="/app.py")
         self.with_command(
             f"python3 -m uvicorn --host 0.0.0.0 --port {self._port} --app-dir / app:app"
         )
 
     def get_connection_url(self) -> str:
         """Returns an HTTP connection URL to the API root."""
```

### Comparing `ghga_connector-0.2.6/tests/fixtures/state.py` & `ghga_connector-0.3.3/tests/fixtures/state.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 # limitations under the License.
 
 """Test data"""
 
 from pathlib import Path
 from typing import Dict, List
 
-from ghga_service_chassis_lib.object_storage_dao_testing import ObjectFixture
-from ghga_service_chassis_lib.utils import TEST_FILE_PATHS
+from hexkit.providers.s3.testutils import TEST_FILE_PATHS, FileObject
 
 
 class FileState:
     """_
     File State class for available files
     """
 
@@ -40,26 +39,32 @@
         Set populate_storage to true in order to upload them to the localstack storage
         """
         self.file_id = file_id
         self.grouping_label = grouping_label
         self.file_path = file_path
         self.populate_storage = populate_storage
 
-        self.storage_objects: List[ObjectFixture] = []
+        self.storage_objects: List[FileObject] = []
         if self.populate_storage:
             self.storage_objects.append(
-                ObjectFixture(
+                FileObject(
                     file_path=self.file_path,
                     bucket_id=self.grouping_label,
                     object_id=self.file_id,
                 )
             )
 
 
 FILES: Dict[str, FileState] = {
+    "encrypted_file": FileState(
+        file_id="encrypted",
+        grouping_label="inbox",
+        file_path=TEST_FILE_PATHS[0],
+        populate_storage=False,
+    ),
     "file_uploadable": FileState(
         file_id="uploadable",
         grouping_label="inbox",
         file_path=TEST_FILE_PATHS[0],
         populate_storage=False,
     ),
     "file_not_uploadable": FileState(
@@ -82,14 +87,20 @@
     ),
     "file_downloadable": FileState(
         file_id="downloadable",
         grouping_label="outbox",
         file_path=TEST_FILE_PATHS[3],
         populate_storage=True,
     ),
+    "file_envelope_missing": FileState(
+        file_id="envelope-missing",
+        grouping_label="outbox",
+        file_path=TEST_FILE_PATHS[3],
+        populate_storage=True,
+    ),
     "file_not_downloadable": FileState(
         file_id="not-downloadable",
         grouping_label="outbox",
         file_path=TEST_FILE_PATHS[1],
         populate_storage=False,
     ),
     "file_retry": FileState(
```

### Comparing `ghga_connector-0.2.6/tests/fixtures/utils.py` & `ghga_connector-0.3.3/tests/integration/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/tests/integration/__init__.py` & `ghga_connector-0.3.3/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/tests/integration/fixtures/__init__.py` & `ghga_connector-0.3.3/tests/integration/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/tests/integration/fixtures/utils.py` & `ghga_connector-0.3.3/tests/unit/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/tests/integration/test_file_operations.py` & `ghga_connector-0.3.3/tests/integration/test_file_operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Test file operations"""
 
-from typing import Optional
+from queue import Queue
+from typing import Any, Iterator, Tuple, Union
 
 import pytest
 
 from ghga_connector.core.file_operations import (
+    calc_part_ranges,
     download_content_range,
     download_file_parts,
 )
 from tests.fixtures.s3 import S3Fixture, get_big_s3_object, s3_fixture  # noqa: F401
 
 
 @pytest.mark.parametrize(
@@ -34,67 +36,83 @@
         (  # download intermediate part:
             5 * 1024 * 1024,
             10 * 1024 * 1024 - 1,
             20 * 1024 * 1024,
         ),
     ],
 )
-def test_download_content_range(
+@pytest.mark.asyncio
+async def test_download_content_range(
     start: int,
     end: int,
     file_size: int,
     s3_fixture: S3Fixture,  # noqa: F811
 ):
     """Test the `download_content_range` function."""
     # prepare state and the expected result:
-    big_object = get_big_s3_object(s3_fixture, object_size=file_size)
-    download_url = s3_fixture.storage.get_object_download_url(
+    big_object = await get_big_s3_object(s3_fixture, object_size=file_size)
+    download_url = await s3_fixture.storage.get_object_download_url(
         object_id=big_object.object_id, bucket_id=big_object.bucket_id
     )
     expected_bytes = big_object.content[start : end + 1]
 
+    queue: Queue = Queue(maxsize=10)
+
     # donwload content range with dedicated function:
-    obtained_bytes = download_content_range(
-        download_url=download_url, start=start, end=end
-    )
+    download_content_range(download_url=download_url, start=start, end=end, queue=queue)
+
+    obtained_start, obtained_bytes = queue.get()
 
+    assert start == obtained_start
     assert expected_bytes == obtained_bytes
 
 
 @pytest.mark.parametrize(
-    "from_part",
-    [None, 3],
+    "part_size",
+    [5 * 1024 * 1024, 3 * 1024 * 1024, 1 * 1024 * 1024],
 )
-def test_download_file_parts(
-    from_part: Optional[int],
+@pytest.mark.asyncio
+async def test_download_file_parts(
+    part_size: int,
     s3_fixture: S3Fixture,  # noqa: F811
 ):
     """Test the `download_file_parts` function."""
     # prepare state and the expected result:
-    part_size = 5 * 1024 * 1024
-    big_object = get_big_s3_object(s3_fixture)
+    big_object = await get_big_s3_object(s3_fixture)
     total_file_size = len(big_object.content)
-    if from_part is not None:
-        offset = (from_part - 1) * part_size
-        expected_bytes = big_object.content[offset:total_file_size]
-    else:
-        expected_bytes = big_object.content
+    expected_bytes = big_object.content
 
-    download_url = s3_fixture.storage.get_object_download_url(
+    download_url = await s3_fixture.storage.get_object_download_url(
         object_id=big_object.object_id, bucket_id=big_object.bucket_id
     )
 
+    def url_generator() -> (
+        Iterator[Union[Tuple[None, None, int], Tuple[str, int, None]]]
+    ):
+        while True:
+            yield download_url, 0, None
+
+    download_urls = url_generator()
+
+    queue: Queue = Queue(maxsize=10)
+
+    part_ranges = calc_part_ranges(part_size=part_size, total_file_size=total_file_size)
+
     # prepare kwargs:
-    kwargs = {
-        "download_url": download_url,
-        "part_size": part_size,
-        "total_file_size": total_file_size,
+    kwargs: dict[str, Any] = {
+        "download_urls": download_urls,
+        "queue": queue,
+        "part_ranges": part_ranges,
+        "max_concurrent_downloads": 5,
     }
-    if from_part is not None:
-        kwargs["from_part"] = from_part
 
     # donwload file parts with dedicated function:
-    obtained_bytes = bytes()
-    for part in download_file_parts(**kwargs):
-        obtained_bytes += part
+    download_file_parts(**kwargs)
 
-    assert expected_bytes == obtained_bytes
+    obtained = 0
+    while obtained < len(expected_bytes):
+        start, obtained_bytes = queue.get()
+        obtained += len(obtained_bytes)
+        queue.task_done()
+        assert expected_bytes[start : start + part_size] == obtained_bytes
+
+    assert obtained == len(expected_bytes)
```

### Comparing `ghga_connector-0.2.6/tests/unit/__init__.py` & `ghga_connector-0.3.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/tests/unit/fixtures/__init__.py` & `ghga_connector-0.3.3/tests/unit/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.2.6/tests/unit/test_core.py` & `ghga_connector-0.3.3/tests/unit/test_core.py`

 * *Files identical despite different names*

