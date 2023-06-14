# Comparing `tmp/code2gist-1.0.1.tar.gz` & `tmp/code2gist-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code2gist-1.0.1.tar", last modified: Wed Jun 14 03:15:16 2023, max compression
+gzip compressed data, was "code2gist-1.1.2.tar", last modified: Wed Jun 14 19:13:57 2023, max compression
```

## Comparing `code2gist-1.0.1.tar` & `code2gist-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:15:16.636114 code2gist-1.0.1/
--rw-rw-rw-   0        0        0    35823 2023-06-13 15:23:13.000000 code2gist-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3961 2023-06-14 03:15:16.635114 code2gist-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2023-06-14 03:13:54.000000 code2gist-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 03:15:16.587160 code2gist-1.0.1/code2gist/
--rw-rw-rw-   0        0        0       22 2023-06-13 18:34:11.000000 code2gist-1.0.1/code2gist/__init__.py
--rw-rw-rw-   0        0        0     3520 2023-06-14 02:33:47.000000 code2gist-1.0.1/code2gist/main.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:15:16.632147 code2gist-1.0.1/code2gist.egg-info/
--rw-rw-rw-   0        0        0     3961 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 03:15:16.000000 code2gist-1.0.1/code2gist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      628 2023-06-14 03:14:07.000000 code2gist-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 03:15:16.636114 code2gist-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 19:13:57.418779 code2gist-1.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-13 15:23:13.000000 code2gist-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4786 2023-06-14 19:13:57.417780 code2gist-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4417 2023-06-14 18:51:47.000000 code2gist-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 19:13:57.375529 code2gist-1.1.2/code2gist/
+-rw-rw-rw-   0        0        0       22 2023-06-13 18:34:11.000000 code2gist-1.1.2/code2gist/__init__.py
+-rw-rw-rw-   0        0        0     3895 2023-06-14 19:11:55.000000 code2gist-1.1.2/code2gist/main.py
+drwxrwxrwx   0        0        0        0 2023-06-14 19:13:57.415778 code2gist-1.1.2/code2gist.egg-info/
+-rw-rw-rw-   0        0        0     4786 2023-06-14 19:13:57.000000 code2gist-1.1.2/code2gist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-14 19:13:57.000000 code2gist-1.1.2/code2gist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 19:13:57.000000 code2gist-1.1.2/code2gist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-14 19:13:57.000000 code2gist-1.1.2/code2gist.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-14 19:13:57.000000 code2gist-1.1.2/code2gist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 19:13:57.000000 code2gist-1.1.2/code2gist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      628 2023-06-14 19:13:11.000000 code2gist-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 19:13:57.418779 code2gist-1.1.2/setup.cfg
```

### Comparing `code2gist-1.0.1/LICENSE` & `code2gist-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `code2gist-1.0.1/PKG-INFO` & `code2gist-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: code2gist
-Version: 1.0.1
-Summary: Upload Python files in a directory to a GitHub Gist.
-Author-email: Cameron Spears <crspears@outlook.com>
-License: GPL-3.0
-Keywords: python,github,gist,upload
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 #  code2gist
 
 `code2gist` is a Python package that makes sharing your code projects easier than ever. With a simple command, it lets you upload your code files to GitHub's Gist. `code2gist` is available on [PyPI](https://pypi.org/project/code2gist/).
 
 The package works hand-in-hand with OpenAI's ChatGPT-4's 'Browse with Bing' feature. This compatibility allows you to present substantial code bases to the model in a single instance, eliminating the need to split your code into smaller parts.
 
 Another key feature of `code2gist` is its ability to handle a wide range of text-based file types, not just Python files.
@@ -24,14 +12,45 @@
 
 You can install the package via pip:
 
 ```
 pip install code2gist
 ```
 
+### Adding code2gist Directory to the PATH Environment Variable
+
+Here are step-by-step instructions to add the code2gist directory to your PATH environment variable on Windows:
+
+1. Open the **Control Panel**.
+2. Navigate to **System and Security > System**.
+3. Click on the **Advanced system settings** link on the left panel.
+4. Click **Environment Variables**.
+5. Under the **System Variables** section, find and double-click the variable **PATH**.
+6. Click **New**.
+7. Add the directory where code2gist is installed. For example, if you have Python 3.11 installed, the directory might look like this: `C:\...\Python311\Scripts`
+8. Click **OK** to close all windows and save the changes.
+
+After following these steps, your system should recognize code2gist commands from any directory in the command line.
+
+### GitHub Token
+
+`code2gist` requires a GitHub token to function. You need to create a new token with the `gist` scope (which allows it to create gists). Follow [this guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a new token.
+
+Once you have your token, you should store it in the "GITHUB_TOKEN" environment variable. Here are the steps to set this variable in Windows:
+
+1. Open the Control Panel.
+2. Search for "Environment Variables".
+3. Click on "Edit the system environment variables".
+4. In the System Properties window that appears, click the "Environment Variables..." button.
+5. In the Environment Variables window, click the "New..." button under the "User variables" section.
+6. Enter "GITHUB_TOKEN" as the variable name and your token as the variable value.
+7. Click "OK" on all open windows to apply the changes.
+
+Please ensure that you have this variable set before using the package.
+
 ## Usage
 
 ### Uploading Files
 
 To use `code2gist`, simply use the following command:
 
 ```
@@ -54,30 +73,14 @@
 
 ```
 code2gist --prune
 ```
 
 Running this command will delete all your gists with "[code2gist]" in the description.
 
-## GitHub Token
-
-`code2gist` requires a GitHub token to function. You need to create a new token with the `gist` scope (which allows it to create gists). Follow [this guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a new token.
-
-Once you have your token, you should store it in the "GITHUB_TOKEN" environment variable. Here are the steps to set this variable in Windows:
-
-1. Open the Control Panel.
-2. Search for "Environment Variables".
-3. Click on "Edit the system environment variables".
-4. In the System Properties window that appears, click the "Environment Variables..." button.
-5. In the Environment Variables window, click the "New..." button under the "User variables" section.
-6. Enter "GITHUB_TOKEN" as the variable name and your token as the variable value.
-7. Click "OK" on all open windows to apply the changes.
-
-Please ensure that you have this variable set before using the package.
-
 ## .gitignore Support
 
 `code2gist` respects `.gitignore` rules. Files that match a rule in the `.gitignore` file of the directory being uploaded will be skipped. In addition, by default, `code2gist` skips files and directories that start with a dot (`.`), although this behavior may change in future versions to strictly adhere to `.gitignore`.
 
 ## Note
 
 The gists created by `code2gist` are private by default, providing a safe way for you to share your code without making it publicly available.
```

### Comparing `code2gist-1.0.1/README.md` & `code2gist-1.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: code2gist
+Version: 1.1.2
+Summary: Upload Python files in a directory to a GitHub Gist.
+Author-email: Cameron Spears <crspears@outlook.com>
+License: GPL-3.0
+Keywords: python,github,gist,upload
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.11.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 #  code2gist
 
 `code2gist` is a Python package that makes sharing your code projects easier than ever. With a simple command, it lets you upload your code files to GitHub's Gist. `code2gist` is available on [PyPI](https://pypi.org/project/code2gist/).
 
 The package works hand-in-hand with OpenAI's ChatGPT-4's 'Browse with Bing' feature. This compatibility allows you to present substantial code bases to the model in a single instance, eliminating the need to split your code into smaller parts.
 
 Another key feature of `code2gist` is its ability to handle a wide range of text-based file types, not just Python files.
@@ -12,14 +24,45 @@
 
 You can install the package via pip:
 
 ```
 pip install code2gist
 ```
 
+### Adding code2gist Directory to the PATH Environment Variable
+
+Here are step-by-step instructions to add the code2gist directory to your PATH environment variable on Windows:
+
+1. Open the **Control Panel**.
+2. Navigate to **System and Security > System**.
+3. Click on the **Advanced system settings** link on the left panel.
+4. Click **Environment Variables**.
+5. Under the **System Variables** section, find and double-click the variable **PATH**.
+6. Click **New**.
+7. Add the directory where code2gist is installed. For example, if you have Python 3.11 installed, the directory might look like this: `C:\...\Python311\Scripts`
+8. Click **OK** to close all windows and save the changes.
+
+After following these steps, your system should recognize code2gist commands from any directory in the command line.
+
+### GitHub Token
+
+`code2gist` requires a GitHub token to function. You need to create a new token with the `gist` scope (which allows it to create gists). Follow [this guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a new token.
+
+Once you have your token, you should store it in the "GITHUB_TOKEN" environment variable. Here are the steps to set this variable in Windows:
+
+1. Open the Control Panel.
+2. Search for "Environment Variables".
+3. Click on "Edit the system environment variables".
+4. In the System Properties window that appears, click the "Environment Variables..." button.
+5. In the Environment Variables window, click the "New..." button under the "User variables" section.
+6. Enter "GITHUB_TOKEN" as the variable name and your token as the variable value.
+7. Click "OK" on all open windows to apply the changes.
+
+Please ensure that you have this variable set before using the package.
+
 ## Usage
 
 ### Uploading Files
 
 To use `code2gist`, simply use the following command:
 
 ```
@@ -42,30 +85,14 @@
 
 ```
 code2gist --prune
 ```
 
 Running this command will delete all your gists with "[code2gist]" in the description.
 
-## GitHub Token
-
-`code2gist` requires a GitHub token to function. You need to create a new token with the `gist` scope (which allows it to create gists). Follow [this guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a new token.
-
-Once you have your token, you should store it in the "GITHUB_TOKEN" environment variable. Here are the steps to set this variable in Windows:
-
-1. Open the Control Panel.
-2. Search for "Environment Variables".
-3. Click on "Edit the system environment variables".
-4. In the System Properties window that appears, click the "Environment Variables..." button.
-5. In the Environment Variables window, click the "New..." button under the "User variables" section.
-6. Enter "GITHUB_TOKEN" as the variable name and your token as the variable value.
-7. Click "OK" on all open windows to apply the changes.
-
-Please ensure that you have this variable set before using the package.
-
 ## .gitignore Support
 
 `code2gist` respects `.gitignore` rules. Files that match a rule in the `.gitignore` file of the directory being uploaded will be skipped. In addition, by default, `code2gist` skips files and directories that start with a dot (`.`), although this behavior may change in future versions to strictly adhere to `.gitignore`.
 
 ## Note
 
 The gists created by `code2gist` are private by default, providing a safe way for you to share your code without making it publicly available.
@@ -74,8 +101,8 @@
 
 ## License
 
 `code2gist` is licensed underthe [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
 
 ------
 
-We hope `code2gist` serves as a valuable tool in your development toolkit. Happy coding!
+We hope `code2gist` serves as a valuable tool in your development toolkit. Happy coding!
```

### Comparing `code2gist-1.0.1/code2gist/main.py` & `code2gist-1.1.2/code2gist/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     }
     data = {
         "public": False,
         "description": description,
         "files": files
     }
     response = requests.post(url, headers=headers, data=json.dumps(data))
+    if response.status_code != 201:
+        print(f"Failed to create a gist: {response.text}")
+        return None
     return response.json()
 
 def get_files_in_directory(directory, extensions):
     # Load the .gitignore file, if it exists.
     gitignore_path = os.path.join(directory, '.gitignore')
     gitignore = None
     if os.path.exists(gitignore_path):
@@ -43,52 +46,57 @@
             # Skip the file if it matches a .gitignore rule.
             if gitignore and gitignore.match_file(rel_path):
                 continue
 
             try:
                 with open(path, 'rt') as file:
                     files[rel_path] = {"content": file.read()}
-            except UnicodeDecodeError:
-                print(f"Could not read file: {path}")
+            except (UnicodeDecodeError, IOError) as e:
+                print(f"Error reading file: {path}. Error: {str(e)}")
+                continue
     return files
 
 def delete_old_gists():
     token = os.getenv("GITHUB_TOKEN")
     if not token:
         raise ValueError("GITHUB_TOKEN environment variable not found")
     url = "https://api.github.com/gists"
     headers = {
         "Authorization": f"token {token}",
         "Accept": "application/vnd.github.v3+json",
     }
     response = requests.get(url, headers=headers)
+    if response.status_code != 200:
+        print(f"Failed to fetch gists: {response.text}")
+        return
     gists = response.json()
     for gist in gists:
         if '[code2gist]' in gist['description']:
             delete_url = f"https://api.github.com/gists/{gist['id']}"
             delete_response = requests.delete(delete_url, headers=headers)
-            if delete_response.status_code == 204:
-                print(f"Deleted Gist: {gist['id']}")
-            else:
-                print(f"Failed to delete Gist: {gist['id']}")
+            if delete_response.status_code != 204:
+                print(f"Failed to delete Gist: {gist['id']}, response: {delete_response.text}")
+                continue
+            print(f"Deleted Gist: {gist['id']}")
 
 def main():
     parser = argparse.ArgumentParser(description='Upload Python files in a directory to Gist.')
     parser.add_argument('directory', type=str, nargs='?', help='the directory to upload')
     parser.add_argument('--ext', nargs='+', default=['.py'], help='file extensions to include')
     parser.add_argument('--prune', action='store_true', help='delete all gists created by this application')
     args = parser.parse_args()
 
     if args.directory:
         directory = args.directory
         description = os.path.basename(os.getcwd()) + " [code2gist]"
         files = get_files_in_directory(directory, args.ext)
         response = create_gist(description, files)
-        for filename, file_info in response['files'].items():
-            print(f"\n- File: {filename}")
-            print(f" URL: {file_info['raw_url']}")
-        
+        if response:
+            for filename, file_info in response['files'].items():
+                print(f"\n- File: {filename}")
+                print(f" URL: {file_info['raw_url']}")
+                print()
     if args.prune:
         delete_old_gists()
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `code2gist-1.0.1/code2gist.egg-info/PKG-INFO` & `code2gist-1.1.2/code2gist.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code2gist
-Version: 1.0.1
+Version: 1.1.2
 Summary: Upload Python files in a directory to a GitHub Gist.
 Author-email: Cameron Spears <crspears@outlook.com>
 License: GPL-3.0
 Keywords: python,github,gist,upload
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
@@ -24,14 +24,45 @@
 
 You can install the package via pip:
 
 ```
 pip install code2gist
 ```
 
+### Adding code2gist Directory to the PATH Environment Variable
+
+Here are step-by-step instructions to add the code2gist directory to your PATH environment variable on Windows:
+
+1. Open the **Control Panel**.
+2. Navigate to **System and Security > System**.
+3. Click on the **Advanced system settings** link on the left panel.
+4. Click **Environment Variables**.
+5. Under the **System Variables** section, find and double-click the variable **PATH**.
+6. Click **New**.
+7. Add the directory where code2gist is installed. For example, if you have Python 3.11 installed, the directory might look like this: `C:\...\Python311\Scripts`
+8. Click **OK** to close all windows and save the changes.
+
+After following these steps, your system should recognize code2gist commands from any directory in the command line.
+
+### GitHub Token
+
+`code2gist` requires a GitHub token to function. You need to create a new token with the `gist` scope (which allows it to create gists). Follow [this guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a new token.
+
+Once you have your token, you should store it in the "GITHUB_TOKEN" environment variable. Here are the steps to set this variable in Windows:
+
+1. Open the Control Panel.
+2. Search for "Environment Variables".
+3. Click on "Edit the system environment variables".
+4. In the System Properties window that appears, click the "Environment Variables..." button.
+5. In the Environment Variables window, click the "New..." button under the "User variables" section.
+6. Enter "GITHUB_TOKEN" as the variable name and your token as the variable value.
+7. Click "OK" on all open windows to apply the changes.
+
+Please ensure that you have this variable set before using the package.
+
 ## Usage
 
 ### Uploading Files
 
 To use `code2gist`, simply use the following command:
 
 ```
@@ -54,30 +85,14 @@
 
 ```
 code2gist --prune
 ```
 
 Running this command will delete all your gists with "[code2gist]" in the description.
 
-## GitHub Token
-
-`code2gist` requires a GitHub token to function. You need to create a new token with the `gist` scope (which allows it to create gists). Follow [this guide](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a new token.
-
-Once you have your token, you should store it in the "GITHUB_TOKEN" environment variable. Here are the steps to set this variable in Windows:
-
-1. Open the Control Panel.
-2. Search for "Environment Variables".
-3. Click on "Edit the system environment variables".
-4. In the System Properties window that appears, click the "Environment Variables..." button.
-5. In the Environment Variables window, click the "New..." button under the "User variables" section.
-6. Enter "GITHUB_TOKEN" as the variable name and your token as the variable value.
-7. Click "OK" on all open windows to apply the changes.
-
-Please ensure that you have this variable set before using the package.
-
 ## .gitignore Support
 
 `code2gist` respects `.gitignore` rules. Files that match a rule in the `.gitignore` file of the directory being uploaded will be skipped. In addition, by default, `code2gist` skips files and directories that start with a dot (`.`), although this behavior may change in future versions to strictly adhere to `.gitignore`.
 
 ## Note
 
 The gists created by `code2gist` are private by default, providing a safe way for you to share your code without making it publicly available.
```

### Comparing `code2gist-1.0.1/pyproject.toml` & `code2gist-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "code2gist"
-version = "1.0.1"
+version = "1.1.2"
 authors = [
     {name = "Cameron Spears", email = "crspears@outlook.com"},
 ]
 description = "Upload Python files in a directory to a GitHub Gist."
 readme = "README.md"
 requires-python = ">=3.11.4"
 keywords = ["python", "github", "gist", "upload"]
```

