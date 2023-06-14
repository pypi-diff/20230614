# Comparing `tmp/slack-watchman-4.0.1.tar.gz` & `tmp/slack-watchman-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-watchman-4.0.1.tar", last modified: Fri May  5 08:08:19 2023, max compression
+gzip compressed data, was "slack-watchman-4.0.2.tar", last modified: Wed Jun 14 20:06:59 2023, max compression
```

## Comparing `slack-watchman-4.0.1.tar` & `slack-watchman-4.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.374801 slack-watchman-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-05-05 08:08:19.374801 slack-watchman-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-05 08:08:19.378800 slack-watchman-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.370800 slack-watchman-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.370800 slack-watchman-4.0.1/src/slack_watchman/
--rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.374801 slack-watchman-4.0.1/src/slack_watchman/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/signature_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/slack_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/sw_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.374801 slack-watchman-4.0.1/src/slack_watchman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:06:59.085652 slack-watchman-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14350 2023-06-14 20:06:59.085652 slack-watchman-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-14 20:06:59.085652 slack-watchman-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:06:59.081652 slack-watchman-4.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:06:59.081652 slack-watchman-4.0.2/src/slack_watchman/
+-rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:06:59.085652 slack-watchman-4.0.2/src/slack_watchman/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/models/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/models/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/signature_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/slack_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-06-14 20:06:44.000000 slack-watchman-4.0.2/src/slack_watchman/sw_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:06:59.085652 slack-watchman-4.0.2/src/slack_watchman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14350 2023-06-14 20:06:59.000000 slack-watchman-4.0.2/src/slack_watchman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-14 20:06:59.000000 slack-watchman-4.0.2/src/slack_watchman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:06:59.000000 slack-watchman-4.0.2/src/slack_watchman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 20:06:59.000000 slack-watchman-4.0.2/src/slack_watchman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:06:58.000000 slack-watchman-4.0.2/src/slack_watchman.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 20:06:59.000000 slack-watchman-4.0.2/src/slack_watchman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 20:06:59.000000 slack-watchman-4.0.2/src/slack_watchman.egg-info/top_level.txt
```

### Comparing `slack-watchman-4.0.1/CHANGELOG.md` & `slack-watchman-4.0.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## [4.0.2] - 2023-06-14
+### Added
+- Added notification for an invalid cookie being passed (Fixes #47)
+### Fixed
+- JSON output for User and Workspace information was malformed, this has now been fixed
+
 ## [4.0.1] - 2023-05-05
 ### Changed
 - User output in stdout logging now includes display name and email. The accounts for cases where usernames are nonsensical.
 
 ## [4.0.0] - 2023-05-03
 This major version release brings multiple updates to Slack Watchman in usability, functionality and behind the scenes improvements.
```

### Comparing `slack-watchman-4.0.1/LICENSE` & `slack-watchman-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/PKG-INFO` & `slack-watchman-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-watchman
-Version: 4.0.1
+Version: 4.0.2
 Summary: Monitoring and enumerating Slack for exposed secrets
 Home-page: https://github.com/PaperMtn/slack-watchman
 Author: PaperMtn
 Author-email: papermtn@protonmail.com
 License: GPL-3.0
 Keywords: audit,slack,slack-watchman,watchman,blue-team,red-team,threat-hunting
 Classifier: Intended Audience :: Information Technology
@@ -201,14 +201,20 @@
 You may be interested in the other apps in the Watchman family:
 - [Slack Watchman for Enterprise Grid](https://github.com/PaperMtn/slack-watchman-enterprise-grid)
 - [GitLab Watchman](https://github.com/PaperMtn/gitlab-watchman)
 - [GitHub Watchman](https://github.com/PaperMtn/github-watchman)
 
 ## License
 The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack Technologies or Salesforce.
+## [4.0.2] - 2023-06-14
+### Added
+- Added notification for an invalid cookie being passed (Fixes #47)
+### Fixed
+- JSON output for User and Workspace information was malformed, this has now been fixed
+
 ## [4.0.1] - 2023-05-05
 ### Changed
 - User output in stdout logging now includes display name and email. The accounts for cases where usernames are nonsensical.
 
 ## [4.0.0] - 2023-05-03
 This major version release brings multiple updates to Slack Watchman in usability, functionality and behind the scenes improvements.
```

### Comparing `slack-watchman-4.0.1/README.md` & `slack-watchman-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/setup.cfg` & `slack-watchman-4.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/src/slack_watchman/__init__.py` & `slack-watchman-4.0.2/src/slack_watchman/__init__.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/src/slack_watchman/__version__.py` & `slack-watchman-4.0.2/src/slack_watchman/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     '__version__',
     '__author__',
     '__email__',
     '__license__',
 ]
 
 __title__ = 'Slack Watchman'
-__version__ = '4.0.1'
+__version__ = '4.0.2'
 __summary__ = 'Monitoring and enumerating Slack for exposed secrets'
 __author__ = 'PaperMtn'
 __email__ = 'papermtn@protonmail.com'
 __license__ = 'GPL-3.0'
 __uri__ = 'https://github.com/PaperMtn/slack-watchman'
 __copyright__ = f'2023 {__author__}'
```

### Comparing `slack-watchman-4.0.1/src/slack_watchman/exceptions.py` & `slack-watchman-4.0.2/src/slack_watchman/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,25 @@
 
     def __init__(self, config_entry):
         self.config_entry = config_entry
         self.message = f'Missing variable in the config file: {self.config_entry}'
         super().__init__(self.message)
 
 
+class InvalidCookieError(Exception):
+    """ Exception raised when the provided cookie is not valid, or it does not
+        nave access to the workspace given.
+    """
+
+    def __init__(self, domain):
+        self.message = "The cookie may not be valid or, if it is valid," \
+                       f" the user it belongs to cant authenticate to the Slack workspace {domain}"
+        super().__init__(self.message)
+
+
 class SlackScopeError(Exception):
     """ Exception raised when the authed user doesn't have the required API scopes
     """
 
     def __init__(self, scope):
         self.scope = scope
         self.message = f'Slack API token is missing the required scope: {self.scope}'
```

### Comparing `slack-watchman-4.0.1/src/slack_watchman/models/conversation.py` & `slack-watchman-4.0.2/src/slack_watchman/models/conversation.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/src/slack_watchman/models/post.py` & `slack-watchman-4.0.2/src/slack_watchman/models/post.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/src/slack_watchman/models/signature.py` & `slack-watchman-4.0.2/src/slack_watchman/models/signature.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/src/slack_watchman/models/user.py` & `slack-watchman-4.0.2/src/slack_watchman/models/user.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/src/slack_watchman/models/workspace.py` & `slack-watchman-4.0.2/src/slack_watchman/models/workspace.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/src/slack_watchman/signature_updater.py` & `slack-watchman-4.0.2/src/slack_watchman/signature_updater.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.1/src/slack_watchman/slack_wrapper.py` & `slack-watchman-4.0.2/src/slack_watchman/slack_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,20 @@
             })
 
     def _get_session_token(self) -> str:
 
         r = requests.get(self.url, cookies=self.cookie_dict).text
         regex = '(xox[a-zA-Z]-[a-zA-Z0-9-]+)'
 
-        return re.search(regex, r)[0]
+        try:
+            return re.search(regex, r)[0]
+        except TypeError:
+            raise exceptions.InvalidCookieError(self.url)
+        except:
+            raise
 
     def _make_request(self, url, params=None, data=None, method='GET', verify_ssl=True):
         try:
             relative_url = '/'.join((self.base_url, url))
             response = self.session.request(
                 method,
                 relative_url,
```

### Comparing `slack-watchman-4.0.1/src/slack_watchman/sw_logger.py` & `slack-watchman-4.0.2/src/slack_watchman/sw_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         ⠀⠀⠀⠀⠀⠀⣠⣾⣿⣿⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
         ⠀⠀⠀⠀⣠⣾⣿⣿⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
         ⠀⠀⠀⣾⣿⣿⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
         ⠀ ⠈⠛⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
         """ + Style.RESET_ALL
               )
         print('   Slack Watchman     ')
-        print(Style.DIM + '   Detect exposed secrets in Slack      ' + Style.RESET_ALL)
+        print(Style.DIM + '   Slack enumeration and exposed secrets detection tool      ' + Style.RESET_ALL)
         print('  ')
         print(Style.BRIGHT + '   by PaperMtn - GNU General Public License')
         print(' '.ljust(79) + Fore.GREEN)
 
 
 class EnhancedJSONEncoder(json.JSONEncoder):
     def default(self, o):
@@ -215,17 +215,17 @@
             '{"timestamp": "%(asctime)s", "level": "NOTIFY", "scope": "%(scope)s", "severity": '
             '"%(severity)s", "detection_type": "%(type)s", "detection_data": %(message)s}')
         self.info_format = logging.Formatter(
             '{"timestamp": "%(asctime)s", "level": "%(levelname)s", "message": "%(message)s"}')
         self.success_format = logging.Formatter(
             '{"timestamp": "%(asctime)s", "level": "SUCCESS", "message": "%(message)s"}')
         self.user_format = logging.Formatter(
-            '{"timestamp": "%(asctime)s", "level": "USER", "message": "%(message)s"}')
+            '{"timestamp": "%(asctime)s", "level": "USER", "message": %(message)s}')
         self.workspace_format = logging.Formatter(
-            '{"timestamp": "%(asctime)s", "level": "WORKSPACE", "message": "%(message)s"}')
+            '{"timestamp": "%(asctime)s", "level": "WORKSPACE", "message": %(message)s}')
         self.logger = logging.getLogger(self.name)
         self.handler = logging.StreamHandler(sys.stdout)
         self.logger.addHandler(self.handler)
         if kwargs.get('debug'):
             self.logger.setLevel(logging.DEBUG)
         else:
             self.logger.setLevel(logging.INFO)
```

### Comparing `slack-watchman-4.0.1/src/slack_watchman.egg-info/PKG-INFO` & `slack-watchman-4.0.2/src/slack_watchman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-watchman
-Version: 4.0.1
+Version: 4.0.2
 Summary: Monitoring and enumerating Slack for exposed secrets
 Home-page: https://github.com/PaperMtn/slack-watchman
 Author: PaperMtn
 Author-email: papermtn@protonmail.com
 License: GPL-3.0
 Keywords: audit,slack,slack-watchman,watchman,blue-team,red-team,threat-hunting
 Classifier: Intended Audience :: Information Technology
@@ -201,14 +201,20 @@
 You may be interested in the other apps in the Watchman family:
 - [Slack Watchman for Enterprise Grid](https://github.com/PaperMtn/slack-watchman-enterprise-grid)
 - [GitLab Watchman](https://github.com/PaperMtn/gitlab-watchman)
 - [GitHub Watchman](https://github.com/PaperMtn/github-watchman)
 
 ## License
 The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack Technologies or Salesforce.
+## [4.0.2] - 2023-06-14
+### Added
+- Added notification for an invalid cookie being passed (Fixes #47)
+### Fixed
+- JSON output for User and Workspace information was malformed, this has now been fixed
+
 ## [4.0.1] - 2023-05-05
 ### Changed
 - User output in stdout logging now includes display name and email. The accounts for cases where usernames are nonsensical.
 
 ## [4.0.0] - 2023-05-03
 This major version release brings multiple updates to Slack Watchman in usability, functionality and behind the scenes improvements.
```

### Comparing `slack-watchman-4.0.1/src/slack_watchman.egg-info/SOURCES.txt` & `slack-watchman-4.0.2/src/slack_watchman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

