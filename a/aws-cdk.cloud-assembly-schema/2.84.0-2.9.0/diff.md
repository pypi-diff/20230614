# Comparing `tmp/aws-cdk.cloud-assembly-schema-2.84.0.tar.gz` & `tmp/aws-cdk.cloud-assembly-schema-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src733638879/src/packages/@aws-cdk/cloud-assembly-schema/dist/python/aws-cdk.cloud-assembly-schema-2.84.0.tar", last modified: Tue Jun 13 23:46:45 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/@aws-cdk/cloud-assembly-schema/dist/python/aws-cdk.cloud-assembly-schema-2.9.0.tar", last modified: Wed Jan 26 10:30:18 2022, max compression
```

## Comparing `aws-cdk.cloud-assembly-schema-2.84.0.tar` & `aws-cdk.cloud-assembly-schema-2.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3872 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3777 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2782 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1805 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk/cloud_assembly_schema/
--rw-r--r--   0 root         (0) root         (0)   373534 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk/cloud_assembly_schema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk/cloud_assembly_schema/_jsii/
--rw-r--r--   0 root         (0) root         (0)      387 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk/cloud_assembly_schema/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   181669 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.84.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:37.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk/cloud_assembly_schema/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk.cloud_assembly_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3777 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk.cloud_assembly_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      563 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk.cloud_assembly_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk.cloud_assembly_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 23:46:45.000000 aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk.cloud_assembly_schema.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.cloud-assembly-schema-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3871 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3928 2022-01-26 10:30:18.000000 aws-cdk.cloud-assembly-schema-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2966 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 10:30:18.000000 aws-cdk.cloud-assembly-schema-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1723 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk/cloud_assembly_schema/
+-rw-r--r--   0 root         (0) root         (0)   153569 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk/cloud_assembly_schema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk/cloud_assembly_schema/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      351 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk/cloud_assembly_schema/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126700 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.9.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 10:30:14.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk/cloud_assembly_schema/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 10:30:18.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk.cloud_assembly_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3928 2022-01-26 10:30:17.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk.cloud_assembly_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      562 2022-01-26 10:30:17.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 10:30:17.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk.cloud_assembly_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2022-01-26 10:30:17.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk.cloud_assembly_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 10:30:17.000000 aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk.cloud_assembly_schema.egg-info/top_level.txt
```

### Comparing `aws-cdk.cloud-assembly-schema-2.84.0/LICENSE` & `aws-cdk.cloud-assembly-schema-2.9.0/LICENSE`

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

### Comparing `aws-cdk.cloud-assembly-schema-2.84.0/NOTICE` & `aws-cdk.cloud-assembly-schema-2.9.0/NOTICE`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 AWS Cloud Development Kit (AWS CDK)
-Copyright 2018-2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+Copyright 2018-2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
 -------------------------------------------------------------------------------
 
 The AWS CDK includes the following third-party software/licensing:
 
 ** jsonschema - https://www.npmjs.com/package/jsonschema
 Copyright (C) 2012-2015 Tom de Grunt <tom@degrunt.nl>
@@ -41,15 +41,15 @@
 ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR
 IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 ----------------
 
-** semver - https://www.npmjs.com/package/semver
+** yallist - https://www.npmjs.com/package/yallist
 Copyright (c) Isaac Z. Schlueter and Contributors
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted, provided that the above
 copyright notice and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
@@ -58,23 +58,23 @@
 ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR
 IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 ----------------
 
-** yallist - https://www.npmjs.com/package/yallist
+** semver - https://www.npmjs.com/package/semver
 Copyright (c) Isaac Z. Schlueter and Contributors
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted, provided that the above
 copyright notice and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR
 IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-----------------
+----------------
```

### Comparing `aws-cdk.cloud-assembly-schema-2.84.0/PKG-INFO` & `aws-cdk.cloud-assembly-schema-2.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cloud-assembly-schema
-Version: 2.84.0
+Version: 2.9.0
 Summary: Cloud Assembly Schema
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
+Classifier: Framework :: AWS CDK :: 1
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Cloud Assembly Schema
 
+<!--BEGIN STABILITY BANNER-->---
+
+
+![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+
+---
+<!--END STABILITY BANNER-->
+
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project.
 
 ## Cloud Assembly
 
 The *Cloud Assembly* is the output of the synthesis operation. It is produced as part of the
-[`cdk synth`](https://github.com/aws/aws-cdk/tree/main/packages/aws-cdk#cdk-synthesize)
-command, or the [`app.synth()`](https://github.com/aws/aws-cdk/blob/main/packages/@aws-cdk/core/lib/app.ts#L135) method invocation.
+[`cdk synth`](https://github.com/aws/aws-cdk/tree/master/packages/aws-cdk#cdk-synthesize)
+command, or the [`app.synth()`](https://github.com/aws/aws-cdk/blob/master/packages/@aws-cdk/core/lib/app.ts#L135) method invocation.
 
 Its essentially a set of files and directories, one of which is the `manifest.json` file. It defines the set of instructions that are
 needed in order to deploy the assembly directory.
 
 > For example, when `cdk deploy` is executed, the CLI reads this file and performs its instructions:
 >
 > * Build container images.
@@ -75,7 +83,9 @@
 
 > For example, if your consumer was built when the schema version was 2.0.0, you should reject deploying cloud assemblies with a
 > manifest version of 3.0.0.
 
 ## Contributing
 
 See [Contribution Guide](./CONTRIBUTING.md)
+
+
```

### Comparing `aws-cdk.cloud-assembly-schema-2.84.0/README.md` & `aws-cdk.cloud-assembly-schema-2.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 # Cloud Assembly Schema
 
+<!--BEGIN STABILITY BANNER-->---
+
+
+![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+
+---
+<!--END STABILITY BANNER-->
+
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project.
 
 ## Cloud Assembly
 
 The *Cloud Assembly* is the output of the synthesis operation. It is produced as part of the
-[`cdk synth`](https://github.com/aws/aws-cdk/tree/main/packages/aws-cdk#cdk-synthesize)
-command, or the [`app.synth()`](https://github.com/aws/aws-cdk/blob/main/packages/@aws-cdk/core/lib/app.ts#L135) method invocation.
+[`cdk synth`](https://github.com/aws/aws-cdk/tree/master/packages/aws-cdk#cdk-synthesize)
+command, or the [`app.synth()`](https://github.com/aws/aws-cdk/blob/master/packages/@aws-cdk/core/lib/app.ts#L135) method invocation.
 
 Its essentially a set of files and directories, one of which is the `manifest.json` file. It defines the set of instructions that are
 needed in order to deploy the assembly directory.
 
 > For example, when `cdk deploy` is executed, the CLI reads this file and performs its instructions:
 >
 > * Build container images.
```

### Comparing `aws-cdk.cloud-assembly-schema-2.84.0/setup.py` & `aws-cdk.cloud-assembly-schema-2.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cloud-assembly-schema",
-    "version": "2.84.0",
+    "version": "2.9.0",
     "description": "Cloud Assembly Schema",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,41 +22,39 @@
     },
     "packages": [
         "aws_cdk.cloud_assembly_schema",
         "aws_cdk.cloud_assembly_schema._jsii"
     ],
     "package_data": {
         "aws_cdk.cloud_assembly_schema._jsii": [
-            "cloud-assembly-schema@2.84.0.jsii.tgz"
+            "cloud-assembly-schema@2.9.0.jsii.tgz"
         ],
         "aws_cdk.cloud_assembly_schema": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": ">=3.6",
     "install_requires": [
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
         "Development Status :: 5 - Production/Stable",
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

### Comparing `aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk.cloud_assembly_schema.egg-info/PKG-INFO` & `aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk.cloud_assembly_schema.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cloud-assembly-schema
-Version: 2.84.0
+Version: 2.9.0
 Summary: Cloud Assembly Schema
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Classifier: Framework :: AWS CDK
-Classifier: Framework :: AWS CDK :: 2
-Requires-Python: ~=3.7
+Classifier: Framework :: AWS CDK :: 1
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Cloud Assembly Schema
 
+<!--BEGIN STABILITY BANNER-->---
+
+
+![cdk-constructs: Stable](https://img.shields.io/badge/cdk--constructs-stable-success.svg?style=for-the-badge)
+
+---
+<!--END STABILITY BANNER-->
+
 This module is part of the [AWS Cloud Development Kit](https://github.com/aws/aws-cdk) project.
 
 ## Cloud Assembly
 
 The *Cloud Assembly* is the output of the synthesis operation. It is produced as part of the
-[`cdk synth`](https://github.com/aws/aws-cdk/tree/main/packages/aws-cdk#cdk-synthesize)
-command, or the [`app.synth()`](https://github.com/aws/aws-cdk/blob/main/packages/@aws-cdk/core/lib/app.ts#L135) method invocation.
+[`cdk synth`](https://github.com/aws/aws-cdk/tree/master/packages/aws-cdk#cdk-synthesize)
+command, or the [`app.synth()`](https://github.com/aws/aws-cdk/blob/master/packages/@aws-cdk/core/lib/app.ts#L135) method invocation.
 
 Its essentially a set of files and directories, one of which is the `manifest.json` file. It defines the set of instructions that are
 needed in order to deploy the assembly directory.
 
 > For example, when `cdk deploy` is executed, the CLI reads this file and performs its instructions:
 >
 > * Build container images.
@@ -75,7 +83,9 @@
 
 > For example, if your consumer was built when the schema version was 2.0.0, you should reject deploying cloud assemblies with a
 > manifest version of 3.0.0.
 
 ## Contributing
 
 See [Contribution Guide](./CONTRIBUTING.md)
+
+
```

### Comparing `aws-cdk.cloud-assembly-schema-2.84.0/src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt` & `aws-cdk.cloud-assembly-schema-2.9.0/src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.cloud_assembly_schema.egg-info/SOURCES.txt
 src/aws_cdk.cloud_assembly_schema.egg-info/dependency_links.txt
 src/aws_cdk.cloud_assembly_schema.egg-info/requires.txt
 src/aws_cdk.cloud_assembly_schema.egg-info/top_level.txt
 src/aws_cdk/cloud_assembly_schema/__init__.py
 src/aws_cdk/cloud_assembly_schema/py.typed
 src/aws_cdk/cloud_assembly_schema/_jsii/__init__.py
-src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.84.0.jsii.tgz
+src/aws_cdk/cloud_assembly_schema/_jsii/cloud-assembly-schema@2.9.0.jsii.tgz
```

