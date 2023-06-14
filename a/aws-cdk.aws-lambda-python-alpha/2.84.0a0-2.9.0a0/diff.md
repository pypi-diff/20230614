# Comparing `tmp/aws-cdk.aws-lambda-python-alpha-2.84.0a0.tar.gz` & `tmp/aws-cdk.aws-lambda-python-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/aws-lambda-python-alpha/dist/python/aws-cdk.aws-lambda-python-alpha-2.84.0", last modified: Tue Jun 13 23:47:04 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-lambda-python/dist/python/aws-cdk.aws-lambda-python-alpha-2", last modified: Wed Jan 26 11:22:05 2022, max compression
```

## Comparing `aws-cdk.aws-lambda-python-alpha-2.84.0a0.tar` & `aws-cdk.aws-lambda-python-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11666 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10651 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1914 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk/aws_lambda_python_alpha/
--rw-r--r--   0 root         (0) root         (0)   121211 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk/aws_lambda_python_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk/aws_lambda_python_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      453 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk/aws_lambda_python_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47212 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk/aws_lambda_python_alpha/_jsii/aws-lambda-python-alpha@2.84.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:57.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk/aws_lambda_python_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11666 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      591 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:47:04.000000 aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7318 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6336 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1839 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk/aws_lambda_python_alpha/
+-rw-r--r--   0 root         (0) root         (0)    73125 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk/aws_lambda_python_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk/aws_lambda_python_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      417 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk/aws_lambda_python_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33854 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk/aws_lambda_python_alpha/_jsii/aws-lambda-python-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk/aws_lambda_python_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7318 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      590 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:05.000000 aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-lambda-python-alpha-2.84.0a0/LICENSE` & `aws-cdk.aws-lambda-python-alpha-2.9.0a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2018-2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+   Copyright 2018-2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `aws-cdk.aws-lambda-python-alpha-2.84.0a0/README.md` & `aws-cdk.aws-lambda-python-alpha-2.9.0a0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -19,46 +19,46 @@
 To use this module, you will need to have Docker installed.
 
 ## Python Function
 
 Define a `PythonFunction`:
 
 ```python
-python.PythonFunction(self, "MyFunction",
+lambda_.PythonFunction(self, "MyFunction",
     entry="/path/to/my/function",  # required
     runtime=Runtime.PYTHON_3_8,  # required
     index="my_index.py",  # optional, defaults to 'index.py'
     handler="my_exported_func"
 )
 ```
 
-All other properties of `lambda.Function` are supported, see also the [AWS Lambda construct library](https://github.com/aws/aws-cdk/tree/main/packages/%40aws-cdk/aws-lambda).
+All other properties of `lambda.Function` are supported, see also the [AWS Lambda construct library](https://github.com/aws/aws-cdk/tree/master/packages/%40aws-cdk/aws-lambda).
 
 ## Python Layer
 
 You may create a python-based lambda layer with `PythonLayerVersion`. If `PythonLayerVersion` detects a `requirements.txt`
 or `Pipfile` or `poetry.lock` with the associated `pyproject.toml` at the entry path, then `PythonLayerVersion` will include the dependencies inline with your code in the
 layer.
 
 Define a `PythonLayerVersion`:
 
 ```python
-python.PythonLayerVersion(self, "MyLayer",
+lambda_.PythonLayerVersion(self, "MyLayer",
     entry="/path/to/my/layer"
 )
 ```
 
 A layer can also be used as a part of a `PythonFunction`:
 
 ```python
-python.PythonFunction(self, "MyFunction",
+lambda_.PythonFunction(self, "MyFunction",
     entry="/path/to/my/function",
     runtime=Runtime.PYTHON_3_8,
     layers=[
-        python.PythonLayerVersion(self, "MyLayer",
+        lambda_.PythonLayerVersion(self, "MyLayer",
             entry="/path/to/my/layer"
         )
     ]
 )
 ```
 
 ## Packaging
@@ -103,80 +103,47 @@
 ```plaintext
 .
 ├── lambda_function.py # exports a function named 'handler'
 ├── pyproject.toml # your poetry project definition
 ├── poetry.lock # your poetry lock file has to be present at the entry path
 ```
 
-**Excluding source files**
-
-You can exclude files from being copied using the optional bundling string array parameter `assetExcludes`
-
-```python
-python.PythonFunction(self, "function",
-    entry="/path/to/poetry-function",
-    runtime=Runtime.PYTHON_3_8,
-    bundling=python.BundlingOptions(
-        # translates to `rsync --exclude='.venv'`
-        asset_excludes=[".venv"]
-    )
-)
-```
-
 ## Custom Bundling
 
 Custom bundling can be performed by passing in additional build arguments that point to index URLs to private repos, or by using an entirely custom Docker images for bundling dependencies. The build args currently supported are:
 
 * `PIP_INDEX_URL`
 * `PIP_EXTRA_INDEX_URL`
 * `HTTPS_PROXY`
 
 Additional build args for bundling that refer to PyPI indexes can be specified as:
 
 ```python
 entry = "/path/to/function"
 image = DockerImage.from_build(entry)
 
-python.PythonFunction(self, "function",
+lambda_.PythonFunction(self, "function",
     entry=entry,
     runtime=Runtime.PYTHON_3_8,
-    bundling=python.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         build_args={"PIP_INDEX_URL": "https://your.index.url/simple/", "PIP_EXTRA_INDEX_URL": "https://your.extra-index.url/simple/"}
     )
 )
 ```
 
 If using a custom Docker image for bundling, the dependencies are installed with `pip`, `pipenv` or `poetry` by using the `Packaging` class. A different bundling Docker image that is in the same directory as the function can be specified as:
 
 ```python
 entry = "/path/to/function"
 image = DockerImage.from_build(entry)
 
-python.PythonFunction(self, "function",
+lambda_.PythonFunction(self, "function",
     entry=entry,
     runtime=Runtime.PYTHON_3_8,
-    bundling=python.BundlingOptions(image=image)
-)
-```
-
-You can set additional Docker options to configure the build environment:
-
-```python
-entry = "/path/to/function"
-
-python.PythonFunction(self, "function",
-    entry=entry,
-    runtime=Runtime.PYTHON_3_8,
-    bundling=python.BundlingOptions(
-        network="host",
-        security_opt="no-new-privileges",
-        user="user:group",
-        volumes_from=["777f7dc92da7"],
-        volumes=[DockerVolume(host_path="/host-path", container_path="/container-path")]
-    )
+    bundling=lambda.BundlingOptions(image=image)
 )
 ```
 
 ## Custom Bundling with Code Artifact
 
 To use a Code Artifact PyPI repo, the `PIP_INDEX_URL` for bundling the function can be customized (requires AWS CLI in the build environment):
 
@@ -191,114 +158,17 @@
 domain_owner = "111122223333"
 repo_name = "my_repo"
 region = "us-east-1"
 code_artifact_auth_token = exec_sync(f"aws codeartifact get-authorization-token --domain {domain} --domain-owner {domainOwner} --query authorizationToken --output text").to_string().trim()
 
 index_url = f"https://aws:{codeArtifactAuthToken}@{domain}-{domainOwner}.d.codeartifact.{region}.amazonaws.com/pypi/{repoName}/simple/"
 
-python.PythonFunction(self, "function",
-    entry=entry,
-    runtime=Runtime.PYTHON_3_8,
-    bundling=python.BundlingOptions(
-        environment={"PIP_INDEX_URL": index_url}
-    )
-)
-```
-
-The index URL or the token are only used during bundling and thus not included in the final asset. Setting only environment variable for `PIP_INDEX_URL` or `PIP_EXTRA_INDEX_URL` should work for accesing private Python repositories with `pip`, `pipenv` and `poetry` based dependencies.
-
-If you also want to use the Code Artifact repo for building the base Docker image for bundling, use `buildArgs`. However, note that setting custom build args for bundling will force the base bundling image to be rebuilt every time (i.e. skip the Docker cache). Build args can be customized as:
-
-```python
-from child_process import exec_sync
-
-
-entry = "/path/to/function"
-image = DockerImage.from_build(entry)
-
-domain = "my-domain"
-domain_owner = "111122223333"
-repo_name = "my_repo"
-region = "us-east-1"
-code_artifact_auth_token = exec_sync(f"aws codeartifact get-authorization-token --domain {domain} --domain-owner {domainOwner} --query authorizationToken --output text").to_string().trim()
-
-index_url = f"https://aws:{codeArtifactAuthToken}@{domain}-{domainOwner}.d.codeartifact.{region}.amazonaws.com/pypi/{repoName}/simple/"
-
-python.PythonFunction(self, "function",
+lambda_.PythonFunction(self, "function",
     entry=entry,
     runtime=Runtime.PYTHON_3_8,
-    bundling=python.BundlingOptions(
+    bundling=lambda.BundlingOptions(
         build_args={"PIP_INDEX_URL": index_url}
     )
 )
 ```
 
-## Command hooks
-
-It is  possible to run additional commands by specifying the `commandHooks` prop:
-
-```python
-entry = "/path/to/function"
-python.PythonFunction(self, "function",
-    entry=entry,
-    runtime=Runtime.PYTHON_3_8,
-    bundling=python.BundlingOptions(
-        command_hooks={
-            # run tests
-            def before_bundling(self, input_dir):
-                return ["pytest"],
-            def after_bundling(self, input_dir):
-                return ["pylint"]
-        }
-    )
-)
-```
-
-The following hooks are available:
-
-* `beforeBundling`: runs before all bundling commands
-* `afterBundling`: runs after all bundling commands
-
-They all receive the directory containing the dependencies file (`inputDir`) and the
-directory where the bundled asset will be output (`outputDir`). They must return
-an array of commands to run. Commands are chained with `&&`.
-
-The commands will run in the environment in which bundling occurs: inside the
-container for Docker bundling or on the host OS for local bundling.
-
-## Docker based bundling in complex Docker configurations
-
-By default the input and output of Docker based bundling is handled via bind mounts.
-In situtations where this does not work, like Docker-in-Docker setups or when using a remote Docker socket, you can configure an alternative, but slower, variant that also works in these situations.
-
-```python
-entry = "/path/to/function"
-
-python.PythonFunction(self, "function",
-    entry=entry,
-    runtime=Runtime.PYTHON_3_8,
-    bundling=python.BundlingOptions(
-        bundling_file_access=BundlingFileAccess.VOLUME_COPY
-    )
-)
-```
-
-## Troubleshooting
-
-### Containerfile: no such file or directory
-
-If you are on a Mac, using [Finch](https://github.com/runfinch/finch) instead of Docker, and see an error
-like this:
-
-```txt
-lstat /private/var/folders/zx/d5wln9n10sn0tcj1v9798f1c0000gr/T/jsii-kernel-9VYgrO/node_modules/@aws-cdk/aws-lambda-python-alpha/lib/Containerfile: no such file or directory
-```
-
-That is a sign that your temporary directory has not been mapped into the Finch VM. Add the following to `~/.finch/finch.yaml`:
-
-```yaml
-additional_directories:
-  - path: /private/var/folders/
-  - path: /var/folders/
-```
-
-Then restart the Finch VM by running `finch vm stop && finch vm start`.
+This type of an example should work for `pip` and `poetry` based dependencies, but will not work for `pipenv`.
```

### Comparing `aws-cdk.aws-lambda-python-alpha-2.84.0a0/setup.py` & `aws-cdk.aws-lambda-python-alpha-2.9.0a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-lambda-python-alpha",
-    "version": "2.84.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS Lambda in Python",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_lambda_python_alpha",
         "aws_cdk.aws_lambda_python_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_lambda_python_alpha._jsii": [
-            "aws-lambda-python-alpha@2.84.0-alpha.0.jsii.tgz"
+            "aws-lambda-python-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_lambda_python_alpha": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk-lib==2.84.0",
+        "aws-cdk-lib>=2.9.0, <3.0.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.82.0, <2.0.0",
-        "publication>=0.0.3",
-        "typeguard~=2.13.3"
+        "jsii>=1.52.1, <2.0.0",
+        "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved",
         "Framework :: AWS CDK",
-        "Framework :: AWS CDK :: 2"
+        "Framework :: AWS CDK :: 1"
     ],
     "scripts": []
 }
 """
 )
 
 with open("README.md", encoding="utf8") as fp:
```

### Comparing `aws-cdk.aws-lambda-python-alpha-2.84.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-lambda-python-alpha-2.9.0a0/src/aws_cdk.aws_lambda_python_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_lambda_python_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_lambda_python_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_lambda_python_alpha.egg-info/requires.txt
 src/aws_cdk.aws_lambda_python_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_lambda_python_alpha/__init__.py
 src/aws_cdk/aws_lambda_python_alpha/py.typed
 src/aws_cdk/aws_lambda_python_alpha/_jsii/__init__.py
-src/aws_cdk/aws_lambda_python_alpha/_jsii/aws-lambda-python-alpha@2.84.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_lambda_python_alpha/_jsii/aws-lambda-python-alpha@2.9.0-alpha.0.jsii.tgz
```

