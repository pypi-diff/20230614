# Comparing `tmp/secscanner2junit-0.1.7.tar.gz` & `tmp/secscanner2junit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secscanner2junit-0.1.7.tar", max compression
+gzip compressed data, was "secscanner2junit-0.1.9.tar", max compression
```

## Comparing `secscanner2junit-0.1.7.tar` & `secscanner2junit-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0    35149 2022-09-27 08:00:47.100817 secscanner2junit-0.1.7/LICENSE
--rw-r--r--   0        0        0     3808 2022-09-27 08:00:47.100817 secscanner2junit-0.1.7/README.md
--rw-r--r--   0        0        0      656 2022-09-27 08:00:47.100817 secscanner2junit-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1244 2022-09-27 08:00:47.100817 secscanner2junit-0.1.7/secscanner2junit/__init__.py
--rw-r--r--   0        0        0     2598 2022-09-27 08:00:47.100817 secscanner2junit-0.1.7/secscanner2junit/config.py
--rw-r--r--   0        0        0      223 2022-09-27 08:00:47.100817 secscanner2junit-0.1.7/secscanner2junit/parser.py
--rw-r--r--   0        0        0     4260 2022-09-27 08:00:47.100817 secscanner2junit-0.1.7/secscanner2junit/sast.py
--rw-r--r--   0        0        0     1244 2022-09-27 08:00:47.100817 secscanner2junit-0.1.7/secscanner2junit/secrets.py
--rw-r--r--   0        0        0     4768 1970-01-01 00:00:00.000000 secscanner2junit-0.1.7/setup.py
--rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 secscanner2junit-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4463 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/README.md
+-rw-r--r--   0        0        0      656 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1462 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/secscanner2junit/__init__.py
+-rw-r--r--   0        0        0     2598 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/secscanner2junit/config.py
+-rw-r--r--   0        0        0     1699 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/secscanner2junit/container_scanning.py
+-rw-r--r--   0        0        0       47 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/secscanner2junit/logger.py
+-rw-r--r--   0        0        0      223 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/secscanner2junit/parser.py
+-rw-r--r--   0        0        0     4260 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/secscanner2junit/sast.py
+-rw-r--r--   0        0        0     1244 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/secscanner2junit/secrets.py
+-rw-r--r--   0        0        0     7232 2022-10-07 10:21:10.892479 secscanner2junit-0.1.9/secscanner2junit/vulnerability.py
+-rw-r--r--   0        0        0     5449 1970-01-01 00:00:00.000000 secscanner2junit-0.1.9/setup.py
+-rw-r--r--   0        0        0     5314 1970-01-01 00:00:00.000000 secscanner2junit-0.1.9/PKG-INFO
```

### Comparing `secscanner2junit-0.1.7/LICENSE` & `secscanner2junit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `secscanner2junit-0.1.7/README.md` & `secscanner2junit-0.1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 - You want to easily access security tool output in merge requests
 
 If you are on the GitLabs Ultimate tier, just use their tooling! No need to mess up your `.gitlab-ci.yml` file. :smile:
 
 ## Which scanning types are supported?
 All scanning types available under the free tier:
 - Secret Scanning
-- Static Application Security Testing
+- Static Application Security Testing (SAST)
+- Container Scanning
 - Infrastructure as Code Scanning
 
 ## How to use?
 Procedure:
 1. Overwrite the existing job so that the report can be used by future jobs.  
 2. Convert report
 3. Upload converted report as junit report
@@ -100,14 +101,39 @@
     - ss2ju sast gl-sast-brakeman-report.json gl-sast-brakeman-report.xml
   artifacts:
     reports:
       junit: gl-sast-brakeman-report.xml
 
 ```
 
+**Example for Container Scanning**
+
+```yml
+- include:
+  - template: Jobs/Build.gitlab-ci.yml #Build and push the container image
+  - template: Security/Container-Scanning.gitlab-ci.yml #Scan the built image
+
+container_scanning:
+  artifacts:
+    paths:
+      - gl-container-scanning-report-format.json
+    when: always
+
+container_scanning-convert:
+  stage: convert
+  dependencies:
+    - container_scanning
+  script:
+    - pip3 install SecScanner2JUnit
+    - ss2ju container_scanning gl-container-scanning-report.json gl-container-scanning-report.xml
+  artifacts:
+    reports:
+      junit: gl-container-scanning-report.xml
+```
+
 **Suppression**
 
 You can provide a file with suppression which will allow to ignore some vulnerabilities.
 
 You have to create a file `ss2ju-config.yml` f.e. in `.gitlab` directory which includes:
 
 ```yml
@@ -115,15 +141,15 @@
   suppressions:
     - type: "cwe"
       value: "2555"
     - type: "find_sec_bugs_type"
       value: "SPRING_ENDPOINT"
 ```
 
-And now you can modify execution command as follows:
+And now you can modify execution commands as follows:
 
 ```bash
     - ss2ju sast gl-sast-semgrep-report.json gl-sast-semgrep-report.xml .gitlab/ss2ju-config.yml
 ```
 
 ## Future Plans
```

### Comparing `secscanner2junit-0.1.7/pyproject.toml` & `secscanner2junit-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secscanner2junit"
-version = "0.1.7"
+version = "0.1.9"
 description = "Convert Security Scanner Output to JUnit Format"
 authors = ["Florian Angermeir <florian.angermeir@tum.de>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/angrymeir/SecScanner2JUnit"
 repository = "https://github.com/angrymeir/SecScanner2JUnit"
 packages = [
```

### Comparing `secscanner2junit-0.1.7/secscanner2junit/__init__.py` & `secscanner2junit-0.1.9/secscanner2junit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import enum
 import json
 import sys
 
 from junit_xml import to_xml_report_file
 
 from secscanner2junit.config import get_config, Config
+from secscanner2junit.container_scanning import ContainerScanningParser
 from .sast import SastParser
 from .secrets import SecretsParser
 
 
 class ScanType(enum.Enum):
     SECRETS = 'secrets'
     SAST = 'sast'
+    CS = 'container_scanning'
 
 
 def load_report(input_path):
     with open(input_path) as input_file:
         report = json.load(input_file)
     return report
 
@@ -36,14 +38,16 @@
     scan_type, input_path, output_path = sys.argv[1], sys.argv[2], sys.argv[3]
     ss2ju_config = load_config()
     report = load_report(input_path)
     if scan_type == ScanType.SECRETS.value:
         parser = SecretsParser(report, input_path, ss2ju_config)
     elif scan_type == ScanType.SAST.value:
         parser = SastParser(report, input_path, ss2ju_config)
+    elif scan_type == ScanType.CS.value:
+        parser = ContainerScanningParser(report, input_path, ss2ju_config)
     else:
         raise NotImplementedError
     testsuite = parser.parse()
     save_junit_report(testsuite, output_path)
 
 
 if __name__ == '__main__':
```

### Comparing `secscanner2junit-0.1.7/secscanner2junit/config.py` & `secscanner2junit-0.1.9/secscanner2junit/config.py`

 * *Files identical despite different names*

### Comparing `secscanner2junit-0.1.7/secscanner2junit/sast.py` & `secscanner2junit-0.1.9/secscanner2junit/sast.py`

 * *Files identical despite different names*

### Comparing `secscanner2junit-0.1.7/secscanner2junit/secrets.py` & `secscanner2junit-0.1.9/secscanner2junit/secrets.py`

 * *Files identical despite different names*

### Comparing `secscanner2junit-0.1.7/setup.py` & `secscanner2junit-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['PyYAML>=6.0,<7.0', 'junit-xml>=1.9,<2.0']
 
 entry_points = \
 {'console_scripts': ['ss2ju = secscanner2junit:main']}
 
 setup_kwargs = {
     'name': 'secscanner2junit',
-    'version': '0.1.7',
+    'version': '0.1.9',
     'description': 'Convert Security Scanner Output to JUnit Format',
-    'long_description': '# SecScanner2JUnit\n[![PyPI version](https://badge.fury.io/py/secscanner2junit.svg)](https://badge.fury.io/py/secscanner2junit)\n[![Downloads](https://pepy.tech/badge/secscanner2junit)](https://pepy.tech/project/secscanner2junit)\n\n[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/angrymeir/SecScanner2JUnit)\n\nGitLab offers [security scanning and visualization](https://docs.gitlab.com/ee/user/application_security/) directly via and on their platform.  \nOne nice feature is direct insights on merge requests. However, this feature is only available with the Ultimate tier. To also use this feature on the free tier, one can build around it by taking the security tool output, converting it to the JUnit format, and uploading it as JUnit report.\n\nTo summarize, this tool is for you if:\n- You use GitLab\'s free tier\n- You use Gitlabs [security templates](https://docs.gitlab.com/ee/user/application_security/)\n- You want to easily access security tool output in merge requests\n\nIf you are on the GitLabs Ultimate tier, just use their tooling! No need to mess up your `.gitlab-ci.yml` file. :smile:\n\n## Which scanning types are supported?\nAll scanning types available under the free tier:\n- Secret Scanning\n- Static Application Security Testing\n- Infrastructure as Code Scanning\n\n## How to use?\nProcedure:\n1. Overwrite the existing job so that the report can be used by future jobs.  \n2. Convert report\n3. Upload converted report as junit report\n\n**Example for Secret Scanning**  \nThis example can be used as is.\n```yaml\nstages:\n  - test\n  - convert\n  \n- include:\n  - template: Security/Secret-Detection.gitlab-ci.yml\n  \nsecret_detection:\n  artifacts:\n    paths:\n      - gl-secret-detection-report.json\n    when: always\n    \nsecret_convert:\n  stage: convert\n  dependencies:\n    - secret_detection\n  script:\n    - pip3 install SecScanner2JUnit\n    - ss2ju secrets gl-secret-detection-report.json gl-secret-detection-report.xml\n  artifacts:\n    reports:\n      junit: gl-secret-detection-report.xml\n```\n\n**Example for SAST**  \nSince GitLab decides dynamically which scanners to use depending on project languages, it makes sense to first perform a testrun only including the template. This way one can see which jobs are executed and then overwrite them. \n```yaml\nstages:\n  - test\n  - convert\n  \n- include:\n  - template: Security/SAST.gitlab-ci.yml\n  \nsemgrep-sast:\n  after_script:\n    - cp gl-sast-report.json gl-sast-semgrep-report.json\n  artifacts:\n    paths:\n      - gl-sast-semgrep-report.json\n    when: always\n\nbrakeman-sast:\n  after_script:\n    - cp gl-sast-report.json gl-sast-brakeman-report.json\n  artifacts:\n    paths:\n      - gl-sast-brakeman-report.json\n    when: always\n\nsemgrep-sast-convert:\n  stage: convert\n  dependencies:\n    - semgrep-sast\n  script:\n    - pip3 install SecScanner2JUnit\n    - ss2ju sast gl-sast-semgrep-report.json gl-sast-semgrep-report.xml\n  artifacts:\n    reports:\n      junit: gl-sast-semgrep-report.xml\n      \nbrakeman-sast-convert:\n  stage: convert\n  dependencies:\n    - brakeman-sast\n  script:\n    - pip3 install SecScanner2JUnit\n    - ss2ju sast gl-sast-brakeman-report.json gl-sast-brakeman-report.xml\n  artifacts:\n    reports:\n      junit: gl-sast-brakeman-report.xml\n\n```\n\n**Suppression**\n\nYou can provide a file with suppression which will allow to ignore some vulnerabilities.\n\nYou have to create a file `ss2ju-config.yml` f.e. in `.gitlab` directory which includes:\n\n```yml\nsast:\n  suppressions:\n    - type: "cwe"\n      value: "2555"\n    - type: "find_sec_bugs_type"\n      value: "SPRING_ENDPOINT"\n```\n\nAnd now you can modify execution command as follows:\n\n```bash\n    - ss2ju sast gl-sast-semgrep-report.json gl-sast-semgrep-report.xml .gitlab/ss2ju-config.yml\n```\n\n## Future Plans\n\n- [ ] Implement IaC Scanning\n',
+    'long_description': '# SecScanner2JUnit\n[![PyPI version](https://badge.fury.io/py/secscanner2junit.svg)](https://badge.fury.io/py/secscanner2junit)\n[![Downloads](https://pepy.tech/badge/secscanner2junit)](https://pepy.tech/project/secscanner2junit)\n\n[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/angrymeir/SecScanner2JUnit)\n\nGitLab offers [security scanning and visualization](https://docs.gitlab.com/ee/user/application_security/) directly via and on their platform.  \nOne nice feature is direct insights on merge requests. However, this feature is only available with the Ultimate tier. To also use this feature on the free tier, one can build around it by taking the security tool output, converting it to the JUnit format, and uploading it as JUnit report.\n\nTo summarize, this tool is for you if:\n- You use GitLab\'s free tier\n- You use Gitlabs [security templates](https://docs.gitlab.com/ee/user/application_security/)\n- You want to easily access security tool output in merge requests\n\nIf you are on the GitLabs Ultimate tier, just use their tooling! No need to mess up your `.gitlab-ci.yml` file. :smile:\n\n## Which scanning types are supported?\nAll scanning types available under the free tier:\n- Secret Scanning\n- Static Application Security Testing (SAST)\n- Container Scanning\n- Infrastructure as Code Scanning\n\n## How to use?\nProcedure:\n1. Overwrite the existing job so that the report can be used by future jobs.  \n2. Convert report\n3. Upload converted report as junit report\n\n**Example for Secret Scanning**  \nThis example can be used as is.\n```yaml\nstages:\n  - test\n  - convert\n  \n- include:\n  - template: Security/Secret-Detection.gitlab-ci.yml\n  \nsecret_detection:\n  artifacts:\n    paths:\n      - gl-secret-detection-report.json\n    when: always\n    \nsecret_convert:\n  stage: convert\n  dependencies:\n    - secret_detection\n  script:\n    - pip3 install SecScanner2JUnit\n    - ss2ju secrets gl-secret-detection-report.json gl-secret-detection-report.xml\n  artifacts:\n    reports:\n      junit: gl-secret-detection-report.xml\n```\n\n**Example for SAST**  \nSince GitLab decides dynamically which scanners to use depending on project languages, it makes sense to first perform a testrun only including the template. This way one can see which jobs are executed and then overwrite them. \n```yaml\nstages:\n  - test\n  - convert\n  \n- include:\n  - template: Security/SAST.gitlab-ci.yml\n  \nsemgrep-sast:\n  after_script:\n    - cp gl-sast-report.json gl-sast-semgrep-report.json\n  artifacts:\n    paths:\n      - gl-sast-semgrep-report.json\n    when: always\n\nbrakeman-sast:\n  after_script:\n    - cp gl-sast-report.json gl-sast-brakeman-report.json\n  artifacts:\n    paths:\n      - gl-sast-brakeman-report.json\n    when: always\n\nsemgrep-sast-convert:\n  stage: convert\n  dependencies:\n    - semgrep-sast\n  script:\n    - pip3 install SecScanner2JUnit\n    - ss2ju sast gl-sast-semgrep-report.json gl-sast-semgrep-report.xml\n  artifacts:\n    reports:\n      junit: gl-sast-semgrep-report.xml\n      \nbrakeman-sast-convert:\n  stage: convert\n  dependencies:\n    - brakeman-sast\n  script:\n    - pip3 install SecScanner2JUnit\n    - ss2ju sast gl-sast-brakeman-report.json gl-sast-brakeman-report.xml\n  artifacts:\n    reports:\n      junit: gl-sast-brakeman-report.xml\n\n```\n\n**Example for Container Scanning**\n\n```yml\n- include:\n  - template: Jobs/Build.gitlab-ci.yml #Build and push the container image\n  - template: Security/Container-Scanning.gitlab-ci.yml #Scan the built image\n\ncontainer_scanning:\n  artifacts:\n    paths:\n      - gl-container-scanning-report-format.json\n    when: always\n\ncontainer_scanning-convert:\n  stage: convert\n  dependencies:\n    - container_scanning\n  script:\n    - pip3 install SecScanner2JUnit\n    - ss2ju container_scanning gl-container-scanning-report.json gl-container-scanning-report.xml\n  artifacts:\n    reports:\n      junit: gl-container-scanning-report.xml\n```\n\n**Suppression**\n\nYou can provide a file with suppression which will allow to ignore some vulnerabilities.\n\nYou have to create a file `ss2ju-config.yml` f.e. in `.gitlab` directory which includes:\n\n```yml\nsast:\n  suppressions:\n    - type: "cwe"\n      value: "2555"\n    - type: "find_sec_bugs_type"\n      value: "SPRING_ENDPOINT"\n```\n\nAnd now you can modify execution commands as follows:\n\n```bash\n    - ss2ju sast gl-sast-semgrep-report.json gl-sast-semgrep-report.xml .gitlab/ss2ju-config.yml\n```\n\n## Future Plans\n\n- [ ] Implement IaC Scanning\n',
     'author': 'Florian Angermeir',
     'author_email': 'florian.angermeir@tum.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/angrymeir/SecScanner2JUnit',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `secscanner2junit-0.1.7/PKG-INFO` & `secscanner2junit-0.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secscanner2junit
-Version: 0.1.7
+Version: 0.1.9
 Summary: Convert Security Scanner Output to JUnit Format
 Home-page: https://github.com/angrymeir/SecScanner2JUnit
 License: GPL-3.0-only
 Author: Florian Angermeir
 Author-email: florian.angermeir@tum.de
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -34,15 +34,16 @@
 - You want to easily access security tool output in merge requests
 
 If you are on the GitLabs Ultimate tier, just use their tooling! No need to mess up your `.gitlab-ci.yml` file. :smile:
 
 ## Which scanning types are supported?
 All scanning types available under the free tier:
 - Secret Scanning
-- Static Application Security Testing
+- Static Application Security Testing (SAST)
+- Container Scanning
 - Infrastructure as Code Scanning
 
 ## How to use?
 Procedure:
 1. Overwrite the existing job so that the report can be used by future jobs.  
 2. Convert report
 3. Upload converted report as junit report
@@ -121,14 +122,39 @@
     - ss2ju sast gl-sast-brakeman-report.json gl-sast-brakeman-report.xml
   artifacts:
     reports:
       junit: gl-sast-brakeman-report.xml
 
 ```
 
+**Example for Container Scanning**
+
+```yml
+- include:
+  - template: Jobs/Build.gitlab-ci.yml #Build and push the container image
+  - template: Security/Container-Scanning.gitlab-ci.yml #Scan the built image
+
+container_scanning:
+  artifacts:
+    paths:
+      - gl-container-scanning-report-format.json
+    when: always
+
+container_scanning-convert:
+  stage: convert
+  dependencies:
+    - container_scanning
+  script:
+    - pip3 install SecScanner2JUnit
+    - ss2ju container_scanning gl-container-scanning-report.json gl-container-scanning-report.xml
+  artifacts:
+    reports:
+      junit: gl-container-scanning-report.xml
+```
+
 **Suppression**
 
 You can provide a file with suppression which will allow to ignore some vulnerabilities.
 
 You have to create a file `ss2ju-config.yml` f.e. in `.gitlab` directory which includes:
 
 ```yml
@@ -136,15 +162,15 @@
   suppressions:
     - type: "cwe"
       value: "2555"
     - type: "find_sec_bugs_type"
       value: "SPRING_ENDPOINT"
 ```
 
-And now you can modify execution command as follows:
+And now you can modify execution commands as follows:
 
 ```bash
     - ss2ju sast gl-sast-semgrep-report.json gl-sast-semgrep-report.xml .gitlab/ss2ju-config.yml
 ```
 
 ## Future Plans
```

