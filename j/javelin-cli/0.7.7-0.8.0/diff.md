# Comparing `tmp/javelin-cli-0.7.7.tar.gz` & `tmp/javelin-cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "javelin-cli-0.7.7.tar", max compression
+gzip compressed data, was "javelin-cli-0.8.0.tar", max compression
```

## Comparing `javelin-cli-0.7.7.tar` & `javelin-cli-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      589 2022-08-08 06:57:49.070529 javelin-cli-0.7.7/README.md
--rw-r--r--   0        0        0       22 2022-08-17 04:05:49.770434 javelin-cli-0.7.7/javelin/__init__.py
--rw-r--r--   0        0        0     6043 2022-08-08 06:42:22.893531 javelin-cli-0.7.7/javelin/__main__.py
--rw-r--r--   0        0        0        0 2022-06-20 23:44:18.476590 javelin-cli-0.7.7/javelin/utils/__init__.py
--rw-r--r--   0        0        0     1716 2022-07-15 05:36:25.525384 javelin-cli-0.7.7/javelin/utils/aws.py
--rw-r--r--   0        0        0     4550 2022-08-08 06:42:21.726821 javelin-cli-0.7.7/javelin/utils/github.py
--rw-r--r--   0        0        0     4428 2022-08-17 04:04:53.626078 javelin-cli-0.7.7/javelin/utils/slack.py
--rw-r--r--   0        0        0      633 2022-08-17 04:05:46.981930 javelin-cli-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     1460 2022-08-17 04:07:59.985734 javelin-cli-0.7.7/setup.py
--rw-r--r--   0        0        0     1390 2022-08-17 04:07:59.986008 javelin-cli-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0      812 2023-06-14 04:57:05.265432 javelin-cli-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-14 04:42:13.306827 javelin-cli-0.8.0/javelin/__init__.py
+-rw-r--r--   0        0        0     6250 2023-06-14 04:42:13.157618 javelin-cli-0.8.0/javelin/__main__.py
+-rw-r--r--   0        0        0        0 2022-06-20 23:44:18.476590 javelin-cli-0.8.0/javelin/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2022-07-15 05:36:25.525384 javelin-cli-0.8.0/javelin/utils/aws.py
+-rw-r--r--   0        0        0     4494 2023-06-14 04:42:13.158776 javelin-cli-0.8.0/javelin/utils/github.py
+-rw-r--r--   0        0        0     4391 2023-06-14 04:42:13.159443 javelin-cli-0.8.0/javelin/utils/slack.py
+-rw-r--r--   0        0        0      633 2023-06-14 04:42:13.307351 javelin-cli-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1703 2023-06-14 05:02:33.949024 javelin-cli-0.8.0/setup.py
+-rw-r--r--   0        0        0     1613 2023-06-14 05:02:33.949329 javelin-cli-0.8.0/PKG-INFO
```

### Comparing `javelin-cli-0.7.7/README.md` & `javelin-cli-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,7 +14,27 @@
 [pyenv exec] pip install javelin-cli
 ```
 
 ## Usage
 ```sh
 python -m javelin --help
 ```
+
+## Contribution
+### Run lint
+```sh
+pylint javelin
+```
+
+### Create and push release commit
+```sh
+git commit -m v1.2.3
+git tag v1.2.3
+git push
+git push --tags
+```
+
+### Build and publish
+```sh
+poetry build
+poetry publish
+```
```

### Comparing `javelin-cli-0.7.7/javelin/__main__.py` & `javelin-cli-0.8.0/javelin/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 """Javelin
 """
 
 import getopt
 import sys
+import time
 
 import yaml
 
 from .utils import aws
 from .utils import github
 from .utils import slack
 from . import __version__
@@ -39,14 +40,15 @@
 """
 
 pr_numbers = []
 pulls = []
 command = ''
 project_name = ''
 bump_level = ''
+start_time = None
 
 def main(argv):
     _parse_command_arguments(argv)
 
     match command:
         case 'pre-release':
             _prerelease()
@@ -55,14 +57,17 @@
         case '':
             print("javelin: missing command")
             sys.exit(2)
         case _:
             print(f"javelin: invalid command '{command}'")
             sys.exit(2)
 
+    duration = time.time() - start_time
+    print(f'Finished in {duration:0.2f} seconds')
+
 def _parse_command_arguments(argv):
     global command
     global project_name
     global bump_level
 
     try:
         opts, args = getopt.gnu_getopt(argv, 'hvP:l:p:', ['help', 'version', 'project=', 'bump-level=', 'pull-request='])
@@ -100,16 +105,18 @@
         print("\njavelin: missing bump level")
         sys.exit(2)
     elif bump_level not in ('major', 'minor', 'patch'):
         print("\njavelin: invalid bump level")
         sys.exit(2)
 
 def _prerelease():
+    global start_time
+
     try:
-        repo_name = _get_project_repo_name(project_name)
+        repo_name = _get_project_repo_name()
         repo = github.get_repo(repo_name)
         prerelease_version = github.get_prerelease_version(repo, bump_level)
 
         print('The following actions will be performed:\n')
         print(f'  1. Merge these pull requests into the "{repo.default_branch}" branch:\n')
 
         for pr_number in pr_numbers:
@@ -125,29 +132,33 @@
         print(f'\n  2. Create a new GitHub Release with version {prerelease_version}')
         print(f'\n  3. Deploy the "{repo.default_branch}" branch to Staging 🚀\n')
 
         print('\n\033[1mDo you want to continue?\033[0m')
         print('  Only "yes" will be accepted.\n')
 
         if input('\033[1mEnter a value:\033[0m ') == 'yes':
+            start_time = time.time()
+
             github_succeeded = github.run_prerelease(repo, prerelease_version, pulls)
 
             if github_succeeded:
                 aws_succeeded = aws.start_pipeline_execution_and_wait(project_name, 'staging')
 
                 if aws_succeeded:
                     slack.notify_prerelease(project_name, repo, prerelease_version)
                 else:
                     slack.notify_prerelease_error(project_name, repo, prerelease_version, pulls)
     except KeyboardInterrupt:
         print('\n\nBye-bye')
 
 def _release():
+    global start_time
+
     try:
-        repo_name = _get_project_repo_name(project_name)
+        repo_name = _get_project_repo_name()
         repo = github.get_repo(repo_name)
         latest_prerelease = github.get_latest_prerelease(repo)
 
         if not latest_prerelease:
             print("javelin: repository doesn't have any pre-releases")
             sys.exit(2)
 
@@ -155,25 +166,27 @@
 
         print('The following actions will be performed:\n')
         print(f'\n  1. Deploy version {release_version} to Production 🚀\n')
         print('\n\033[1mDo you want to continue?\033[0m')
         print('  Only "yes" will be accepted.\n')
 
         if input('\033[1mEnter a value:\033[0m ') == 'yes':
+            start_time = time.time()
+
             succeeded = aws.start_pipeline_execution_and_wait(project_name, 'production')
 
             if succeeded:
                 github.run_release(repo)
                 slack.notify_release(project_name, repo, release_version)
             else:
                 slack.notify_release_error(project_name, repo, release_version, pulls)
     except KeyboardInterrupt:
         print('\n\nBye-bye')
 
-def _get_project_repo_name(project_name):
+def _get_project_repo_name():
     with open('./config/projects.yml', 'r', encoding='utf-8') as stream:
         try:
             config = yaml.safe_load(stream)
 
             return config[project_name]['repo_full_names']
         except (KeyError, yaml.YAMLError):
             print("\njavelin: invalid project name")
```

### Comparing `javelin-cli-0.7.7/javelin/utils/aws.py` & `javelin-cli-0.8.0/javelin/utils/aws.py`

 * *Files identical despite different names*

### Comparing `javelin-cli-0.7.7/javelin/utils/github.py` & `javelin-cli-0.8.0/javelin/utils/github.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,41 +107,41 @@
         repo.merge(repo.default_branch, pull.head.sha, f'{pull.title} #{pull.number}')
         repo.get_git_ref(f"heads/{pull.head.ref}").delete()
 
 def create_prerelease(repo, version):
     print(f'Creating pre-release {version}')
 
     default_branch = repo.get_branch(repo.default_branch)
-    release_message = build_release_message(repo, version)
+    release_message = build_release_message(repo)
 
     repo.create_git_tag_and_release(
         version,
         '',
         version,
         release_message,
         default_branch.commit.sha,
         'commit',
         prerelease=True,
     )
 
 def update_prerelease(release, repo, version):
     print(f'Updating pre-release {version}')
 
-    release_message = build_release_message(repo, version)
+    release_message = build_release_message(repo)
 
     release.update_release(
         version,
         release_message,
         prerelease=True,
         tag_name=version,
         target_commitish='main'
     )
 
-def build_release_message(repo, version):
-    commits = commits_between_prerelease_and_latest_release(repo, version)
+def build_release_message(repo):
+    commits = commits_between_prerelease_and_latest_release(repo)
     release_messages = []
 
     for commit in commits:
         if len(commit.parents) < 2:
             continue
 
         pulls = commit.get_pulls()
@@ -156,15 +156,15 @@
 
         release_messages.append(f'- [{commit_message}]({commit_url})')
 
     release_messages_unique = sorted(set(release_messages), key=release_messages.index)
 
     return '\n'.join(release_messages_unique)
 
-def commits_between_prerelease_and_latest_release(repo, prerelease_version):
+def commits_between_prerelease_and_latest_release(repo):
     try:
         tag_name = repo.get_latest_release().tag_name
         tag_commit_sha = repo.get_commit(tag_name).sha
         tag_commit = repo.get_git_commit(tag_commit_sha)
 
         since = tag_commit.author.date + datetime.timedelta(seconds=1)
     except UnknownObjectException:
```

### Comparing `javelin-cli-0.7.7/javelin/utils/slack.py` & `javelin-cli-0.8.0/javelin/utils/slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def notify_prerelease(project_name, repo, prerelease_version):
     url = _get_project_webhook_url(project_name)
     text = notify_prerelease_text(project_name, repo, prerelease_version)
 
     _send_message(url, text)
 
 def notify_prerelease_text(project_name, repo, prerelease_version):
-    commits = github.commits_between_prerelease_and_latest_release(repo, prerelease_version)
+    commits = github.commits_between_prerelease_and_latest_release(repo)
 
     message = f"""
 *{project_name.upper()} pre-release :pray:*
 
 <https://github.com/{repo.full_name}/releases/tag/{prerelease_version}|*{prerelease_version}*>
 {_message_links(commits)}
 
@@ -34,15 +34,15 @@
 def notify_release(project_name, repo, release_version):
     url = _get_project_webhook_url(project_name)
     text = notify_release_text(project_name, repo, release_version)
 
     _send_message(url, text)
 
 def notify_release_text(project_name, repo, release_version):
-    commits = github.commits_between_prerelease_and_latest_release(repo, release_version)
+    commits = github.commits_between_prerelease_and_latest_release(repo)
 
     message = f"""
 <!here> *{project_name.upper()} release :rocket:*
 
 <https://github.com/{repo.full_name}/releases/tag/{release_version}|*{release_version}*>
 {_message_links(commits)}
```

### Comparing `javelin-cli-0.7.7/pyproject.toml` & `javelin-cli-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "javelin-cli"
-version = "0.7.7"
+version = "0.8.0"
 description = "CLI tool for managing Spearly deployments."
 authors = ["David Grilli <dj@unimal.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/unimal-jp/javelin"
 packages = [
     { include = "javelin" }
```

### Comparing `javelin-cli-0.7.7/setup.py` & `javelin-cli-0.8.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'packaging>=21.3,<22.0',
  'python-dotenv>=0.20.0,<0.21.0',
  'python-semantic-release>=7.29.2,<8.0.0',
  'slack-sdk>=3.17.2,<4.0.0']
 
 setup_kwargs = {
     'name': 'javelin-cli',
-    'version': '0.7.7',
+    'version': '0.8.0',
     'description': 'CLI tool for managing Spearly deployments.',
-    'long_description': '# Javelin\n\nCLI tool for managing Spearly deployments.\n\n## Requirements\n- Python 3.10+\n- `GITHUB_ACCESS_TOKEN` environment variable set to a **GitHub Personal Access Token** with `repo` scope ([Ref](https://github.com/settings/tokens))\n- **AWS IAM User** with `codepipeline:StartPipelineExecution` permission to the required resources ([Ref](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html#configuration))\n\n## Installation\n```sh\nbrew install pyenv\npyenv install 3.10:latest\n[pyenv exec] pip install javelin-cli\n```\n\n## Usage\n```sh\npython -m javelin --help\n```\n',
+    'long_description': '# Javelin\n\nCLI tool for managing Spearly deployments.\n\n## Requirements\n- Python 3.10+\n- `GITHUB_ACCESS_TOKEN` environment variable set to a **GitHub Personal Access Token** with `repo` scope ([Ref](https://github.com/settings/tokens))\n- **AWS IAM User** with `codepipeline:StartPipelineExecution` permission to the required resources ([Ref](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html#configuration))\n\n## Installation\n```sh\nbrew install pyenv\npyenv install 3.10:latest\n[pyenv exec] pip install javelin-cli\n```\n\n## Usage\n```sh\npython -m javelin --help\n```\n\n## Contribution\n### Run lint\n```sh\npylint javelin\n```\n\n### Create and push release commit\n```sh\ngit commit -m v1.2.3\ngit tag v1.2.3\ngit push\ngit push --tags\n```\n\n### Build and publish\n```sh\npoetry build\npoetry publish\n```\n',
     'author': 'David Grilli',
     'author_email': 'dj@unimal.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/unimal-jp/javelin',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `javelin-cli-0.7.7/PKG-INFO` & `javelin-cli-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: javelin-cli
-Version: 0.7.7
+Version: 0.8.0
 Summary: CLI tool for managing Spearly deployments.
 Home-page: https://github.com/unimal-jp/javelin
 License: MIT
 Author: David Grilli
 Author-email: dj@unimal.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -37,7 +37,27 @@
 ```
 
 ## Usage
 ```sh
 python -m javelin --help
 ```
 
+## Contribution
+### Run lint
+```sh
+pylint javelin
+```
+
+### Create and push release commit
+```sh
+git commit -m v1.2.3
+git tag v1.2.3
+git push
+git push --tags
+```
+
+### Build and publish
+```sh
+poetry build
+poetry publish
+```
+
```

