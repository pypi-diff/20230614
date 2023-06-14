# Comparing `tmp/remindmail-2023.6.4.2.tar.gz` & `tmp/remindmail-2023.6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2023.6.4.2.tar", last modified: Mon Jun  5 04:57:41 2023, max compression
+gzip compressed data, was "remindmail-2023.6.8.1.tar", last modified: Thu Jun  8 06:31:47 2023, max compression
```

## Comparing `remindmail-2023.6.4.2.tar` & `remindmail-2023.6.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-05 04:57:41.224496 remindmail-2023.6.4.2/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.6.4.2/LICENSE.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    13624 2023-06-05 04:57:41.224496 remindmail-2023.6.4.2/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    13275 2023-06-05 04:37:46.000000 remindmail-2023.6.4.2/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.6.4.2/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-06-05 04:57:41.224496 remindmail-2023.6.4.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-05 04:57:41.220496 remindmail-2023.6.4.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-05 04:57:41.220496 remindmail-2023.6.4.2/src/remind/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.6.4.2/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4199 2023-06-05 04:48:55.000000 remindmail-2023.6.4.2/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.6.4.2/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    25417 2023-06-05 04:52:55.000000 remindmail-2023.6.4.2/src/remind/remindmail.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11658 2023-06-05 04:56:51.000000 remindmail-2023.6.4.2/src/remind/remindmail_utils.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-05 04:57:41.224496 remindmail-2023.6.4.2/src/remindmail.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    13624 2023-06-05 04:57:41.000000 remindmail-2023.6.4.2/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-06-05 04:57:41.000000 remindmail-2023.6.4.2/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-05 04:57:41.000000 remindmail-2023.6.4.2/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-06-05 04:57:41.000000 remindmail-2023.6.4.2/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-06-05 04:57:41.000000 remindmail-2023.6.4.2/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.6.8.1/LICENSE.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    13861 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    13512 2023-06-08 06:27:14.000000 remindmail-2023.6.8.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.6.8.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-08 06:31:47.033063 remindmail-2023.6.8.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/src/remind/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.6.8.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     4611 2023-06-08 06:31:13.000000 remindmail-2023.6.8.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.6.8.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    25417 2023-06-05 04:59:42.000000 remindmail-2023.6.8.1/src/remind/remindmail.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    12809 2023-06-08 06:30:34.000000 remindmail-2023.6.8.1/src/remind/remindmail_utils.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/src/remindmail.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    13861 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2023.6.4.2/LICENSE.md` & `remindmail-2023.6.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.6.4.2/PKG-INFO` & `remindmail-2023.6.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: remindmail
-Version: 2023.6.4.2
-Summary: Easily schedule reminders to be emailed
-Home-page: https://github.com/tylerjwoodfin/remindmail
-Author: Tyler Woodfin
-Author-email: feedback@tyler.cloud
-License: : OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # remindmail
 
 - turns reminders written in terminal into emails; supports scheduled reminders
 
 ## features
 
 - easily manage your To Do list from anywhere in the terminal
@@ -321,13 +309,18 @@
 ```
 
 Make sure to replace values in brackets with your own values.
 
 ## Usage
 
 ```
-# creates a ticket directly with no confirmation
+# creates a ticket (with prompts for description, label, issue type)
 remind -m this is a new ticket --jira
 
+# creates a ticket without prompts
+remind --jira "this is a story 4" -t task --desc "Testing description" --label "testing"
+
 # select '(j)' in confirmation menu
 remind -m this is a new jira ticket
 ```
+
+After the issue has been created, a success message and link to the new issue will appear.
```

### Comparing `remindmail-2023.6.4.2/README.md` & `remindmail-2023.6.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: remindmail
+Version: 2023.6.8.1
+Summary: Easily schedule reminders to be emailed
+Home-page: https://github.com/tylerjwoodfin/remindmail
+Author: Tyler Woodfin
+Author-email: feedback@tyler.cloud
+License: : OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # remindmail
 
 - turns reminders written in terminal into emails; supports scheduled reminders
 
 ## features
 
 - easily manage your To Do list from anywhere in the terminal
@@ -309,13 +321,18 @@
 ```
 
 Make sure to replace values in brackets with your own values.
 
 ## Usage
 
 ```
-# creates a ticket directly with no confirmation
+# creates a ticket (with prompts for description, label, issue type)
 remind -m this is a new ticket --jira
 
+# creates a ticket without prompts
+remind --jira "this is a story 4" -t task --desc "Testing description" --label "testing"
+
 # select '(j)' in confirmation menu
 remind -m this is a new jira ticket
-```
+```
+
+After the issue has been created, a success message and link to the new issue will appear.
```

### Comparing `remindmail-2023.6.4.2/setup.cfg` & `remindmail-2023.6.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = remindmail
-version = 2023.06.04.2
+version = 2023.06.08.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls =
```

### Comparing `remindmail-2023.6.4.2/src/remind/__main__.py` & `remindmail-2023.6.8.1/src/remind/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,20 @@
     parser.add_argument('--show-tomorrow', action='store_true',
                         help='Shows a list of reminders scheduled for tomorrow')
     parser.add_argument('--sent-today', action='store_true',
                         help='Prints the sum of reminders sent today (yesterday, if before 4AM)')
     parser.add_argument('manual_reminder_args', nargs='*')
     parser.add_argument('-j', '--jira', action='store_true',
                         help='Creates an issue through Jira rather than using email.')
+    parser.add_argument('-t', '--type', nargs='?', const='task',
+                        help='Specify the issue type ("story", "task", "bug", "spike", "epic")')
+    parser.add_argument('--desc', '--description', nargs='?',
+                        help='Jira issue description')
+    parser.add_argument('--label', nargs='?',
+                        help='Jira label')
 
     args = parser.parse_args()
 
     if args.list:
         RemindMailUtils().print_reminders_file()
     elif args.generate:
         RemindMail().generate(force=args.force, dry_run=args.dry_run)
@@ -75,15 +81,16 @@
         RemindMailUtils().edit_reminders_file()
     elif args.show_tomorrow:
         RemindMail().show_tomorrow()
     elif args.sent_today:
         print(RemindMailUtils().get_sent_today())
     elif args.jira:
         RemindMailUtils().create_jira_issue(
-            args.message or ' '.join(args.manual_reminder_args), args.notes or '')
+            args.message or ' '.join(args.manual_reminder_args),
+            args.desc or None, args.type or None, args.label)
     elif args.manual_reminder_args:
         RemindMail().parse_query(query=' '.join(args.manual_reminder_args),
                                  noconfirm=args.noconfirm)
     else:
         RemindMail().manual_reminder(manual_message=args.message or '',
                                      manual_date=args.date or '', noconfirm=args.noconfirm)
```

### Comparing `remindmail-2023.6.4.2/src/remind/reminder.py` & `remindmail-2023.6.8.1/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.6.4.2/src/remind/remindmail.py` & `remindmail-2023.6.8.1/src/remind/remindmail.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.6.4.2/src/remind/remindmail_utils.py` & `remindmail-2023.6.8.1/src/remind/remindmail_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -244,48 +244,45 @@
 
         body += f"<br><br>Sent via {method}"
 
         RemindMailUtils.mail.send(
             f"Reminder - {subject}", body or "", is_quiet=is_quiet)
         print("\nSent! Check your inbox.")
 
-    def create_jira_issue(self, summary, description):
+    def create_jira_issue(self, summary, description, issue_type: str = None, label=None):
         """
         A barebones integration with Jira.
 
         Requires Cabinet to be configured as described in README.
 
         Parameters:
             summary(str): issue title
             description(str): issue description
+            issue_type(str): issue type ("story", "task", "bug", "spike", "epic")
+            label(str): label
         """
 
         api_url_base = self.cab.get('jira', 'project-url')
 
         if api_url_base is None:
-            self.cab.log(
-                "RemindMail - Cannot create Jira issue; cabinet -> jira -> project-url is unset",
-                level="warn")
+            self.cab.log("RemindMail - Cannot create Jira issue; cabinet",
+                         "-> jira -> project-url is unset",
+                         level="warn")
             return
+
         api_url = f"{str(api_url_base).rstrip('/')}/rest/api/2/issue"
 
         # Set your Jira credentials
         jira_email = self.cab.get("jira", "email")
         jira_api_token = self.cab.get("keys", "jira")
 
-        # Set the project key and issue details
-        project_key = self.cab.get("jira", "project-key")
-        issue_type = 'Task'
-
         if not jira_api_token or not jira_email:
-            self.cab.log(
-                "RemindMail - cannot create Jira issue; cabinet is missing "
-                "`keys -> jira` or `jira -> email` (see README)",
-                level="warn"
-            )
+            self.cab.log("RemindMail - cannot create Jira issue; cabinet is missing "
+                         "`keys -> jira` or `jira -> email` (see README)",
+                         level="warn")
             return
 
         if not summary:
             self.cab.log("RemindMail - cannot create Jira issue; summary cannot be blank",
                          level="warn")
             return
 
@@ -297,29 +294,53 @@
             'Content-Type': 'application/json',
             'Authorization': f'Basic {encoded_credentials}'
         }
 
         # Create the issue payload
         payload = {
             'fields': {
-                'project': {'key': project_key},
-                'summary': summary,
-                'description': f"Added via RemindMail\n\n{description}",
-                'issuetype': {'name': issue_type}
+                'project': {'key': self.cab.get("jira", "project-key")},
+                'summary': f"RMMJ: {summary}",
+                'issuetype': {'name': issue_type.capitalize() if issue_type else ''},
+                'labels': [label] if label else None,
             }
         }
 
+        # Prompt for missing fields
+        if not issue_type:
+            issue_type_input = input('Please enter an issue type:\n'
+                                     'story\nbug\ntask\nspike\nepic\n\n').capitalize()
+            payload['fields']['issuetype']['name'] = issue_type_input
+
+        if description is None:
+            description_input = input(
+                '\nPlease enter a description (or Enter for none)\n')
+            payload['fields']['description'] = description_input
+        else:
+            payload['fields']['description'] = description
+
+        issue_type_lower = payload['fields']['issuetype']['name'].lower()
+        if issue_type_lower in ['story', 'bug']:
+            if issue_type_lower == 'story':
+                a_c = input('\nPlease enter an AC:\n')
+                payload['fields']['customfield_10035'] = a_c
+
+        if label is None:
+            label_input = input('\nPlease enter a Label:\n')
+            payload['fields']['labels'] = [label_input]
+
         # Send the POST request to create the issue
-        response = requests.post(
-            api_url, headers=headers, json=payload, timeout=10)
+        response = requests.post(api_url, headers=headers,
+                                 json=payload, timeout=10)
 
         # Check the response
         if response.status_code == 201:
             created_issue = response.json()
-            print(f'{created_issue["key"]} created successfully.')
-            self.cab.log(
-                f"Created Jira issue {created_issue['key']}", is_quiet=True)
+            issue_key = created_issue['key']
+            print(f"{issue_key} has been created.")
+            print(f"{api_url_base}/browse/{issue_key}")
+            self.cab.log(f"\n{issue_key} has been created.", is_quiet=True)
         else:
             print('Failed to create the issue.')
             print(f'Response: {response.text}')
             self.cab.log(
                 f"RemindMail unable to create Jira issue: {response}", level="warn")
```

### Comparing `remindmail-2023.6.4.2/src/remindmail.egg-info/PKG-INFO` & `remindmail-2023.6.8.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.6.4.2
+Version: 2023.6.8.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -321,13 +321,18 @@
 ```
 
 Make sure to replace values in brackets with your own values.
 
 ## Usage
 
 ```
-# creates a ticket directly with no confirmation
+# creates a ticket (with prompts for description, label, issue type)
 remind -m this is a new ticket --jira
 
+# creates a ticket without prompts
+remind --jira "this is a story 4" -t task --desc "Testing description" --label "testing"
+
 # select '(j)' in confirmation menu
 remind -m this is a new jira ticket
 ```
+
+After the issue has been created, a success message and link to the new issue will appear.
```

