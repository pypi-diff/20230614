# Comparing `tmp/awsparams-1.5.2.tar.gz` & `tmp/awsparams-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsparams-1.5.2.tar", max compression
+gzip compressed data, was "awsparams-1.5.3.tar", max compression
```

## Comparing `awsparams-1.5.2.tar` & `awsparams-1.5.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-05-18 17:00:43.569322 awsparams-1.5.2/LICENSE
--rw-r--r--   0        0        0     4765 2023-05-18 17:00:43.569322 awsparams-1.5.2/README.md
--rw-r--r--   0        0        0    10098 2023-05-18 17:00:43.569322 awsparams-1.5.2/awsparams/__init__.py
--rwxr-xr-x   0        0        0    10779 2023-05-18 17:00:43.569322 awsparams-1.5.2/awsparams/cli.py
--rw-r--r--   0        0        0      680 2023-05-18 17:00:43.569322 awsparams-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     5658 1970-01-01 00:00:00.000000 awsparams-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-14 14:22:05.906460 awsparams-1.5.3/LICENSE
+-rw-r--r--   0        0        0     4765 2023-06-14 14:22:05.906460 awsparams-1.5.3/README.md
+-rw-r--r--   0        0        0    10098 2023-06-14 14:22:05.906460 awsparams-1.5.3/awsparams/__init__.py
+-rwxr-xr-x   0        0        0    11420 2023-06-14 14:22:05.906460 awsparams-1.5.3/awsparams/cli.py
+-rw-r--r--   0        0        0      680 2023-06-14 14:22:05.906460 awsparams-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     5658 1970-01-01 00:00:00.000000 awsparams-1.5.3/PKG-INFO
```

### Comparing `awsparams-1.5.2/LICENSE` & `awsparams-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `awsparams-1.5.2/README.md` & `awsparams-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `awsparams-1.5.2/awsparams/__init__.py` & `awsparams-1.5.3/awsparams/__init__.py`

 * *Files identical despite different names*

### Comparing `awsparams-1.5.2/awsparams/cli.py` & `awsparams-1.5.3/awsparams/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
+from botocore.exceptions import ProfileNotFound, NoRegionError, SSOTokenLoadError, UnauthorizedSSOTokenError
 
 from awsparams import __VERSION__, AWSParams
 
 
 def sanity_check(param: str, force: bool) -> bool:
     if force:
         return True
@@ -44,24 +45,40 @@
     help="by default display decrypted values",
     default=True,
 )
 def ls(prefix="", profile="", region="", delimiter="", values=False, dot_env=False, tfvars=False, jetbrains_run_config=False, esc_quotes=False, decryption=True):
     """
     List Parameters, optionally matching a specific prefix
     """
-    aws_params = AWSParams(profile, region)
+    aws_params = None
+    try:
+        aws_params = AWSParams(profile, region)
+    except ProfileNotFound:
+        print('Error: profile specified with AWS_PROFILE not found! Please specify a valid profile.')
+        quit()
+    except NoRegionError:
+        print('Error: no profile specified, or no region specified.')
+        quit()
+
     if jetbrains_run_config or dot_env or tfvars:  # all of these options should also fetch the values
         values = True
     if not values:
         decryption = False
     if not delimiter:
         delimiter = "/"
-    for parm in aws_params.get_all_parameters(
+    all_params = []
+    try:
+        all_params = aws_params.get_all_parameters(
             prefix=prefix, values=values, decryption=decryption, trim_name=False
-    ):
+        )
+    except (SSOTokenLoadError, UnauthorizedSSOTokenError):
+        print('Error: Your AWS SSO credentials are invalid or have expired. Please log in again.')
+        quit()
+
+    for parm in all_params:
         if values:
             if jetbrains_run_config or dot_env or tfvars:
                 param_parts = parm.Name.split(delimiter)
                 prefix_parts = prefix.split(delimiter)
                 # remove any duplicate, leading, or trailing delimiters from both lists
                 for arr in [param_parts, prefix_parts]:
                     for part in arr:
@@ -90,14 +107,15 @@
                 elif jetbrains_run_config:
                     click.echo(f"{name}={parm.Value};")
             else:
                 click.echo(f"{parm.Name}: {parm.Value}")
         else:
             click.echo(parm.Name)
 
+
 def escape_quotes(string):
     newstr = ''
     for c in string:
         if c == '"':
             newstr += '\\"'
         else:
             newstr += c
```

### Comparing `awsparams-1.5.2/pyproject.toml` & `awsparams-1.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awsparams"
-version = "1.5.2"
+version = "1.5.3"
 description = "A simple CLI and Library for adding/removing/renaming/copying AWS Param Store Parameters"
 authors = ["Nate Peterson <ndpete@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/byu-oit/awsparams"
 repository = "https://github.com/byu-oit/awsparams"
```

### Comparing `awsparams-1.5.2/PKG-INFO` & `awsparams-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsparams
-Version: 1.5.2
+Version: 1.5.3
 Summary: A simple CLI and Library for adding/removing/renaming/copying AWS Param Store Parameters
 Home-page: https://github.com/byu-oit/awsparams
 License: Apache-2.0
 Author: Nate Peterson
 Author-email: ndpete@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

