# Comparing `tmp/jirarelease-1.2.1.tar.gz` & `tmp/jirarelease-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jirarelease-1.2.1.tar", last modified: Tue Jan 31 08:57:18 2023, max compression
+gzip compressed data, was "jirarelease-1.2.2.tar", last modified: Wed Jun 14 09:09:55 2023, max compression
```

## Comparing `jirarelease-1.2.1.tar` & `jirarelease-1.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1799 2023-01-29 08:42:42.706166 jirarelease-1.2.1/.gitignore
--rw-r--r--   0        0        0     1064 2023-01-29 08:42:42.706166 jirarelease-1.2.1/LICENSE
--rw-r--r--   0        0        0       56 2023-01-29 08:42:42.706166 jirarelease-1.2.1/README.md
--rw-r--r--   0        0        0     4324 2023-01-31 08:56:35.942624 jirarelease-1.2.1/jirarelease/__init__.py
--rw-r--r--   0        0        0      442 2023-01-30 14:58:49.192143 jirarelease-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 jirarelease-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-01-29 08:42:42.706166 jirarelease-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1064 2023-01-29 08:42:42.706166 jirarelease-1.2.2/LICENSE
+-rw-r--r--   0        0        0       56 2023-01-29 08:42:42.706166 jirarelease-1.2.2/README.md
+-rw-r--r--   0        0        0     4978 2023-06-14 09:07:07.392902 jirarelease-1.2.2/jirarelease/__init__.py
+-rw-r--r--   0        0        0      442 2023-01-30 14:58:49.192143 jirarelease-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 jirarelease-1.2.2/PKG-INFO
```

### Comparing `jirarelease-1.2.1/.gitignore` & `jirarelease-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jirarelease-1.2.1/LICENSE` & `jirarelease-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jirarelease-1.2.1/jirarelease/__init__.py` & `jirarelease-1.2.2/jirarelease/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 This is a example for jira release
 """
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 import os
 from datetime import datetime, timezone, timedelta
 import pkg_resources
 from jira import JIRA
 import re
+from loguru import logger
 
 
 class DailyReleaseModel:
     
     date_format = '%Y.%m.%d'
     
     @staticmethod
@@ -29,31 +30,37 @@
                 _versions.append(match.group())
         return _versions
     
     def __init__(self, vers: list, base_version: str, eod_hour: int, label: str)-> dict:
         version = {}
         today_date = datetime.now(timezone(offset=timedelta(hours=eod_hour))).strftime(self.date_format)
         matched_version = [v for v in vers if self.match_version(v, label)]
-        
+
+        logger.info("Getting matched versions:")
+        logger.info(matched_version)
         if matched_version:
             for v in matched_version:
                 arr = v.split('-')
                 version.setdefault(arr[0], set())
                 version[arr[0]].add(arr[1])
                 
             latest_ver = max(version.keys(), key=pkg_resources.parse_version)
             latest_date = max(self.to_date(version[latest_ver]), key=lambda d: datetime.strptime(d, self.date_format))
-            print("matched versions:", version) 
         else:
             latest_ver = base_version
             latest_date = today_date
         
         self.today_ver = f"{latest_ver}-{label}.{today_date}"
+        logger.info("today version: " + self.today_ver)
+
         self.latest_ver = f"{latest_ver}-{label}.{latest_date}"
+        logger.info("latest version: " +self.latest_ver)
+        
         self.today_date = today_date
+        logger.info("today date: " +self.today_date)
     
     def daily_version(self)-> str:
         return self.today_ver
     
     def semantic_version(self):
         return self.daily_version().split('-')[0]
     
@@ -92,25 +99,35 @@
         
     def include_issue(self, jira_issue: str, release_previous=True, label='rc'):
         issue = self.jira.issue(jira_issue)
         project = jira_issue.split('-')[0]
         
         versions = self.jira.project_versions(project)
         version_names = [v.name for v in versions]
-        
+        logger.info("all assigned version: ")
+        logger.info(version_names)
+
         model = DailyReleaseModel(
             vers=version_names, 
             base_version=self.base_version, 
             eod_hour=self.eod_hour,
             label=label
         )
         
-        assignable_versions = self._create_versions(project, model, versions)
+        assignable_versions = set(self._create_versions(project, model, versions))
+        existing_versions = set(issue.get_field("fixVersions"))
+        existing_versions = existing_versions - assignable_versions
+        
+        assignable_versions = list(assignable_versions)
+        assignable_versions.extend(list(existing_versions))
+        logger.info(assignable_versions)
         
         fix_vers = [{'id': v.id} for v in assignable_versions]
-        print("Updating issue:", issue.key ,"to version: ", fix_vers)
+        logger.info("Updating issue: " + issue.key + " to versions: ")
+        logger.info(fix_vers)
+        
         issue.update(fields={'fixVersions': fix_vers})
             
         if release_previous and model.has_unreleased_version():
             latest_version = [v for v in versions if v.name == model.latest_ver][0]
-            print("Releasing previous version: ", latest_version.name)
+            logger.info("Releasing previous version: " + latest_version.name)
             latest_version.update(released=True)
```

