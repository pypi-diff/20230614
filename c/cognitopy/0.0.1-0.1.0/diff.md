# Comparing `tmp/cognitopy-0.0.1.tar.gz` & `tmp/cognitopy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognitopy-0.0.1.tar", last modified: Tue Jun 13 18:10:09 2023, max compression
+gzip compressed data, was "cognitopy-0.1.0.tar", last modified: Wed Jun 14 16:16:57 2023, max compression
```

## Comparing `cognitopy-0.0.1.tar` & `cognitopy-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:10:09.373486 cognitopy-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-12 18:07:48.000000 cognitopy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5451 2023-06-13 18:10:09.372553 cognitopy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4902 2023-06-13 17:54:47.000000 cognitopy-0.0.1/README.md
--rw-rw-rw-   0        0        0      664 2023-06-12 18:18:48.000000 cognitopy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 18:10:09.373486 cognitopy-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 18:10:09.362445 cognitopy-0.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:59:33.000000 cognitopy-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:10:09.368450 cognitopy-0.0.1/src/cognitopy/
--rw-rw-rw-   0        0        0       48 2023-06-13 18:08:47.000000 cognitopy-0.0.1/src/cognitopy/__init__.py
--rw-rw-rw-   0        0        0    13005 2023-06-13 18:09:07.000000 cognitopy-0.0.1/src/cognitopy/cognitopy.py
--rw-rw-rw-   0        0        0      218 2023-06-08 14:21:49.000000 cognitopy-0.0.1/src/cognitopy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:10:09.371956 cognitopy-0.0.1/src/cognitopy.egg-info/
--rw-rw-rw-   0        0        0     5451 2023-06-13 18:10:09.000000 cognitopy-0.0.1/src/cognitopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-06-13 18:10:09.000000 cognitopy-0.0.1/src/cognitopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:10:09.000000 cognitopy-0.0.1/src/cognitopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-13 18:10:09.000000 cognitopy-0.0.1/src/cognitopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:16:57.619990 cognitopy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-14 16:16:43.000000 cognitopy-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-14 16:16:57.619990 cognitopy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-14 16:16:43.000000 cognitopy-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-14 16:16:43.000000 cognitopy-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:16:57.619990 cognitopy-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:16:57.619990 cognitopy-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:16:43.000000 cognitopy-0.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:16:57.619990 cognitopy-0.1.0/src/cognitopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 16:16:43.000000 cognitopy-0.1.0/src/cognitopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-06-14 16:16:43.000000 cognitopy-0.1.0/src/cognitopy/cognitopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-14 16:16:43.000000 cognitopy-0.1.0/src/cognitopy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:16:57.619990 cognitopy-0.1.0/src/cognitopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-14 16:16:57.000000 cognitopy-0.1.0/src/cognitopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-14 16:16:57.000000 cognitopy-0.1.0/src/cognitopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:16:57.000000 cognitopy-0.1.0/src/cognitopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 16:16:57.000000 cognitopy-0.1.0/src/cognitopy.egg-info/top_level.txt
```

### Comparing `cognitopy-0.0.1/LICENSE` & `cognitopy-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `cognitopy-0.0.1/PKG-INFO` & `cognitopy-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-Metadata-Version: 2.1
-Name: cognitopy
-Version: 0.0.1
-Summary: Python package to use aws cognito in a simple way
-Author-email: Daniel Muñoz Gonzalez <dani16595@gmail.com>
-Project-URL: Homepage, https://github.com/DaniMG95/cognitopy
-Project-URL: Bug Tracker, https://github.com/DaniMG95/cognitopy/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# cognitopy
-This is a package that will allow you to use the aws Cognito technology, so for now we are going to allow the management of users, authentication and creation of groups by Roles.  
-The potential of this package is the ease of management of all these functionalities and only creating an object with 3 parameters.
-
-## Installation
-```bash
-pip install cognitopy
-```
-
-## Variables for using the admin functions
-
-The cognito admin functions require that we have the aws, access key and secret access key credentials defined as system environment variables.
-
-```python
-import os
-
-os.environ["AWS_ACCESS_KEY_ID"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
-os.environ["AWS_SECRET_ACCESS_KEY"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
-```
-
-## Usage
-To define the cognitopy object it is necessary to give it the userpool_id, the client_id and the client_secret information.
-```python
-from cognitopy import CognitoPy
-
-COGNITO_USERPOOL_ID = 'XXX-XXX-XXXXXX'
-COGNITO_APP_CLIENT_ID = 'XXXXXXXXXXXXXXXXXXXXXXXX'
-COGNITO_APP_CLIENTE_SECRET = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
-
-cognito = CognitoPy(userpool_id=COGNITO_USERPOOL_ID, client_id=COGNITO_APP_CLIENT_ID, client_secret=COGNITO_APP_CLIENTE_SECRET)
-```
-
-Now I will explain the different functions that we can use in this version, with an example.  
-All these examples are in the directory example
-
-### Register a new user
-It will register a user in our cognito service and send us a confirmation message.
-```python
-cognitopy.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
-```
-
-### Confirm a new user
-It is responsible for confirming the user from the number received by mail.
-```python
-cognitopy.confirm_sing_up(username='XXXXX@mail.to', confirmation_code='820850')
-```
-
-### Resend confirm code
-It allows us to receive a confirmation code again, when we have previously requested to change password or register.
-```python
-cognitopy.resend_confirmation_code(username='XXXXX@mail.to')
-```
-
-### Login a user
-It will return the access token and refresh token of a confirmed user.
-```python
-tokens = cognitopy.login(username='XXXXX@mail.to', password='XXXXXXX')
-print(tokens['access_token'], tokens['refresh_token'])
-```
-
-### Refresh access token
-It will renew the user's access token
-```python
-access_token = cognitopy.renew_access_token(access_token='XXXXXXXXX', refresh_token='XXXXXXXXX')
-print(access_token)
-```
-
-### Check if access token is expired
-Check if the access token has expired
-```python
-is_expired = cognitopy.check_expired_token(access_token='XXXXXXXXX')
-print(is_expired)
-```
-
-### Forgot password
-Allows us to change our password by sending us a confirmation code.
-```python
-cognitopy.initiate_forgot_password(username='XXXXX@mail.to')
-```
-
-### Confirm forgot password
-Change the password of a user from the confirmation code received.
-```python
-cognitopy.confirm_forgot_password(username='XXXXX@mail.to', confirmation_code='YYYYY', password='XXXXXXX')
-```
-
-### Delete user
-Delete the user from his access token
-```python
-cognitopy.delete_user(access_token='XXXXXXXXX')
-```
-
-### Change password
-Change the password from your access token
-```python
-cognitopy.change_password(access_token='XXXXXXXXX', previous_password='XXXXXXX', proposed_password="XXXXXXX")
-```
-
-### Get user information
-We obtain basic user information from the user's access token.
-```python
-data_user = cognitopy.get_info_user_by_token(access_token='XXXXXXXXX')
-print(data_user['username'], data_user['groups'])
-```
-
-### Admin delete user
-We remove a user from our service from the administrator credentials
-```python
-cognitopy.admin_delete_user(username='XXXXX@mail.to')
-```
-
-### Admin create group
-We create a group from our service from the administrator credentials
-precedence: A non-negative integer value that specifies the precedence of this group relative to the other groups that a user can belong to in the user pool. Zero is the highest precedence value. Groups with lower Precedence values take precedence over groups with higher or null Precedence values.
-role_arn: The role Amazon Resource Name (ARN) for the group.
-```python
-cognitopy.admin_create_group(group_name='test_group', description='test group', precedence=1)
-```
-
-### Admin delete group
-We remove a group from our service from the administrator credentials
-```python
-cognitopy.admin_delete_group(group_name='test_group')
-```
-
-### Admin add user to group
-We add a user to group from our service from the administrator credentials
-```python
-cognitopy.admin_add_user_to_group(username='XXXXX@mail.to', group_name='test_group')
-```
-
-### Admin remove user from group
-We remove a user to group from our service from the administrator credentials
-```python
-cognitopy.admin_remove_user_from_group(username='XXXXX@mail.to', group_name='test_group')
-```
-
-
+Metadata-Version: 2.1
+Name: cognitopy
+Version: 0.1.0
+Summary: Python package to use aws cognito in a simple way
+Author-email: Daniel Muñoz Gonzalez <dani16595@gmail.com>
+Project-URL: Homepage, https://github.com/DaniMG95/cognitopy
+Project-URL: Bug Tracker, https://github.com/DaniMG95/cognitopy/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cognitopy
+This is a package that will allow you to use the aws Cognito technology, so for now we are going to allow the management of users, authentication and creation of groups by Roles.  
+The potential of this package is the ease of management of all these functionalities and only creating an object with 3 parameters.
+
+## Installation
+```bash
+pip install cognitopy
+```
+
+## Variables for using the admin functions
+
+The cognito admin functions require that we have the aws, access key and secret access key credentials defined as system environment variables.
+
+```python
+import os
+
+os.environ["AWS_ACCESS_KEY_ID"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
+os.environ["AWS_SECRET_ACCESS_KEY"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
+```
+
+## Usage
+To define the cognitopy object it is necessary to give it the userpool_id, the client_id and the client_secret information.
+```python
+from cognitopy import CognitoPy
+
+COGNITO_USERPOOL_ID = 'XXX-XXX-XXXXXX'
+COGNITO_APP_CLIENT_ID = 'XXXXXXXXXXXXXXXXXXXXXXXX'
+COGNITO_APP_CLIENTE_SECRET = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
+
+cognito = CognitoPy(userpool_id=COGNITO_USERPOOL_ID, client_id=COGNITO_APP_CLIENT_ID, client_secret=COGNITO_APP_CLIENTE_SECRET)
+```
+
+Now I will explain the different functions that we can use in this version, with an example.  
+All these examples are in the directory example
+
+### Register a new user
+It will register a user in our cognito service and send us a confirmation message.
+```python
+cognitopy.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+```
+
+### Confirm a new user
+It is responsible for confirming the user from the number received by mail.
+```python
+cognitopy.confirm_sing_up(username='XXXXX@mail.to', confirmation_code='820850')
+```
+
+### Resend confirm code
+It allows us to receive a confirmation code again, when we have previously requested to change password or register.
+```python
+cognitopy.resend_confirmation_code(username='XXXXX@mail.to')
+```
+
+### Login a user
+It will return the access token and refresh token of a confirmed user.
+```python
+tokens = cognitopy.login(username='XXXXX@mail.to', password='XXXXXXX')
+print(tokens['access_token'], tokens['refresh_token'])
+```
+
+### Refresh access token
+It will renew the user's access token
+```python
+access_token = cognitopy.renew_access_token(access_token='XXXXXXXXX', refresh_token='XXXXXXXXX')
+print(access_token)
+```
+
+### Check if access token is expired
+Check if the access token has expired
+```python
+is_expired = cognitopy.check_expired_token(access_token='XXXXXXXXX')
+print(is_expired)
+```
+
+### Forgot password
+Allows us to change our password by sending us a confirmation code.
+```python
+cognitopy.initiate_forgot_password(username='XXXXX@mail.to')
+```
+
+### Confirm forgot password
+Change the password of a user from the confirmation code received.
+```python
+cognitopy.confirm_forgot_password(username='XXXXX@mail.to', confirmation_code='YYYYY', password='XXXXXXX')
+```
+
+### Delete user
+Delete the user from his access token
+```python
+cognitopy.delete_user(access_token='XXXXXXXXX')
+```
+
+### Change password
+Change the password from your access token
+```python
+cognitopy.change_password(access_token='XXXXXXXXX', previous_password='XXXXXXX', proposed_password="XXXXXXX")
+```
+
+### Get user information
+We obtain basic user information from the user's access token.
+```python
+data_user = cognitopy.get_info_user_by_token(access_token='XXXXXXXXX')
+print(data_user['username'], data_user['groups'])
+```
+
+### Admin delete user
+We remove a user from our service from the administrator credentials
+```python
+cognitopy.admin_delete_user(username='XXXXX@mail.to')
+```
+
+### Admin create group
+We create a group from our service from the administrator credentials
+precedence: A non-negative integer value that specifies the precedence of this group relative to the other groups that a user can belong to in the user pool. Zero is the highest precedence value. Groups with lower Precedence values take precedence over groups with higher or null Precedence values.
+role_arn: The role Amazon Resource Name (ARN) for the group.
+```python
+cognitopy.admin_create_group(group_name='test_group', description='test group', precedence=1)
+```
+
+### Admin delete group
+We remove a group from our service from the administrator credentials
+```python
+cognitopy.admin_delete_group(group_name='test_group')
+```
+
+### Admin add user to group
+We add a user to group from our service from the administrator credentials
+```python
+cognitopy.admin_add_user_to_group(username='XXXXX@mail.to', group_name='test_group')
+```
+
+### Admin remove user from group
+We remove a user to group from our service from the administrator credentials
+```python
+cognitopy.admin_remove_user_from_group(username='XXXXX@mail.to', group_name='test_group')
+```
+
+
```

### Comparing `cognitopy-0.0.1/README.md` & `cognitopy-0.1.0/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-# cognitopy
-This is a package that will allow you to use the aws Cognito technology, so for now we are going to allow the management of users, authentication and creation of groups by Roles.  
-The potential of this package is the ease of management of all these functionalities and only creating an object with 3 parameters.
-
-## Installation
-```bash
-pip install cognitopy
-```
-
-## Variables for using the admin functions
-
-The cognito admin functions require that we have the aws, access key and secret access key credentials defined as system environment variables.
-
-```python
-import os
-
-os.environ["AWS_ACCESS_KEY_ID"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
-os.environ["AWS_SECRET_ACCESS_KEY"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
-```
-
-## Usage
-To define the cognitopy object it is necessary to give it the userpool_id, the client_id and the client_secret information.
-```python
-from cognitopy import CognitoPy
-
-COGNITO_USERPOOL_ID = 'XXX-XXX-XXXXXX'
-COGNITO_APP_CLIENT_ID = 'XXXXXXXXXXXXXXXXXXXXXXXX'
-COGNITO_APP_CLIENTE_SECRET = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
-
-cognito = CognitoPy(userpool_id=COGNITO_USERPOOL_ID, client_id=COGNITO_APP_CLIENT_ID, client_secret=COGNITO_APP_CLIENTE_SECRET)
-```
-
-Now I will explain the different functions that we can use in this version, with an example.  
-All these examples are in the directory example
-
-### Register a new user
-It will register a user in our cognito service and send us a confirmation message.
-```python
-cognitopy.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
-```
-
-### Confirm a new user
-It is responsible for confirming the user from the number received by mail.
-```python
-cognitopy.confirm_sing_up(username='XXXXX@mail.to', confirmation_code='820850')
-```
-
-### Resend confirm code
-It allows us to receive a confirmation code again, when we have previously requested to change password or register.
-```python
-cognitopy.resend_confirmation_code(username='XXXXX@mail.to')
-```
-
-### Login a user
-It will return the access token and refresh token of a confirmed user.
-```python
-tokens = cognitopy.login(username='XXXXX@mail.to', password='XXXXXXX')
-print(tokens['access_token'], tokens['refresh_token'])
-```
-
-### Refresh access token
-It will renew the user's access token
-```python
-access_token = cognitopy.renew_access_token(access_token='XXXXXXXXX', refresh_token='XXXXXXXXX')
-print(access_token)
-```
-
-### Check if access token is expired
-Check if the access token has expired
-```python
-is_expired = cognitopy.check_expired_token(access_token='XXXXXXXXX')
-print(is_expired)
-```
-
-### Forgot password
-Allows us to change our password by sending us a confirmation code.
-```python
-cognitopy.initiate_forgot_password(username='XXXXX@mail.to')
-```
-
-### Confirm forgot password
-Change the password of a user from the confirmation code received.
-```python
-cognitopy.confirm_forgot_password(username='XXXXX@mail.to', confirmation_code='YYYYY', password='XXXXXXX')
-```
-
-### Delete user
-Delete the user from his access token
-```python
-cognitopy.delete_user(access_token='XXXXXXXXX')
-```
-
-### Change password
-Change the password from your access token
-```python
-cognitopy.change_password(access_token='XXXXXXXXX', previous_password='XXXXXXX', proposed_password="XXXXXXX")
-```
-
-### Get user information
-We obtain basic user information from the user's access token.
-```python
-data_user = cognitopy.get_info_user_by_token(access_token='XXXXXXXXX')
-print(data_user['username'], data_user['groups'])
-```
-
-### Admin delete user
-We remove a user from our service from the administrator credentials
-```python
-cognitopy.admin_delete_user(username='XXXXX@mail.to')
-```
-
-### Admin create group
-We create a group from our service from the administrator credentials
-precedence: A non-negative integer value that specifies the precedence of this group relative to the other groups that a user can belong to in the user pool. Zero is the highest precedence value. Groups with lower Precedence values take precedence over groups with higher or null Precedence values.
-role_arn: The role Amazon Resource Name (ARN) for the group.
-```python
-cognitopy.admin_create_group(group_name='test_group', description='test group', precedence=1)
-```
-
-### Admin delete group
-We remove a group from our service from the administrator credentials
-```python
-cognitopy.admin_delete_group(group_name='test_group')
-```
-
-### Admin add user to group
-We add a user to group from our service from the administrator credentials
-```python
-cognitopy.admin_add_user_to_group(username='XXXXX@mail.to', group_name='test_group')
-```
-
-### Admin remove user from group
-We remove a user to group from our service from the administrator credentials
-```python
-cognitopy.admin_remove_user_from_group(username='XXXXX@mail.to', group_name='test_group')
-```
-
-
+# cognitopy
+This is a package that will allow you to use the aws Cognito technology, so for now we are going to allow the management of users, authentication and creation of groups by Roles.  
+The potential of this package is the ease of management of all these functionalities and only creating an object with 3 parameters.
+
+## Installation
+```bash
+pip install cognitopy
+```
+
+## Variables for using the admin functions
+
+The cognito admin functions require that we have the aws, access key and secret access key credentials defined as system environment variables.
+
+```python
+import os
+
+os.environ["AWS_ACCESS_KEY_ID"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
+os.environ["AWS_SECRET_ACCESS_KEY"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
+```
+
+## Usage
+To define the cognitopy object it is necessary to give it the userpool_id, the client_id and the client_secret information.
+```python
+from cognitopy import CognitoPy
+
+COGNITO_USERPOOL_ID = 'XXX-XXX-XXXXXX'
+COGNITO_APP_CLIENT_ID = 'XXXXXXXXXXXXXXXXXXXXXXXX'
+COGNITO_APP_CLIENTE_SECRET = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
+
+cognito = CognitoPy(userpool_id=COGNITO_USERPOOL_ID, client_id=COGNITO_APP_CLIENT_ID, client_secret=COGNITO_APP_CLIENTE_SECRET)
+```
+
+Now I will explain the different functions that we can use in this version, with an example.  
+All these examples are in the directory example
+
+### Register a new user
+It will register a user in our cognito service and send us a confirmation message.
+```python
+cognitopy.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+```
+
+### Confirm a new user
+It is responsible for confirming the user from the number received by mail.
+```python
+cognitopy.confirm_sing_up(username='XXXXX@mail.to', confirmation_code='820850')
+```
+
+### Resend confirm code
+It allows us to receive a confirmation code again, when we have previously requested to change password or register.
+```python
+cognitopy.resend_confirmation_code(username='XXXXX@mail.to')
+```
+
+### Login a user
+It will return the access token and refresh token of a confirmed user.
+```python
+tokens = cognitopy.login(username='XXXXX@mail.to', password='XXXXXXX')
+print(tokens['access_token'], tokens['refresh_token'])
+```
+
+### Refresh access token
+It will renew the user's access token
+```python
+access_token = cognitopy.renew_access_token(access_token='XXXXXXXXX', refresh_token='XXXXXXXXX')
+print(access_token)
+```
+
+### Check if access token is expired
+Check if the access token has expired
+```python
+is_expired = cognitopy.check_expired_token(access_token='XXXXXXXXX')
+print(is_expired)
+```
+
+### Forgot password
+Allows us to change our password by sending us a confirmation code.
+```python
+cognitopy.initiate_forgot_password(username='XXXXX@mail.to')
+```
+
+### Confirm forgot password
+Change the password of a user from the confirmation code received.
+```python
+cognitopy.confirm_forgot_password(username='XXXXX@mail.to', confirmation_code='YYYYY', password='XXXXXXX')
+```
+
+### Delete user
+Delete the user from his access token
+```python
+cognitopy.delete_user(access_token='XXXXXXXXX')
+```
+
+### Change password
+Change the password from your access token
+```python
+cognitopy.change_password(access_token='XXXXXXXXX', previous_password='XXXXXXX', proposed_password="XXXXXXX")
+```
+
+### Get user information
+We obtain basic user information from the user's access token.
+```python
+data_user = cognitopy.get_info_user_by_token(access_token='XXXXXXXXX')
+print(data_user['username'], data_user['groups'])
+```
+
+### Admin delete user
+We remove a user from our service from the administrator credentials
+```python
+cognitopy.admin_delete_user(username='XXXXX@mail.to')
+```
+
+### Admin create group
+We create a group from our service from the administrator credentials
+precedence: A non-negative integer value that specifies the precedence of this group relative to the other groups that a user can belong to in the user pool. Zero is the highest precedence value. Groups with lower Precedence values take precedence over groups with higher or null Precedence values.
+role_arn: The role Amazon Resource Name (ARN) for the group.
+```python
+cognitopy.admin_create_group(group_name='test_group', description='test group', precedence=1)
+```
+
+### Admin delete group
+We remove a group from our service from the administrator credentials
+```python
+cognitopy.admin_delete_group(group_name='test_group')
+```
+
+### Admin add user to group
+We add a user to group from our service from the administrator credentials
+```python
+cognitopy.admin_add_user_to_group(username='XXXXX@mail.to', group_name='test_group')
+```
+
+### Admin remove user from group
+We remove a user to group from our service from the administrator credentials
+```python
+cognitopy.admin_remove_user_from_group(username='XXXXX@mail.to', group_name='test_group')
+```
+
+
```

### Comparing `cognitopy-0.0.1/src/cognitopy.egg-info/PKG-INFO` & `cognitopy-0.1.0/src/cognitopy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-Metadata-Version: 2.1
-Name: cognitopy
-Version: 0.0.1
-Summary: Python package to use aws cognito in a simple way
-Author-email: Daniel Muñoz Gonzalez <dani16595@gmail.com>
-Project-URL: Homepage, https://github.com/DaniMG95/cognitopy
-Project-URL: Bug Tracker, https://github.com/DaniMG95/cognitopy/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# cognitopy
-This is a package that will allow you to use the aws Cognito technology, so for now we are going to allow the management of users, authentication and creation of groups by Roles.  
-The potential of this package is the ease of management of all these functionalities and only creating an object with 3 parameters.
-
-## Installation
-```bash
-pip install cognitopy
-```
-
-## Variables for using the admin functions
-
-The cognito admin functions require that we have the aws, access key and secret access key credentials defined as system environment variables.
-
-```python
-import os
-
-os.environ["AWS_ACCESS_KEY_ID"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
-os.environ["AWS_SECRET_ACCESS_KEY"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
-```
-
-## Usage
-To define the cognitopy object it is necessary to give it the userpool_id, the client_id and the client_secret information.
-```python
-from cognitopy import CognitoPy
-
-COGNITO_USERPOOL_ID = 'XXX-XXX-XXXXXX'
-COGNITO_APP_CLIENT_ID = 'XXXXXXXXXXXXXXXXXXXXXXXX'
-COGNITO_APP_CLIENTE_SECRET = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
-
-cognito = CognitoPy(userpool_id=COGNITO_USERPOOL_ID, client_id=COGNITO_APP_CLIENT_ID, client_secret=COGNITO_APP_CLIENTE_SECRET)
-```
-
-Now I will explain the different functions that we can use in this version, with an example.  
-All these examples are in the directory example
-
-### Register a new user
-It will register a user in our cognito service and send us a confirmation message.
-```python
-cognitopy.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
-```
-
-### Confirm a new user
-It is responsible for confirming the user from the number received by mail.
-```python
-cognitopy.confirm_sing_up(username='XXXXX@mail.to', confirmation_code='820850')
-```
-
-### Resend confirm code
-It allows us to receive a confirmation code again, when we have previously requested to change password or register.
-```python
-cognitopy.resend_confirmation_code(username='XXXXX@mail.to')
-```
-
-### Login a user
-It will return the access token and refresh token of a confirmed user.
-```python
-tokens = cognitopy.login(username='XXXXX@mail.to', password='XXXXXXX')
-print(tokens['access_token'], tokens['refresh_token'])
-```
-
-### Refresh access token
-It will renew the user's access token
-```python
-access_token = cognitopy.renew_access_token(access_token='XXXXXXXXX', refresh_token='XXXXXXXXX')
-print(access_token)
-```
-
-### Check if access token is expired
-Check if the access token has expired
-```python
-is_expired = cognitopy.check_expired_token(access_token='XXXXXXXXX')
-print(is_expired)
-```
-
-### Forgot password
-Allows us to change our password by sending us a confirmation code.
-```python
-cognitopy.initiate_forgot_password(username='XXXXX@mail.to')
-```
-
-### Confirm forgot password
-Change the password of a user from the confirmation code received.
-```python
-cognitopy.confirm_forgot_password(username='XXXXX@mail.to', confirmation_code='YYYYY', password='XXXXXXX')
-```
-
-### Delete user
-Delete the user from his access token
-```python
-cognitopy.delete_user(access_token='XXXXXXXXX')
-```
-
-### Change password
-Change the password from your access token
-```python
-cognitopy.change_password(access_token='XXXXXXXXX', previous_password='XXXXXXX', proposed_password="XXXXXXX")
-```
-
-### Get user information
-We obtain basic user information from the user's access token.
-```python
-data_user = cognitopy.get_info_user_by_token(access_token='XXXXXXXXX')
-print(data_user['username'], data_user['groups'])
-```
-
-### Admin delete user
-We remove a user from our service from the administrator credentials
-```python
-cognitopy.admin_delete_user(username='XXXXX@mail.to')
-```
-
-### Admin create group
-We create a group from our service from the administrator credentials
-precedence: A non-negative integer value that specifies the precedence of this group relative to the other groups that a user can belong to in the user pool. Zero is the highest precedence value. Groups with lower Precedence values take precedence over groups with higher or null Precedence values.
-role_arn: The role Amazon Resource Name (ARN) for the group.
-```python
-cognitopy.admin_create_group(group_name='test_group', description='test group', precedence=1)
-```
-
-### Admin delete group
-We remove a group from our service from the administrator credentials
-```python
-cognitopy.admin_delete_group(group_name='test_group')
-```
-
-### Admin add user to group
-We add a user to group from our service from the administrator credentials
-```python
-cognitopy.admin_add_user_to_group(username='XXXXX@mail.to', group_name='test_group')
-```
-
-### Admin remove user from group
-We remove a user to group from our service from the administrator credentials
-```python
-cognitopy.admin_remove_user_from_group(username='XXXXX@mail.to', group_name='test_group')
-```
-
-
+Metadata-Version: 2.1
+Name: cognitopy
+Version: 0.1.0
+Summary: Python package to use aws cognito in a simple way
+Author-email: Daniel Muñoz Gonzalez <dani16595@gmail.com>
+Project-URL: Homepage, https://github.com/DaniMG95/cognitopy
+Project-URL: Bug Tracker, https://github.com/DaniMG95/cognitopy/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cognitopy
+This is a package that will allow you to use the aws Cognito technology, so for now we are going to allow the management of users, authentication and creation of groups by Roles.  
+The potential of this package is the ease of management of all these functionalities and only creating an object with 3 parameters.
+
+## Installation
+```bash
+pip install cognitopy
+```
+
+## Variables for using the admin functions
+
+The cognito admin functions require that we have the aws, access key and secret access key credentials defined as system environment variables.
+
+```python
+import os
+
+os.environ["AWS_ACCESS_KEY_ID"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
+os.environ["AWS_SECRET_ACCESS_KEY"] = 'XXXXXXXXXXXXXXXXXXXXXXXX'
+```
+
+## Usage
+To define the cognitopy object it is necessary to give it the userpool_id, the client_id and the client_secret information.
+```python
+from cognitopy import CognitoPy
+
+COGNITO_USERPOOL_ID = 'XXX-XXX-XXXXXX'
+COGNITO_APP_CLIENT_ID = 'XXXXXXXXXXXXXXXXXXXXXXXX'
+COGNITO_APP_CLIENTE_SECRET = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
+
+cognito = CognitoPy(userpool_id=COGNITO_USERPOOL_ID, client_id=COGNITO_APP_CLIENT_ID, client_secret=COGNITO_APP_CLIENTE_SECRET)
+```
+
+Now I will explain the different functions that we can use in this version, with an example.  
+All these examples are in the directory example
+
+### Register a new user
+It will register a user in our cognito service and send us a confirmation message.
+```python
+cognitopy.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+```
+
+### Confirm a new user
+It is responsible for confirming the user from the number received by mail.
+```python
+cognitopy.confirm_sing_up(username='XXXXX@mail.to', confirmation_code='820850')
+```
+
+### Resend confirm code
+It allows us to receive a confirmation code again, when we have previously requested to change password or register.
+```python
+cognitopy.resend_confirmation_code(username='XXXXX@mail.to')
+```
+
+### Login a user
+It will return the access token and refresh token of a confirmed user.
+```python
+tokens = cognitopy.login(username='XXXXX@mail.to', password='XXXXXXX')
+print(tokens['access_token'], tokens['refresh_token'])
+```
+
+### Refresh access token
+It will renew the user's access token
+```python
+access_token = cognitopy.renew_access_token(access_token='XXXXXXXXX', refresh_token='XXXXXXXXX')
+print(access_token)
+```
+
+### Check if access token is expired
+Check if the access token has expired
+```python
+is_expired = cognitopy.check_expired_token(access_token='XXXXXXXXX')
+print(is_expired)
+```
+
+### Forgot password
+Allows us to change our password by sending us a confirmation code.
+```python
+cognitopy.initiate_forgot_password(username='XXXXX@mail.to')
+```
+
+### Confirm forgot password
+Change the password of a user from the confirmation code received.
+```python
+cognitopy.confirm_forgot_password(username='XXXXX@mail.to', confirmation_code='YYYYY', password='XXXXXXX')
+```
+
+### Delete user
+Delete the user from his access token
+```python
+cognitopy.delete_user(access_token='XXXXXXXXX')
+```
+
+### Change password
+Change the password from your access token
+```python
+cognitopy.change_password(access_token='XXXXXXXXX', previous_password='XXXXXXX', proposed_password="XXXXXXX")
+```
+
+### Get user information
+We obtain basic user information from the user's access token.
+```python
+data_user = cognitopy.get_info_user_by_token(access_token='XXXXXXXXX')
+print(data_user['username'], data_user['groups'])
+```
+
+### Admin delete user
+We remove a user from our service from the administrator credentials
+```python
+cognitopy.admin_delete_user(username='XXXXX@mail.to')
+```
+
+### Admin create group
+We create a group from our service from the administrator credentials
+precedence: A non-negative integer value that specifies the precedence of this group relative to the other groups that a user can belong to in the user pool. Zero is the highest precedence value. Groups with lower Precedence values take precedence over groups with higher or null Precedence values.
+role_arn: The role Amazon Resource Name (ARN) for the group.
+```python
+cognitopy.admin_create_group(group_name='test_group', description='test group', precedence=1)
+```
+
+### Admin delete group
+We remove a group from our service from the administrator credentials
+```python
+cognitopy.admin_delete_group(group_name='test_group')
+```
+
+### Admin add user to group
+We add a user to group from our service from the administrator credentials
+```python
+cognitopy.admin_add_user_to_group(username='XXXXX@mail.to', group_name='test_group')
+```
+
+### Admin remove user from group
+We remove a user to group from our service from the administrator credentials
+```python
+cognitopy.admin_remove_user_from_group(username='XXXXX@mail.to', group_name='test_group')
+```
+
+
```

